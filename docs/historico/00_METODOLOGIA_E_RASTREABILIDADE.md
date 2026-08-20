# Metodologia e Rastreabilidade do Projeto Mário Holanda

**Versão:** 1.0  
**Status:** Oficial  
**Data:** 20 de Agosto de 2026  
**Método de Referência:** Jornada IA — Vibe Coding v1.5

---

## 1. Propósito da Rastreabilidade

O objetivo desta documentação histórica não é transcrever exaustivamente cada comando isolado ou conversa pontual, mas **preservar e organizar o contexto estratégico, técnico e metodológico** necessário para compreender como e por que o Projeto Mário Holanda foi construído e evoluiu ao longo do tempo.

A rastreabilidade serve para:
- Registrar decisões de produto, design e arquitetura;
- Preservar instruções e prompts que guiaram a IA e o desenvolvimento;
- Documentar o que foi implementado e como foi validado;
- Permitir que qualquer pessoa (ou a própria IA em sessões futuras) compreenda a trajetória do projeto com clareza, continuidade e fidelidade.

> *"Preservar não apenas o produto, mas também o conhecimento de como e por que ele foi construído."* (03_FSD.md)

---

## 2. Fontes de Evidência

As informações registradas nesta documentação apoiam-se exclusivamente em fontes confiáveis e verificáveis:

1. **Documentação Oficial:** `PRD.md`, `DESIGN.md`, `DECISOES_TECNICAS.md`, `03_FSD.md` e outros documentos aprovados;
2. **Histórico de Versionamento do Git:** Commits, mensagens, timestamps, branches e histórico de alterações;
3. **Código-Fonte e Estrutura do Projeto:** Arquivos de componentes, páginas, estilos, configurações e dependências;
4. **Resultados de Validações:** Verificações estáticas (`astro check`), compilações (`astro build`), testes de acessibilidade e validações visuais;
5. **Instruções e Prompts Disponíveis:** Prompts textuais originais recuperados e registrados durante as sessões de trabalho;
6. **Decisões Registradas:** Alinhamentos e definições estabelecidos explicitamente durante o processo de construção.

---

## 3. Classificação dos Registros

Para assegurar integridade e transparência, os registros históricos são organizados nas seguintes categorias:

### 3.1 Decisão Oficial
Uma diretriz ou escolha técnica/arquitetural/de design conscientemente adotada para orientar os rumos do projeto.

### 3.2 Prompt ou Instrução Registrada
Uma instrução textual cujo conteúdo original está disponível e pode ser transcrito ou resumido com fidelidade direta.

### 3.3 Implementação
O relato objetivo do que foi efetivamente criado, modificado, refatorado ou removido no código-fonte e na estrutura de arquivos.

### 3.4 Validação
O registro de verificações técnicas e de qualidade executadas (ex.: `npx astro check`, `npm run build`, auditorias visuais, conformidade de Design System, acessibilidade por teclado e leitores de tela).

### 3.5 Reconstrução Histórica
Um registro estruturado posteriormente a partir da análise combinada de evidências técnicas, documentação e histórico do Git, aplicado a etapas anteriores em que o prompt literal original não estava gravado.

> **Regra fundamental:** Uma reconstrução histórica jamais deve ser apresentada como se fosse um prompt literal original.

---

## 4. Regras para Reconstruções Históricas

Quando o texto literal exato de uma instrução não estiver disponível, o histórico do desenvolvimento pode ser reconstituído com base nas evidências existentes, respeitando as seguintes diretrizes:

1. **Identificação Explícita:** Declarar claramente no início da seção que se trata de uma *Reconstrução Histórica*;
2. **Citação de Evidências:** Indicar as fontes técnicas utilizadas (ex.: hashes de commits, arquivos criados, dependências instaladas);
3. **Não-Invenção:** Não criar ou simular diálogos ou prompts literais inexistentes;
4. **Separação de Fatos e Interpretações:** Diferenciar com clareza o que é fato comprovado pelo código/Git daquilo que é dedução lógica sobre a intenção da etapa.

---

## 5. Relação com o Processo de Desenvolvimento

A documentação de histórico acompanha a evolução do projeto e deve ser atualizada em momentos relevantes (ao final de blocos, etapas significativas ou marcos de versão).

Ela existe para **garantir clareza e continuidade**, sem se transformar em uma burocracia excessiva que comprometa o ritmo e a fluidez do desenvolvimento.

---

## 6. Desvios ou Exceções de Processo

O método padrão de trabalho — guiado pela documentação oficial, planejamento prévio, validação passo a passo e implementação consciente — é a norma contínua do projeto e não precisa ser justificado repetidamente a cada etapa.

Caso ocorra alguma situação excepcional que exija desvio temporário do fluxo habitual, a exceção deve:
- Ser **comunicada claramente** antes da execução;
- Ter seu **motivo justificado** de forma transparente;
- Ter seu **impacto técnico e conceitual avaliado**;
- Ser **devidamente registrada** no histórico quando for relevante para a compreensão futura do projeto.

---

## 7. Organização da Pasta de Histórico

A documentação histórica é mantida no diretório `docs/historico/`, com a seguinte estrutura inicial:

```text
docs/historico/
├── 00_METODOLOGIA_E_RASTREABILIDADE.md   # Este documento: metodologia, princípios e regras
├── 01_BLOCO_01_FUNDACAO.md              # Reconstrução histórica da fundação, casca e Home
└── 02_BLOCO_02_EXPANSAO.md              # Registro da expansão estrutural e páginas-índice
```

Novos documentos serão adicionados progressivamente à medida que novos blocos ou marcos importantes forem planejados e concluídos, mantendo a numeração sequencial e a coerência do ecossistema.
