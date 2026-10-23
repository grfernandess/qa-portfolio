# O dia a dia de um QA Júnior

> Rotina típica de um QA Júnior em um time ágil. Não é um diário pessoal.

## Exemplo de preenchimento

### Registrar um bug
- O que faz: abre o defeito com título claro, passos para reproduzir, resultado esperado, resultado obtido e evidência (print, log ou vídeo).
- Por que importa: sem reprodutibilidade, o desenvolvedor não consegue corrigir e o defeito volta.
- Exemplo: "Ao salvar o cadastro sem e-mail, o sistema mostra 'sucesso' em vez de 'campo obrigatório'."

## 1. Participar da daily
- O que faz: Conversar com o time para analisar, verificar e, se possível, alinhar problemas e erros encontrados.
- Por que importa: Alinhar como estão os testes, apontar problemas e combinar com os desenvolvedores a correção, caso não seja urgente.
- Exemplo: "Encontrei um BUG no sistema; analisando, foi na linha X do código. Preciso que o desenvolvedor valide e corrija para testarmos novamente."

## 2. Analisar histórias e critérios de aceite
- O que faz: Ler a história e os critérios de aceite antes do desenvolvimento, apontando ambiguidades, dependências e casos de teste que precisam existir.
- Por que importa: Para encontrar problemas, erros ou falhas antes do desenvolvimento e ter um documento para cobrar o que foi combinado.
- Exemplo: "Precisamos que o aplicativo valide cadastros únicos com esse tipo de identificador; atualmente não encontrei esse critério que combinamos anteriormente."

## 3. Planejar os testes (casos, prioridade e risco)
- O que faz: Planejar o que e como será testado o software/aplicação.
- Por que importa: Mapear e encontrar erros antes de causar danos ao projeto.
- Exemplo: "Hoje planejei testar esse caso na aplicação, prioridade média — não subiu em produção, está na branch — e o risco é mediano: pode impedir o usuário de cadastrar mais um endereço."

## 4. Preparar ambiente e dados de teste
- O que faz: Abrir os aplicativos que serão utilizados no teste e buscar os dados em um commit/branch, como também em algum ticket do Jira, para começar os testes.
- Por que importa: Uma boa preparação sempre terá um bom resultado; com os dados em dia, os testes poderão começar e finalizar rápido e com qualidade.
- Exemplo: "Hoje vou testar manualmente o checkout do carrinho, aplicar condições, produtos e cupons para avaliar o comportamento; utilizarei o DevTools para isso."

## 5. Executar testes manuais e exploratórios
- O que faz: Testar manualmente a aplicação, desenvolvimento, site etc., avaliando cenários no front-end como se fosse um usuário.
- Por que importa: Encontrar problemas no front-end que podem afetar a experiência do usuário.
- Exemplo: "Hoje vou testar o formulário de login no site, preenchendo com informações inválidas ou inexistentes, para avaliar o comportamento."

## 6. Registrar e acompanhar bugs
- O que faz: Após executar os testes, registrar qualquer defeito, problema ou bug encontrado e acompanhar as correções de bugs pendentes.
- Por que importa: Ter uma relação de todos os bugs que foram registrados e como está o andamento.
- Exemplo: "Encontrei um problema no formulário de login, registrei no Jira e estou acompanhando o andamento."

## 7. Validar correções e fazer regressão
- O que faz: Verificar se as correções foram aplicadas e se não existe mais nenhum novo problema.
- Por que importa: Verificar se o bug foi corrigido e se aquela mesma situação não ocorre mais.
- Exemplo: "O checkout do carrinho estava com problema ao aplicar o cupom 'XPTO'; verifiquei que agora está aplicando o cupom corretamente."

## 8. Atualizar casos de teste e documentação
- O que faz: Atualizar se o que foi mapeado foi corrigido ou se ainda se mantém com o mesmo ou um novo bug.
- Por que importa: Para manter o histórico atualizado, evitando cair no esquecimento.
- Exemplo: "Atualizei a documentação do ticket 123134; o teste foi um sucesso e o problema não ocorre mais."

## 9. Acompanhar métricas e status de qualidade
- O que faz: Verificar se o produto/aplicação está funcionando corretamente e acompanhar números como bugs abertos, bugs fechados e status dos testes.
- Por que importa: Para manter um padrão de como está a qualidade do software, tanto para o cliente como para a empresa.
- Exemplo: "Arrumamos 10 bugs dos 12 apontados."

## 10. Comunicar riscos e fechar o dia
- O que faz: Comunicar caso exista algum bug crítico ou arriscado para o sistema antes de finalizar o dia.
- Por que importa: Deixar alinhados todos os problemas atuais e o que pode acontecer.
- Exemplo: "Antes de encerrar, avisei no canal do time que o checkout tinha um bug crítico em produção e que o deploy de amanhã dependia da correção."

## Dúvidas que ficaram

1. O que é teste de regressão e quando ele é necessário?
2. Como comunicar riscos ao time sem parecer alarmista?
3. Como priorizar os testes quando o tempo é curto?
