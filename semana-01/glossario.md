# Glossário de QA

## Qualidade de software
- Definição: É o grau em que o software atende aos requisitos e às expectativas do usuário, com níveis aceitáveis de defeitos.
- Exemplo: Entregar funcionalidade, confiabilidade, usabilidade e segurança ao cliente.

## QA
- Definição: É o conjunto de processos e práticas que previnem defeitos e criam condições para que a qualidade aconteça durante todo o ciclo. O profissional de QA atua nesses processos.
- Exemplo: Revisar critérios de aceite com o PO antes do desenvolvimento e acompanhar o processo de testes.

## QC
- Definição: É o controle de qualidade, com foco no produto! Nesse caso o profissional de QC detecta defeitos já existentes.
- Exemplo: Executar um caso de teste no build e comparar o resultado com o esperado.

## Teste
- Definição: É a atividade de verificação e validação que revela defeitos e fornece informação para decidir se o software está pronto. Pode ser manual ou automatizada; o teste não corrige, ele encontra e reporta.
- Exemplo: Testar o login com senha válida, inválida, vazia e usuário bloqueado.

## Defeito
- Definição: A imperfeição materializada no artefato. É o erro “escrito” no código, no requisito, no banco de dados ou na configuração.
- Exemplo: No documento de requisitos, falta a regra de que usuários inativos não podem acessar o painel.

## Erro
- Definição: Uma ação humana incorreta. É a causa raiz: alguém (analista, desenvolvedor, arquiteto, QA, PO) comete um engano ao produzir um artefato (requisito, código, configuração, documento).
- Exemplo: O analista escreve no requisito: “o campo CEP aceita até 8 dígitos”, esquecendo de dizer que deve ser apenas numérico.

## BUG
- Definição: É o termo coloquial mais usado para se referir a um defeito no código ou no programa em execução.
- Exemplo: Clicar no botão “Excluir” não remove o item da lista (bug no frontend). A API retorna status 200 OK mesmo quando não salva os dados (bug no backend).

## Falha
- Definição: É o defeito se manifestando durante a execução. O software não realiza a função exigida sob condições específicas. É o que o usuário ou o testador realmente vê e pode reproduzir.
- Exemplo: O usuário tenta finalizar a compra e recebe a mensagem “Erro inesperado. Tente novamente”. O relatório de vendas exibe valores negativos.

## Caso de teste
- Definição: Um documento ou item que descreve um cenário específico a ser executado para validar se o software se comporta como esperado. Ele define: o que testar, como testar e qual é o resultado esperado.
- Exemplo: “Login com senha válida deve redirecionar para a home.”

## Plano de teste
- Definição: Plano de teste é o documento estratégico que define como os testes serão realizados em um projeto, release ou sprint. É o guia da equipe de QA para garantir cobertura e organização.
- Exemplo: Plano da release 2.0: escopo, estratégia, responsáveis, cronograma e critérios de saída.

## Critério de aceite
- Definição: É a condição que precisa ser atendida para que uma história, funcionalidade ou entrega seja considerada aceita.
- Exemplo: “O usuário só acessa a home após login válido.”

## Teste funcional
- Definição: Verifica se o sistema faz o que foi especificado, com base nos requisitos funcionais.
- Exemplo: Validar se o cálculo do frete aplica a regra correta para cada CEP.

## Teste não funcional
- Definição: Verifica características de qualidade como desempenho, segurança, usabilidade, compatibilidade e acessibilidade.
- Exemplo: Medir o tempo de resposta da listagem com 10 mil registros.

## Teste de regressão
- Definição: É a reexecução de testes em funcionalidades que podem ter sido afetadas por uma mudança, para garantir que nada quebrou.
- Exemplo: Após corrigir o login, testar cadastro, recuperação de senha e logout.

## Smoke test
- Definição: É um teste rápido e superficial para confirmar que as funções críticas funcionam e que o build está apto para testes mais profundos.
- Exemplo: Após o deploy, abrir o sistema, fazer login e acessar a tela principal.
