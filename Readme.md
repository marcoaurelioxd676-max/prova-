# TechPulse — Portal de Notícias de Tecnologia

Primeira versão funcional (MVP) da página inicial do **TechPulse**, desenvolvida com foco em semântica HTML5, acessibilidade, separação estrita entre estrutura e apresentação (CSS externo) e responsividade mobile-first.

---

## Especificações Técnicas e Justificativas de Design

### 1. Paleta de Cores (Hexadecimal e RGBA)
A escolha cromática foi pensada para transmitir credibilidade editorial, modernidade tecnológica e alto contraste para leitura:
* **Azul Marinho Profundo (`#0F172A`):** Utilizado no cabeçalho e rodapé para ancorar visualmente a página e dar peso institucional à marca.
* **Azul Tecnológico (`#2563EB`) e Azul Ciano (`#38BDF8`):** Aplicados no logotipo, bordas de destaque e botões de ação (CTA) para guiar o olhar do leitor aos elementos interativos.
* **Cinza Ardósia (`#1E293B` e `#475569`):** Empregados nos textos principais sobre fundo claro (`#F8FAFC`), evitando o cansaço visual causado pelo contraste extremo do preto puro (`#000000`).
* **Sombra Suave (`rgba(15, 23, 42, 0.05)`):** Utilizada no cartão de artigo para criar profundidade sutil sem poluir a interface.

### 2. Tipografia e Legibilidade
* **Família Tipográfica:** Pilha de fontes sem serifa nativa (`'Segoe UI', Roboto, Helvetica, Arial, sans-serif`), garantindo carregamento instantâneo e familiaridade visual tanto no Windows/macOS quanto em dispositivos Android/iOS.
* **Hierarquia e Escala:** Tamanho base de `16px` (`1rem`) com altura de linha (`line-height`) de `1.6` para leitura confortável. Títulos escalonados (`2rem` para `<h1>`, `1.75rem` para `<h2>` e `1.35rem` para `<h3>`) estabelecem clara hierarquia visual.

### 3. Espaçamentos, Box Model e Responsividade
* **Respiro Visual:** Uso consistente de `margin` entre blocos (`32px` a `40px`) e `padding` interno (`24px` nos cartões e cabeçalho) para evitar aglomeração de informações.
* **Adaptação Multiplataforma:** O contêiner fluido (`width: 90%; max-width: 1000px`) aliado a `flex-wrap` e media queries (`@media (max-width: 600px)`) reorganiza o menu e expande o botão de ação para `100%` da largura em smartphones, facilitando o toque.

### 4. Tecnologias e Serviços Abordados no Portal
O portal foi estruturado para cobrir os três pilares centrais da computação contemporânea:
* **Inteligência Artificial Generativa:** Foco em LLMs, visão computacional e impactos éticos.
* **Computação em Nuvem (Cloud):** Cobertura de arquiteturas escaláveis, microsserviços e computação serverless.
* **Cibersegurança e Privacidade:** Análises sobre proteção de dados (LGPD), criptografia e segurança ofensiva/defensiva.

---

## Sitemap Visual e Taxonomia de Conteúdo

A arquitetura de informação abaixo organiza o portal por **hierarquia de conteúdo** (do geral para o específico) e **taxonomia temática** (agrupamento por domínios tecnológicos):

```text
[ Página Inicial (Home - TechPulse) ]
│
├── 1. Inteligência Artificial
│   ├── Machine Learning & Deep Learning
│   ├── IA Generativa & LLMs
│   └── Ética e Regulação de IA
│
├── 2. Desenvolvimento & Engenharia
│   ├── Front-end & Web Moderna
│   ├── Back-end & Arquitetura de Software
│   └── DevOps & Cloud Computing
│
└── 3. Cibersegurança & Privacidade
    ├── Defesa Cibernética & Vulnerabilidades
    ├── Criptografia & Blockchain
    └── Legislação e Proteção de Dados
    