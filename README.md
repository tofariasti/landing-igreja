# Nova Vida — Igreja Comunitária

Landing page de alta conversão para igreja fictícia, desenvolvida com foco em responsividade, acessibilidade e integração WhatsApp para agendamento de visitas.

[![Live Demo](https://img.shields.io/badge/demo-online-brightgreen)](https://tofariasti.github.io/landing-igreja/)

## Demo

**Moldura (preview):** [https://tofariasti.github.io/landing-igreja/](https://tofariasti.github.io/landing-igreja/)

**Tela cheia:** [https://tofariasti.github.io/landing-igreja/site/](https://tofariasti.github.io/landing-igreja/site/)

## Screenshots

### Desktop (1280px)
![Desktop view](screenshots/desktop.png)

### Tablet (768px)
![Tablet view](screenshots/tablet.png)

### Mobile (390px)
![Mobile view](screenshots/mobile.png)

## Funcionalidades

- Design responsivo (mobile-first) com identidade índigo e dourado
- Integração WhatsApp com formulário estruturado para agendamento de visita
- Animações ao scroll (AOS) + partículas, contadores e hover effects
- Acessibilidade WCAG 2.1 AA (skip link, ARIA, foco visível, reduced motion)
- SEO básico (meta description, HTML semântico)
- Botão flutuante WhatsApp com pulse
- FAQ accordion interativo
- Galeria com lazy loading
- Moldura iframe com preview desktop/tablet/mobile

## Seções

1. **Hero** — Headline inspiradora, CTAs, estatísticas animadas e imagem de culto
2. **Sobre** — Missão, visão e valores
3. **Programação** — Cultos, EBD, células, jovens, kids e oração
4. **Ministérios** — Louvor, jovens, crianças, ação social, casais e missões
5. **Como funciona** — 3 passos: conheça, participe, cresça
6. **Galeria** — Fotos de cultos, comunidade e eventos
7. **Depoimentos** — 3 testemunhos fictícios
8. **CTA** — Convite para primeira visita
9. **FAQ** — Dress code, estacionamento, crianças, células
10. **Contato** — Formulário WhatsApp para agendamento
11. **Footer** — Endereço, horários, redes e créditos

## Tecnologias

- HTML5 semântico
- CSS3 (Flexbox/Grid, custom properties)
- JavaScript vanilla (ES6+)
- AOS (Animate On Scroll) v2.3.4
- Font Awesome 6.4
- Google Fonts (Playfair Display + Source Sans 3)

## Testes de Responsividade

| Dispositivo | Resolução | Status | Verificado |
|-------------|-----------|--------|------------|
| iPhone SE | 375×667 | ✅ | Menu mobile, formulário, float WhatsApp |
| iPhone 12 Pro | 390×844 | ✅ | Hero, CTAs above the fold |
| iPhone 14 Pro Max | 428×926 | ✅ | Grid programação, depoimentos |
| iPad | 768×1024 | ✅ | Grid 2 colunas, FAQ, galeria |
| Desktop HD | 1280×720 | ✅ | Layout completo, moldura preview |
| Desktop FHD | 1920×1080 | ✅ | Max-width container, galeria |

## Acessibilidade

- Semântica HTML5 (`header`, `main`, `footer`, `nav`, landmarks)
- Skip link para conteúdo principal
- Atributos ARIA (`aria-expanded`, `aria-label`, `role="alert"` em erros)
- Contraste WCAG AA — dourado #d4a843 sobre índigo #1a1347 e branco #f8f6f0
- Navegação por teclado (Escape fecha menu mobile)
- Focus states visíveis em todos os interativos
- Alt text descritivo em imagens
- Labels explícitos em formulários
- Font-size mínimo 16px em inputs mobile
- `prefers-reduced-motion`: desabilita AOS, partículas, pulse e contadores

## Como usar

```bash
git clone https://github.com/tofariasti/landing-igreja.git
cd landing-igreja
# Abrir index.html no navegador (preview com moldura iframe)
# Ou abrir site/index.html para tela cheia
python3 -m http.server 8080
```

## Screenshots (geração)

```bash
python3 -m http.server 8765
npm install
npm run screenshots
```

## Personalização

1. **WhatsApp:** altere `WHATSAPP_NUMBER` em `site/assets/js/main.js`
2. **Cores:** edite as variáveis CSS em `:root` no `site/assets/css/style.css`
3. **Textos:** edite `site/index.html`

## Estrutura

```
igreja/
├── index.html              # Preview shell (moldura iframe)
├── assets/css/preview.css
├── assets/js/preview.js
├── site/
│   ├── index.html          # Landing page
│   └── assets/
│       ├── css/style.css
│       └── js/main.js
├── screenshots/
├── scripts/capture-screenshots.mjs
├── .github/workflows/deploy.yml
└── README.md
```

## Autor

**Tiago O. de Farias** — [Farias Digital](https://fariasdigital.com.br/)

- GitHub: [@tofariasti](https://github.com/tofariasti)
- WhatsApp: [(51) 99121-3724](https://wa.me/5551991213724)

---

<p align="center">
  <a href="https://tofariasti.github.io/landing-igreja/">🌐 Demo Online</a> ·
  <a href="https://fariasdigital.com.br/">🏢 Site Comercial</a>
</p>
