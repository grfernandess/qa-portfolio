# SDLC (Software Development Life Cycle — Ciclo de Vida de Desenvolvimento de Software) e o papel do QA

## 1. Requisitos
- O que acontece:
É a fase em que se define o que o software deve fazer. Levantam-se requisitos funcionais (o que o sistema faz) e não funcionais (desempenho, segurança, usabilidade, compatibilidade), user stories, regras de negócio e critérios de aceitação.

- O que o QA faz:
Revisa os requisitos quanto à clareza, completude e testabilidade (evitando que uma ambiguidade vire um defeito grande/custoso no final).
Participa do refinamento de backlog / grooming com PO e desenvolvedores (alinhando a expectativa antes do desenvolvimento).
Ajuda a escrever critérios de aceitação.
Identifica conflitos, duplicidades ou regras de negócio faltantes (prevenindo retrabalhos).
Levanta requisitos não funcionais (garantindo que a qualidade não seja tratada apenas como "funciona/não funciona").

## 2. Design
- O que acontece:
É a fase de planejar como o software será construído: diagrama de classes, modelo de dados, fluxos de integração, wireframes, protótipos, escolha de tecnologias, desenho de APIs e componentes de segurança.

- O que o QA faz:
Revisa o design técnico para identificar pontos de risco e complexidade de teste (evitando arquitetura difícil de testar ou automação inviável).
Define a estratégia de testes (distribuindo o esforço de teste de forma eficiente na pirâmide de testes).
Planeja necessidades de ambiente de teste, dados de teste, mocks e stubs (garantindo que haverá onde e como validar as integrações).
Valida se o design contempla requisitos de segurança, desempenho e acessibilidade (evitando que falhas de segurança cheguem ao código).

## 3. Desenvolvimento
- O que acontece:
É a escrita efetiva do código, construção das funcionalidades e integração dos módulos.

- O que o QA faz:
Acompanha o desenvolvimento e faz testes exploratórios em funcionalidades já prontas (encontrando defeitos cedo, antes de acumular dívida técnica).
Revisa o pull request com foco em testabilidade (código difícil de testar gera defeitos escondidos).
Cria e mantém testes automatizados em paralelo com o dev.
Valida a Definition of Done (DoD): código revisado, testes passando, documentação atualizada.
Configura e mantém ambientes de homologação (QA/UAT).

## 4. Testes
- O que acontece: É a fase tradicional de executar testes para encontrar defeitos, validar funcionalidades e garantir que o software atende aos requisitos antes do release.

- O que o QA faz:
Executa casos de teste (manuais e automatizados): funcionais, negativos, de borda.
Executa testes não funcionais: desempenho, segurança, usabilidade, compatibilidade.
Executa testes de regressão após cada correção.
Reporta, rastreia e valida defeitos (bug life cycle).
Apoia o UAT (Teste de Aceitação do Usuário).
Assina o sign-off de qualidade (decisão baseada em métricas, não em achismo).

## 5. Deploy
- O que acontece:
É colocar o software em produção (ou em ambiente de pré-produção/homologação final), incluindo configuração de infraestrutura, variáveis de ambiente, migrações de banco e possíveis rollbacks.

- O que o QA faz:
Valida o build de release (versão correta, versão do banco, dependências).
Executa smoke tests ou sanity tests em homologação e, se possível, em produção (confirmando que as funções críticas continuam funcionando após o deploy).
Testa scripts de deploy e de rollback.
Verifica configurações (variáveis de ambiente, conexões de banco, serviços externos).
Monitora os primeiros minutos após o deploy em produção (shift-right).

## 6. Manutenção
- O que acontece:
É o período pós-produção: correção de defeitos que escaparam (hotfixes), aplicação de patches, melhorias contínuas, suporte a usuários e adaptação a mudanças de ambiente (ex.: nova versão do navegador, lei nova).

- O que o QA faz:
Valida correções de bugs em produção (hotfixes) antes ou após o deploy.
Executa testes de regressão em funcionalidades afetadas pela manutenção.
Coleta feedback do suporte e de usuários para transformar em novos requisitos ou defeitos.
Participa de pós-mortem de incidentes.
Atualiza casos de teste e automação com base nas mudanças.
