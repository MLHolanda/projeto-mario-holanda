# Projeto Mário Holanda — DECISOES_TECNICAS.md

**Versão:** 1.0  
**Status:** Aprovado para validação do FSD  
**Método:** Jornada IA — Vibe Coding v1.5

> Este documento registra as decisões técnicas necessárias para orientar o FSD e, posteriormente, a IA codadora.

## 1. Stack principal

**Astro**

O MVP será construído com Astro como framework principal, considerando sua natureza predominantemente orientada a conteúdo, páginas estruturadas, multilíngue, desempenho e evolução gradual para interatividade.

HTML, CSS e JavaScript/TypeScript poderão ser utilizados nos pontos necessários.

## 2. Modelo do MVP

O MVP será predominantemente orientado a conteúdo, com:

- conteúdo estruturado;
- páginas e rotas claras;
- componentes reutilizáveis;
- HTML semântico;
- acessibilidade;
- desempenho;
- interatividade somente quando tiver propósito claro.

## 3. Conteúdo

Categorias principais:

- Histórias;
- Projetos;
- Aprendizados;
- Pensamentos e Reflexões.

O conteúdo deverá crescer continuamente sem exigir reconstrução da estrutura principal.

Certificados poderão representar marcos da trajetória e, quando houver valor narrativo, relacionar-se às histórias correspondentes.

## 4. Multilinguismo

Idiomas iniciais:

- Português;
- Inglês;
- Espanhol.

A arquitetura deverá permitir a organização, manutenção e futura expansão dos idiomas, preservando identidade, sentido e contexto.

## 5. Banco de dados

**Não será adotado banco de dados para o núcleo do MVP.**

O conteúdo predominantemente estático permanecerá versionado junto ao projeto enquanto isso atender aos requisitos.

Banco de dados somente será introduzido diante de necessidade concreta.

## 6. Backend e APIs

**Não haverá backend de aplicação no núcleo inicial do MVP.**

APIs, processamento no servidor ou outros serviços dinâmicos somente serão introduzidos quando houver necessidade funcional ou técnica claramente identificada.

## 7. Athena

Athena faz parte da evolução do projeto, mas **não determinará a arquitetura do MVP**.

A primeira versão deverá permitir evolução futura sem exigir imediatamente uma arquitetura própria de IA ou backend dedicado.

## 8. Blog

O Blog existente continuará independente.

O novo projeto poderá conectar-se a ele, mas não deverá absorvê-lo nem exigir sua reconstrução nesta etapa.

## 9. Multimídia

Imagens, áudio, vídeo, animações e outros recursos poderão ser usados quando contribuírem para a experiência.

Deverão respeitar acessibilidade, desempenho, preferências do visitante e limitações do dispositivo/navegador.

Áudio avançado, narração e voz não são obrigatórios na primeira versão.

## 10. Acessibilidade

A acessibilidade será tratada desde o início, priorizando:

- HTML semântico;
- teclado;
- foco;
- textos alternativos;
- hierarquia de títulos;
- contraste;
- formulários acessíveis;
- preferências do visitante.

## 11. Desempenho

Desempenho é requisito desde o início.

Imagens, animações, áudio, vídeo e recursos interativos deverão ser otimizados. Recursos visuais não deverão ser adicionados apenas por estética quando prejudicarem significativamente a experiência.

## 12. SEO e compartilhamento

Conteúdos relevantes deverão possuir estrutura adequada para acesso direto, compartilhamento e mecanismos de busca, considerando título, descrição, URL, idioma e metadados quando aplicáveis.

## 13. Privacidade, segurança e legislação

O projeto deverá respeitar privacidade, segurança e legislação aplicável.

Não serão coletados dados pessoais sem necessidade definida. Recursos de contato e interação deverão ser analisados também sob os aspectos legais antes da implementação.

## 14. Monitoramento

O MVP deverá possuir monitoramento compatível com seu escopo.

Recursos gratuitos serão priorizados quando forem tecnicamente adequados. Quando o recurso ideal não estiver disponível gratuitamente, a experiência poderá ser adaptada preservando sua intenção.

## 15. Hospedagem

A arquitetura deverá priorizar publicação simples e compatível com o modelo predominantemente estático do MVP.

O provedor definitivo poderá ser definido na configuração do ambiente de publicação.

## 16. Versionamento

**Git + GitHub**

Deverão ser preservados histórico, documentação, commits compreensíveis e possibilidade de retorno a versões anteriores. Segredos não deverão ser versionados.

## 17. Ambiente de desenvolvimento

Serão utilizadas somente as ferramentas necessárias ao desenvolvimento definido no FSD.

Não deverão ser instaladas bibliotecas, frameworks, serviços ou ferramentas adicionais sem necessidade ou decisão explícita.

## 18. IA codadora

A IA codadora será executora técnica dentro das decisões tomadas anteriormente.

Suas referências principais serão:

1. PRD.md;
2. DESIGN.md;
3. DECISOES_TECNICAS.md;
4. FSD.md;
5. demais arquivos oficiais quando necessários.

A IA não deverá inventar requisitos, arquitetura, regras de negócio, bibliotecas ou serviços fora do definido.

Quando faltar uma decisão técnica relevante, deverá solicitar orientação antes de implementar.

O desenvolvimento ocorrerá por etapas, permitindo revisão humana.

## 19. Recursos gratuitos e aprendizado

Recursos gratuitos serão priorizados quando adequados.

As ferramentas também serão instrumentos de aprendizado, habilidades, autonomia, raciocínio e inteligência.

Se o recurso ideal não estiver disponível gratuitamente, a experiência poderá ser adaptada preservando sua intenção.

## 20. Regra de evolução

Nenhuma decisão técnica é permanente por si só.

Novas necessidades deverão ser analisadas antes de alterar a arquitetura.

> **Nenhuma decisão deste documento é uma lei intocável.**

## 21. Resumo

| Área | Decisão |
|---|---|
| Framework principal | Astro |
| Modelo | Predominantemente orientado a conteúdo |
| Conteúdo | Estruturado e versionado |
| Idiomas | Português, Inglês e Espanhol |
| Banco de dados | Não necessário no núcleo do MVP |
| Backend | Não necessário no núcleo do MVP |
| Athena | Evolução futura; não condiciona o MVP |
| Blog | Independente |
| Acessibilidade | Desde o início |
| Desempenho | Desde o início |
| SEO | Incluído |
| Privacidade/segurança | Incluídas |
| Monitoramento | Conforme escopo |
| Hospedagem | Publicação simples |
| Versionamento | Git + GitHub |
| IA codadora | Segue documentação e não improvisa |
| Recursos gratuitos | Priorizados quando adequados |

## 22. Relação com o FSD

Este documento será fonte técnica para criação e validação do FSD.

O FSD deverá refletir estas decisões. Alterações deverão ser analisadas e registradas antes de serem incorporadas.

## 23. Evolução do documento

Este documento poderá evoluir quando novas necessidades forem identificadas, preservando a coerência entre PRD, DESIGN.md, DECISOES_TECNICAS.md e FSD.md.
