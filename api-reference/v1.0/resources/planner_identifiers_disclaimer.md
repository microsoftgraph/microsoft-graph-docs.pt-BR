# <a name="identifiers-in-planner"></a>Identificadores no Planner

Os identificadores de objetos no Planner são valores da cadeia de caracteres gerados pelo serviço. Observe que os valores têm 28 caracteres e diferenciam maiúsculas de minúsculas. Quando passado da forma como está, o serviço fará uma simples validação do formato do identificador, se a validação do formato falhar, os chamadores receberão uma resposta de erro Solicitação Incorreta (400) indicando esse problema. Receber esse erro indica um bug no aplicativo de chamada, como:

- O aplicativo de chamada processou o identificador como uma cadeia de caracteres que não diferencia maiúsculas de minúsculas. Os identificadores em Tarefas diferenciam maiúsculas de minúsculas.
- O aplicativo de chamada truncou o identificador. Os identificadores em Tarefas têm 28 caracteres.
- O aplicativo de chamada tentou gerar um valor do identificador para um objeto em Tarefas. Não são aceitos identificadores gerados por clientes. Todos os identificadores são gerados pelo serviço durante a criação de objetos.

A validação **não é um recurso de segurança**. Ela serve para informar os aplicativos sobre problemas comuns relacionados aos identificadores durante o desenvolvimento do aplicativo que, caso contrário, seriam difíceis de identificar.