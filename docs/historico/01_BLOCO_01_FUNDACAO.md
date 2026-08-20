# Bloco 01 — Fundação

**Data dos Registros Originais:** 18 a 19 de Agosto de 2026  
**Status do Documento:** Reconstrução Histórica  
**Método de Referência:** Jornada IA — Vibe Coding v1.5

---

## Status da Reconstrução Histórica

> **Aviso de Rastreabilidade:** Este documento constitui uma **Reconstrução Histórica** elaborada a partir das evidências técnicas consolidadas no repositório: documentação oficial, histórico de commits do Git, estrutura do código-fonte e registros de validação.
>
> Os prompts literais originais trocados durante o desenvolvimento inicial do Bloco 01 não estão reproduzidos aqui por não estarem gravados no repositório. Nenhuma instrução ou diálogo foi inventado.

---

## 1. Contexto Inicial

O marco inaugural do projeto está registrado em **28 de julho de 2026**, assinalando a conclusão da *Jornada IA: Vibe Coding* e o início da construção consciente do **Projeto Mário Holanda**.

O produto foi concebido não como um portfólio estático ou tradicional, mas como uma **experiência digital narrativa, viva e evolutiva**, fundamentada no conceito central:

> **"Um Capítulo de Cada Vez"**

A experiência foi planejada para apresentar a trajetória de Mário de forma autêntica, acolhedora e progressiva, integrando histórias, aprendizados, projetos e pensamentos. A premissa central é que o projeto crescerá continuamente ao longo dos anos, guiado pela documentação oficial como fonte de verdade para a parceria entre Mário e a IA.

---

## 2. Fundação Documental

A estruturação inicial foi consolidada formalmente através do conjunto de documentos técnicos e conceituais na pasta `docs/`.

* **Commit identificado:** `ea1b4e3` — *docs: adiciona documentação base do projeto* (18/08/2026)

### Papel de cada documento:
- **`docs/PRD.md` (Product Requirements Document):** Define o propósito, os princípios (Autenticidade, Simplicidade, Acolhimento, Evolução, Presença), os Requisitos Funcionais (RF-01 a RF-10) e Não Funcionais (RNF-01 a RNF-10), além dos limites e visão do MVP.
- **`docs/DESIGN.md`:** Estabelece a identidade visual e atmosfera editorial, definindo a paleta de cores (`--color-primary: #0B1F3A`, `--color-secondary: #0F766E`, `--color-accent: #C9A227`, `--color-text: #1F2937`, `--color-background: #F5F7FA`), a tipografia (*Merriweather* para títulos e *Inter* para corpo/interface), a escala de espaçamento modular (`--space-1` a `--space-11`), limites de contêiner e diretrizes de acessibilidade.
- **`docs/DECISOES_TECNICAS.md`:** Formaliza a escolha do **Astro** como framework principal do MVP, a ausência de banco de dados e backend no núcleo inicial, a independência do Blog existente, e os critérios de acessibilidade, desempenho e SEO.
- **`docs/03_FSD.md` (Functional Specification Document):** Consolidação v1.1 do comportamento funcional esperado para cada área da experiência, regras para a IA codadora e os critérios de aceitação.

---

## 3. Preparação da Infraestrutura

A preparação técnica do ambiente ocorreu em etapas documentadas no Git:

### 3.1 Dependências do Astro
* **Commit:** `0936756` — *chore: configura dependencias do Astro* (18/08/2026)
* **Evidência:** Inclusão de `package.json` e `package-lock.json`, estabelecendo as dependências base do framework Astro.

### 3.2 Estrutura Inicial do Astro
* **Commit:** `2c739df` — *feat: inicializa estrutura Astro* (19/08/2026)
* **Evidência:** Criação dos arquivos de configuração essenciais:
  - `astro.config.mjs`: Configuração do Astro;
  - `tsconfig.json`: Configuração de tipagem estrita TypeScript;
  - `src/pages/index.astro`: Estrutura inicial da página de entrada.

### 3.3 Ajustes de Referência e Scripts
* **Commit:** `3af4029` — *chore: ajusta configuracao e referencias do projeto* (19/08/2026)
* **Evidência:** Padronização das referências nominais ao documento `03_FSD.md` nos arquivos de documentação e consolidação dos scripts de execução no `package.json` (`dev`, `build`, `preview`, `astro`).

---

## 4. Implementação do Bloco 01

O Bloco 01 estabeleceu a fundação visual, semântica e estrutural do projeto, integrando o Design System aos primeiros componentes e à página inicial.

* **Commit:** `e298ddf` — *feat: conclui estrutura do Bloco 01* (19/08/2026)

### Arquivos implementados e suas responsabilidades:

#### `src/styles/global.css`
- Declaração dos Design Tokens no `:root` (paleta de cores, tipografia, escala tipográfica com adaptação mobile, escala modular de espaçamento);
- Classes de contenção de leitura e seções amplas (`.container-reading` e `.container-wide`);
- Reset CSS consistente e seguro;
- Regras universais de acessibilidade (foco visível de alto contraste `:focus-visible`, classe `.skip-link` para navegação por teclado e suporte a `prefers-reduced-motion`).

