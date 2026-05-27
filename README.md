# Construtora Vista

> Landing page premium para construtora, reformas e projetos arquitetônicos em Bragança Paulista, SP.

---

## Sobre o Projeto

A **Construtora Vista** é uma landing page corporativa de alto padrão, desenvolvida para transmitir **confiança, segurança e sofisticação técnica** — valores essenciais no setor da construção civil.

A experiência foi desenhada no nível de uma agência internacional: design refinado com **glassmorphism**, gradientes mesh sutis, sombras em camadas, textura de grão, grid bento e tipografia fluida. As animações de reveal usam **CSS custom + Intersection Observer** como base robusta (funcionam sem JS pesado), com **GSAP + ScrollTrigger** como camada de aprimoramento progressivo para parallax suave. O objetivo é converter visitantes em leads qualificados através de uma jornada clara: conhecer os serviços, entender o processo, explorar o portfólio, validar a confiança via depoimentos e certificações, e solicitar um orçamento grátis.

---

## Tecnologias Utilizadas

| Tecnologia | Versão | Propósito |
|---|---|---|
| HTML5 | — | Estrutura semântica, acessível, single-file |
| Tailwind CSS | Play CDN v3.x | Estilização utilitária + customizações via `@layer` |
| Lucide Icons | Latest | Ícones vetoriais limpos e consistentes |
| GSAP + ScrollTrigger | 3.12.x (CDN) | Parallax suave — aprimoramento progressivo (degrada para fallback nativo) |
| Google Fonts | — | **Sora** (display/títulos) + **Inter** (corpo) |
| JavaScript (vanilla) | ES6 | Reveals, contadores, cursor magnético, menu, barra de progresso — zero frameworks de UI |

Sem build, sem bundler, sem React/Vue. O GSAP é opcional: se não carregar, o parallax do hero usa um fallback nativo e os reveals continuam funcionando via Intersection Observer.

---

## Paleta de Cores

- **Graphite / Ink** (`#0B0F1A`) — Fundo escuro principal, transmite solidez e sofisticação
- **Ink2** (`#131826`) — Superfícies elevadas (rodapé, menu mobile)
- **Cinza Ardósia** (`#64748B`) — Cor corporativa de apoio, textos secundários
- **Laranja Segurança** (`#F97316` / `#EA580C`) — Destaque para CTAs e elementos interativos
- **Sand / Off-white** (`#FAFAF8`) — Fundos claros e quentes para seções de leitura

---

## Estrutura do Site

1. **Loader** — Curtain de carregamento com marca e barra animada (respeita `reduced-motion`)
2. **Navegação Fixa** — Glassmorphism ao scroll, menu hambúrguer animado, link ativo dinâmico, barra de progresso de leitura
3. **Hero** — Imagem com **parallax GPU**, headline com gradiente, CTA magnético e estatísticas com **contador animado**
4. **Serviços** — 6 cards com micro-interações, seta revelada no hover e reveal escalonado (stagger)
5. **Processo** — Timeline de 4 etapas em cartões glass (Diagnóstico → Projeto → Execução → Entrega)
6. **Diferenciais** — Checklist em cartões, foto em parallax e badges flutuantes (obras + avaliação)
7. **Portfólio** — **Grid bento** de 6 obras com overlay animado, zoom suave e foco por teclado
8. **Depoimentos** — 3 cards de clientes com avaliação em estrelas
9. **Certificações** — CREA-SP, ISO 9001, NR 18, GBC Brasil + marquee de parceiros
10. **Orçamento Grátis** — Formulário acessível com validação e status `aria-live`
11. **Footer** — Navegação, serviços, contato e redes sociais
12. **WhatsApp Flutuante** — Botão fixo com pulso animado para conversão imediata

---

## Destaques de UI/UX

- **Glassmorphism** na navbar e nos cartões do processo
- **Gradientes mesh** e **textura de grão** sutil para profundidade premium
- **Reveals** via Intersection Observer com **stagger** em cards e listas
- **Parallax suave** (GSAP ScrollTrigger, com fallback nativo) no hero e na foto de diferenciais
- **Contadores animados** com easing nas estatísticas
- **Cursor customizado** com ring + **botões magnéticos** (apenas ponteiro fino)
- **Grid bento** no portfólio e **micro-interações**: hover lift, glow, seta revelada, shimmer no CTA
- **Barra de progresso** de leitura e **link de navegação ativo** conforme a seção visível
- **Marquee** infinito de parceiros que pausa ao passar o mouse

---

## Responsividade & Performance

- **Mobile-first** com breakpoints precisos do Tailwind
- **Tipografia fluida** com `clamp()` (escala perfeitamente entre telas)
- **Menu hambúrguer animado** e interações touch-friendly
- **Lazy loading nativo** (`loading="lazy"`) com fade-in nas imagens
- **Preconnect** para fonts, CDNs e Unsplash
- Animações restritas a `transform` e `opacity` para 60fps

---

## Acessibilidade

- Contraste em conformidade com **WCAG AA**
- **Skip link** e landmarks semânticas (`header`, `main`, `nav`, `footer`)
- **Aria labels** em elementos interativos e ícones decorativos marcados como `aria-hidden`
- **Focus states** visíveis (`:focus-visible`)
- Formulário com `label` associado a cada campo e status `aria-live`
- **`prefers-reduced-motion`** respeitado — todas as animações são desativadas

---

## Como Visualizar

Abra o arquivo `index.html` diretamente em qualquer navegador moderno. Não requer build ou servidor — todos os assets são carregados via CDN.

```bash
# Opção 1: abrir diretamente
open index.html

# Opção 2: servidor local simples (Python)
python3 -m http.server 8080
# Acesse http://localhost:8080
```

---

## Créditos

- **Imagens**: [Unsplash](https://unsplash.com) — fotografias reais de construção civil
- **Ícones**: [Lucide](https://lucide.dev)
- **Framework CSS**: [Tailwind CSS](https://tailwindcss.com)
- **Tipografia**: Google Fonts (Sora + Inter)

---

## Desenvolvimento

Projeto desenvolvido por **[JulioAkaminee](https://github.com/JulioAkaminee)** como parte do portfólio da **Akamine Web Studio**.

A Akamine Web Studio cria experiências digitais de alto impacto para empresas de Bragança Paulista e região. Sites modernos, responsivos e otimizados para conversão.

📍 Bragança Paulista, SP
🔗 [github.com/JulioAkaminee](https://github.com/JulioAkaminee)

---

## Licença

Este projeto é de uso exclusivo para demonstração. As imagens são de uso editorial via Unsplash License.
