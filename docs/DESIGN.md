# DESIGN.md --- Mário Holanda --- Um Capítulo de Cada Vez

**Versão:** 1.0\
**Status:** Consolidado para validação final\
**Método:** Jornada IA --- Vibe Coding v1.5

> **Um Capítulo de Cada Vez.**

## 1. Identidade do projeto

**Nome:** Mário Holanda --- Um Capítulo de Cada Vez

O projeto é uma extensão de seu criador. A tecnologia é meio de
expressão, aprendizado e criação; não é o centro da experiência.

A experiência deve ser humana, verdadeira, acolhedora e acessível a
pessoas com diferentes níveis de conhecimento.

## 2. Conceito visual

O site deve ser percebido como uma experiência que pode ser lida como um
livro: capítulos, narrativa, descoberta e exploração gradual.

**Personalidade visual:** humana, elegante, acolhedora, tecnológica na
medida certa, autêntica, limpa e respirável.

### Princípio central

> Conteúdo primeiro. Tecnologia e efeitos a serviço dele.

## 3. Princípios de design

-   Poucas cores, bem hierarquizadas.
-   Evitar poluição visual.
-   Conteúdo antes da decoração.
-   Hierarquia visual clara.
-   Espaço para respirar.
-   Cards somente quando ajudarem.
-   Efeitos discretos.
-   Liberdade para explorar sem deixar o visitante perdido.
-   A identidade deve estar presente sem tentar aparecer.
-   Toda decisão deve favorecer uma experiência que faça o visitante
    querer continuar.

## 4. Paleta de cores

  Token                  HEX         Função
  ---------------------- ----------- ---------------------------------
  `--color-primary`      `#0B1F3A`   Azul profundo --- primária
  `--color-secondary`    `#0F766E`   Teal/petróleo --- secundária
  `--color-accent`       `#C9A227`   Dourado --- acento
  `--color-text`         `#1F2937`   Grafite --- texto
  `--color-background`   `#F5F7FA`   Neutro claro --- fundo
  `--color-white`        `#FFFFFF`   Branco --- conteúdo e contraste

**Hierarquia:** azul protagonista; teal como apoio; dourado pontual;
grafite, branco e neutros como base.

## 5. Tipografia

**Títulos:** Merriweather\
**Textos e interface:** Inter

Máximo de duas famílias.

### Desktop

-   H1: 48/56, Merriweather 700
-   H2: 36/44, Merriweather 700
-   H3: 24/32, Merriweather 700
-   Corpo: 16/24, Inter 400
-   Pequeno: 14/20, Inter 400
-   Legenda: 12/16, Inter 400

### Mobile

-   H1: 36/44
-   H2: 28/36
-   H3: 20/28
-   Corpo: 16/24
-   Pequeno: 14/20
-   Legenda: 12/16

## 6. Espaçamento

Escala: `4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80 / 96 / 128px`

``` css
--space-1: 4px;
--space-2: 8px;
--space-3: 12px;
--space-4: 16px;
--space-5: 24px;
--space-6: 32px;
--space-7: 48px;
--space-8: 64px;
--space-9: 80px;
--space-10: 96px;
--space-11: 128px;
```

## 7. Layout e grid

-   Área de leitura: aproximadamente 720--760px.
-   Seções visuais: até aproximadamente 1200px.
-   Texto longo nunca ocupa toda a largura.
-   Projetos/cards: 2--3 colunas quando houver espaço.
-   Celular: uma coluna.
-   Telas grandes ganham respiro, não conteúdo excessivamente esticado.

## 8. Responsividade

-   Mobile: até aproximadamente 767px.
-   Tablet: aproximadamente 768--1023px.
-   Desktop: a partir de aproximadamente 1024px.
-   Um único projeto responsivo, sem versões independentes.

> O conteúdo determina a mudança de layout, não o dispositivo.

## 9. Formas, bordas e profundidade

-   Raios suaves e moderados.
-   Bordas discretas.
-   Sombras leves.
-   Sem efeitos pesados.
-   Sem excesso de arredondamento.
-   Sem transformar a interface em coleção de caixas.

## 10. Botões, links e ações

-   Primário: azul profundo.
-   Secundário: discreto, podendo usar teal ou outline.
-   Dourado não é botão principal.
-   Links reconhecíveis e elegantes.
-   Hover e foco sutis, porém perceptíveis.
-   Textos curtos e claros.
-   Poucas ações por seção.

> A ação deve ser evidente sem dominar a experiência.

## 11. Cards e blocos

-   Não são padrão.
-   Usar apenas quando organizarem ou destacarem conteúdo.
-   Sem cards aninhados.
-   Sem sombras pesadas.
-   Capítulos e textos importantes podem existir sem molduras.

> Se o conteúdo funciona melhor sem uma caixa, não colocamos uma caixa.

## 12. Formulários

Campos limpos e espaçosos; rótulos claros; bordas discretas; foco
visível; erros claros e humanos; sucesso discreto; áreas de toque
confortáveis.

## 13. Estados

Normal, hover, foco, ativo/selecionado, desabilitado, erro, sucesso e
carregamento, quando aplicável.

Cada estado deve comunicar o que acontece sem quebrar a experiência de
leitura.

## 14. Ícones e linguagem gráfica

-   Família visual consistente.
-   Ícones simples e limpos.
-   Sem mistura de estilos.
-   Usar ícones quando houver ganho de compreensão.
-   Elementos gráficos devem ter propósito.

## 15. Imagens

Imagens devem acrescentar história, contexto ou emoção. Fotografias
podem aproximar o visitante do Mário quando fizer sentido. Nada deve ser
usado apenas para preencher espaço.

## 16. Movimento

Movimentos sutis, transições suaves e efeitos com função de orientar,
revelar ou enriquecer. Respeitar redução de movimento, leitura e
desempenho.

## 17. Multimídia

Áudio, vídeo e narração são complementares, opcionais e controláveis.
Sem reprodução automática invasiva. Voz do Mário e voz da Athena são
possibilidades futuras.

> Multimídia complementa a leitura; não a substitui.

## 18. Navegação

Discreta, compreensível, com poucos caminhos principais, localização
clara, retorno fácil e adaptação ao toque.

> Liberdade para explorar, sem deixar o visitante perdido.

## 19. Acessibilidade

Contraste adequado; texto legível; foco de teclado visível; descrição de
imagens quando necessário; áreas de toque adequadas; redução de
movimento; informação não dependente apenas de cor.

## 20. Identidade de marca

A logo deve preservar forma, proporções e espaço de respiro. O nome
Mário Holanda deve ter presença clara sem transformar a experiência em
autopromoção.

**Athena** poderá possuir identidade própria, integrada ao universo
visual do projeto, sem competir com Mário Holanda.

## 21. Conceitos preservados

-   **Além do Código**
-   **Construindo Caminhos**

Poderão futuramente nomear capítulos, seções ou temas.

## 22. Referência visual

A **V3 visual** é a referência consolidada para a implementação: paleta,
tipografia, espaçamento, componentes, estados, navegação,
responsividade, acessibilidade e atmosfera editorial.

## 23. Status

**Design System conceitual:** aprovado.\
**Paleta técnica:** aprovada.\
**Tipografia:** aprovada.\
**Escala tipográfica:** aprovada.\
**Espaçamento:** aprovado.\
**Grid e responsividade:** aprovados.\
**Componentes e estados:** aprovados.

**Próxima etapa:** revisão final do documento e preparação da
documentação que antecede a revisão do FSD/PSD.