#### `src/layouts/BaseLayout.astro`
- Composição estrutural do documento HTML (`<!DOCTYPE html>`, `<head>`, `<body>`);
- Injeção de metadados (`title`, `description`, `lang`);
- Carregamento assíncrono das fontes oficiais (*Merriweather* e *Inter*) via Google Fonts;
- Implementação do skip-link acessível no topo do DOM;
- Delimitação semântica do landmark `<main id="main-content">` via `<slot />`;
- Integração modular com os componentes `Header` e `Footer`.

#### `src/components/Header.astro`
- Landmark semântico `<header>`;
- Identidade visual e tipográfica do projeto ("Mário Holanda — Um Capítulo de Cada Vez");
- Integração do componente de navegação (`Navigation.astro`) com diagramação responsiva.

#### `src/components/Navigation.astro`
- Landmark semântico `<nav aria-label="Navegação principal">`;
- Estruturação dos caminhos principais através de links provisórios em âncora (`#capitulos`, `#projetos`, `#aprendizados`, `#pensamentos`, `#contato`);
- Preservação de área de toque mínima confortável (44px) para acessibilidade mobile.

#### `src/components/Footer.astro`
- Landmark semântico `<footer>`;
- Mensagem de continuidade narrativa:
  > *"A história continua."*
- Assinatura do conceito *"Um Capítulo de Cada Vez"* e menção de direitos autorais dinamicamente datada.

#### `src/pages/index.astro`
- Página inicial atuando como Capa e Entrada da experiência;
- Seção Hero (`<section class="hero-entry">`) contendo:
  - Eyebrow de contexto (*"Trajetória em construção"*);
  - Título principal `H1` (*"Mário Holanda"*);
  - Subtítulo conceitual (*"Um Capítulo de Cada Vez"*);
  - Texto introdutório acolhedor;
  - Frase central do projeto:
    > *"O livro não precisa estar terminado para começar a ser lido."*

---

## 5. Decisões Consolidadas pelo Bloco 01

A conclusão do Bloco 01 consolidou as seguintes decisões de arquitetura e design:
1. **Astro como gerador estático (SSG):** Desempenho nativo, HTML limpo e ausência de complexidade desnecessária;
2. **Arquitetura estática e sem backend:** Foco exclusivo na experiência editorial, sem banco de dados ou APIs dinâmicas no núcleo;
3. **Componentes semânticos e reutilizáveis:** Separação estrita de responsabilidades entre Layout, Header, Navigation e Footer;
4. **Design System integrado:** Fidelidade estrita aos tokens definidos em `DESIGN.md`;
5. **Acessibilidade estrutural desde o início:** Skip-links, contrastes adequados, área de toque mínima e foco visível;
6. **Conteúdo em primeiro lugar:** A tecnologia permanece a serviço da narrativa humana;
7. **Home como Capa:** A página inicial funcionando como acolhimento e declaração de princípios.

---

## 6. Validação Registrada

Antes do encerramento do Bloco 01, o projeto passou pelas seguintes etapas formais de verificação técnica:

### Verificação Estática e de Tipagem:
```bash
npx astro check
```
**Resultado:**
- 0 errors
- 0 warnings
- 0 hints

### Compilação de Produção:
```bash
npx astro build
```
**Resultado:**
- Build concluído com sucesso;
- 1 página estática construída (`/index.html`);
- Sem erros de assets ou links quebrados.

### Validação Visual:
- Inspeção visual executada, confirmando a fidelidade à identidade estética, hierarquia tipográfica, contraste de cores e responsividade em diferentes larguras de tela.

---

## 7. Versionamento e Publicação

A fundação do Bloco 01 foi formalizada no Git com os seguintes dados:

* **Commit:** `e298ddf369d94f9935f7f585133be955c1b1ba23`
* **Mensagem:** `feat: conclui estrutura do Bloco 01`
* **Data:** 19 de Agosto de 2026 às 22:13:45 (-03:00)
* **Status:** Commit realizado na branch `main` e sincronizado com sucesso no repositório remoto (`origin/main`).

---

## 8. Limites do Bloco 01

O Bloco 01 entregou a fundação essencial, deixando expressamente fora de seu escopo (para implementação nos blocos subsequentes):
- Páginas-índice reais e rotas independentes para as seções;
- Capítulos e histórias individuais;
- Páginas e detalhamento individual de projetos;
- Conteúdo estruturado dinâmico / Content Collections;
- Suporte a múltiplos idiomas (i18n / PT, EN, ES);
- Formulários funcionais de contato;
- Integrações de backend ou banco de dados;
- Recursos de inteligência artificial (Athena pública);
- Ferramentas avançadas de monitoramento.

---

## 9. Resultado da Fundação

O Bloco 01 estabeleceu com sucesso a base técnica, semântica e visual sobre a qual todo o ecossistema do Projeto Mário Holanda pode evoluir com segurança, sem a necessidade de reconstruções estruturais.

O próximo marco planejado no desenvolvimento é o **Bloco 02 — Expansão**, cujo objetivo é transformar a experiência da Home de "Capa isolada" para "Capa + Sumário" e estabelecer as páginas-índice reais para as principais áreas da narrativa.
