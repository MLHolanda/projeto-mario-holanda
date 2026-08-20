# Bloco 02 — Expansão da Estrutura e dos Caminhos

**Versão:** Em andamento  
**Status:** Parcialmente implementado  
**Data de início:** 20 de agosto de 2026

---

## 1. Objetivo do Bloco 02

Após a conclusão do Bloco 01, o Projeto Mário Holanda possuía sua fundação estrutural e visual: Design System, layout base, Header, Navigation, Footer e a Home como porta de entrada da experiência.

O objetivo do Bloco 02 é expandir essa estrutura inicial, transformando a Home de uma **capa isolada** em uma experiência de **Capa + Sumário**, permitindo que o visitante encontre caminhos reais para as principais áreas do projeto.

A intenção é preservar os princípios definidos na documentação oficial:

- Conteúdo antes da tecnologia;
- Simplicidade e acolhimento;
- Navegação clara;
- Liberdade para explorar sem impor uma ordem;
- Crescimento progressivo do projeto;
- Estrutura preparada para evoluir sem reconstruções desnecessárias.

---

## 2. Análise realizada antes da implementação

Antes da execução do Bloco 02, foram analisados:

- `docs/PRD.md`;
- `docs/DESIGN.md`;
- `docs/DECISOES_TECNICAS.md`;
- `docs/03_FSD.md`;
- estrutura atual do projeto;
- componentes existentes;
- layout base;
- estilos globais;
- Home implementada no Bloco 01.

A análise foi realizada antes de qualquer nova implementação.

O entendimento consolidado foi que o projeto não deveria concentrar todo o conteúdo em uma única página, nem transformar a Home apenas em uma lista de links.

A solução escolhida foi uma combinação entre entrada narrativa e páginas independentes.

---

## 3. Decisão de Arquitetura: Capa + Sumário

Foi definida a seguinte organização conceitual:

```text
Home
│
├── Capa / Entrada narrativa
│
└── Sumário / Caminhos principais
    │
    ├── Capítulos
    ├── Projetos
    ├── Aprendizados
    ├── Pensamentos
    └── Contato
