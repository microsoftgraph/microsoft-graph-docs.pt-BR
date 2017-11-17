# <a name="planner"></a>Planner
A API do Office 365 Planner permite que você crie e atribua tarefas aos usuários em um grupo no Office 365.

Antes de começar a experimentar a API do Planner, vale a pena entender como os principais objetos na API do Planner se relacionam entre si e também com os grupos do Office 365.

## <a name="groups"></a>Grupos
Os grupos do Office 365 são os proprietários dos planos da API do Planner. Para [obter os planos pertencentes a um grupo](../api/plannergroup_list_plans.md), faça a solicitação HTTP abaixo.

```http
GET /groups/{id}/planner/plans
```

Ao [criar um novo plano](../api/planner_post_plans.md), torne o grupo o proprietário do plano. Para isso, basta definir a propriedade `owner` em um objeto de plano. Os planos devem pertencer a grupos.

>**Observação:** O usuário que está criando o plano deve ser um membro do grupo. Ao criar um novo grupo usando a API, você não é automaticamente adicionado ao grupo como membro. Isso precisa ser feito usando uma chamada de API separada.

## <a name="plans"></a>Planos
Os [planos](plannerplan.md) são os contêineres das [tarefas](plannertask.md). Para [criar uma tarefa em um plano](../api/planner_post_tasks.md), defina a propriedade `planId` no objeto da tarefa como a ID do plano ao criar a tarefa. No momento, as tarefas não podem ser criadas sem planos. Para [recuperar as tarefas em um plano de](../api/plannerplan_list_tasks.md), faça a solicitação HTTP abaixo.

```http
GET /planner/plans/{id}/tasks
```

## <a name="tasks"></a>Tarefas
Cada tarefa pode ser atribuída a um usuário ao adicionar uma [atribuição](plannerassignment.md) à propriedade [assignments](plannerassignments.md) no objeto task. A ID do usuário ao qual a tarefa será atribuída é o nome da propriedade open em `assignments`. Além disso, a propriedade `orderHint` na atribuição deve ser especificada.

## <a name="task-and-plan-details"></a>Detalhes de planos e tarefas 
Os recursos do Planner são organizados em objetos básicos e objetos detalhados. Os objetos básicos oferecem acesso às propriedades comuns dos recursos, adequadas para modos de exibição de lista. No entanto, os objetos detalhados fornecem acesso a grandes propriedades dos recursos, adequadas para modos de exibição de busca detalhada.

## <a name="visualization"></a>Visualização
Além do plano de dados e tarefas, a API do Planner também oferece recursos para disponibilizar uma visualização comum de dados nos clientes. Há vários tipos de visualização de dados disponíveis para as tarefas:

| As tarefas são exibidas como      | As tarefas são ordenadas com informações de|
|:------------------|:----------|
|Lista plana (tarefas em um plano)| Propriedade `orderHint` em tarefas|
|Lista plana (tarefas atribuídas a um usuário)| Propriedade `assigneePriority` em tarefas|
|Modo de exibição de quadro com colunas para os destinatários (atribuídos ao quadro de tarefas)| Objeto [assignedToTaskBoardTaskFormat](plannerassignedToTaskBoardTaskFormat.md)|
|O modo de exibição de quadro com colunas para o andamento da tarefa na direção de conclusão (quadro de tarefa de andamento)| Objeto [progressTaskBoardTaskFormat](plannerprogressTaskBoardTaskFormat.md)|
|Modo de exibição de quadro com colunas personalizadas de tarefas (quadro de tarefa do bucket):|Objeto [bucketTaskBoardTaskFormat](plannerbucketTaskBoardTaskFormat.md)|

As colunas personalizadas no quadro de tarefas do bucket são representadas pelos objetos [bucket](plannerbucket.md) e, sua ordem, pela propriedade `orderHint` no objeto.

Toda a ordem é controlada pelos princípios identificados em [Dicas de ordem do Planner](planner_order_hint_format.md).

## <a name="planner-resource-versioning"></a>Versão do recurso do Planner

O Planner cria versões com todos os recursos usando etags. Essas etags são retornadas com a propriedade `@odata.etag` em cada recurso e, as solicitações `PATCH` e `DELETE`, exigem a última etag conhecida pelo cliente a ser especificado pelo cabeçalho `If-Match`. O Planner permite alterações em versões mais antigas de recursos, se a alteração pretendida não estiver em conflito com as alterações mais recentes aceitas pelo serviço do Planner no mesmo recurso. Os clientes podem identificar qual etag para o mesmo recurso é mais recente ao calcular qual valor de etag é maior em comparação com a cadeia de caracteres ordinal. Cada recurso tem uma etag separada. Não há comparações entre os valores de etags de recursos diferentes, incluindo aqueles com relações de confinamento. Espera-se que os aplicativos cliente tratem dos dois controles de versão relacionados aos códigos de status de erro 409 e 412 ao ler a versão mais recente do item e resolver as alterações conflitantes.

## <a name="common-planner-error-conditions"></a>Condições de erro comuns do Planner

Além dos [erros gerais](../../../concepts/errors.md) que se aplicam ao Microsoft Graph, algumas condições de erro são específicas da API do Planner.

### <a name="400-bad-request"></a>400 Solicitação Incorreta

Há diversos casos comuns onde as solicitações `POST` e `PATCH` podem ter um código de status 400. Os problemas comuns incluem:
* As propriedades Open Type não têm os tipos corretos ou o tipo não foi especificado ou não contêm propriedades. Por exemplo, as propriedades [plannerAssignments](plannerAssignments.md) com valores complexos precisam declarar a propriedade `@odata.type` com valor `microsoft.graph.plannerAssignment`.
* Os valores da dica de ordem não têm o [formato correto](planner_order_hint_format.md). Por exemplo, um valor de dica de ordem está sendo definido diretamente como o valor retornado ao cliente.
* Os dados são logicamente inconsistentes. Por exemplo, a data de início da tarefa é posterior à data de conclusão da tarefa.

### <a name="403-forbidden"></a>403 Proibido

Além dos erros gerais, a API do Planner também retorna esse código de status quando um limite definido pelo serviço é excedido. Se esse for o caso, a propriedade `code` no tipo de recurso do erro indicará o tipo do limite excedido pela solicitação. Os valores possíveis para os tipos de limite incluem:

| Valor  | Descrição|
|:------------------|:----------|
|MaximumProjectsOwnedByUser|Foi excedido o número máximo de Planos pertencentes ao limite do grupo. Esse limite se baseia na propriedade `owner` no recurso [plannerPlan](plannerPlan.md).|
|MaximumProjectsSharedWithUser|Foi excedido o número máximo de Planos compartilhados com um limite de usuário.  Esse limite se baseia na propriedade `sharedWith` no recurso [plannerPlanDetails](plannerPlanDetails.md).|
|MaximumTasksCreatedByUser|Foi excedido o número máximo de Tarefas criadas pelo limite do usuário. Esse limite se baseia na propriedade `createdBy` no recurso [plannerTask](plannerTask.md).|
|MaximumTasksAssignedToUser|Foi excedido o número máximo de Tarefas atribuídas ao limite do usuário. Esse limite se baseia na propriedade `assignments` no recurso [plannerTask](plannerTask.md).|
|MaximumTasksInProject|Foi excedido o número máximo de Tarefas no limite de um Plano. Esse limite se baseia na propriedade `planId` no recurso [plannerTask](plannerTask.md).|
|MaximumActiveTasksInProject|Foi excedido o número máximo de Tarefas que não foram concluídas no limite de um Plano. Esse limite se baseia nas propriedades `planId` e `percentComplete` no recurso [plannerTask](plannerTask.md).|
|MaximumBucketsInProject|Foi excedido o número máximo de Buckets no limite de um Plano. Esse limite se baseia na propriedade `planId` no recurso [plannerBucket](plannerBucket.md).|
|MaximumUsersSharedWithProject|A propriedade `sharedWith` no recurso [plannerPlanDetails](plannerPlanDetails.md) contém muitos valores.|
|MaximumReferencesOnTask|A propriedade `references` no recurso [plannerTaskDetails](plannerTaskDetails.md) contém muitos valores.|
|MaximumChecklistItemsOnTask|A propriedade `checklist` no recurso [plannerTaskDetails](plannerTaskDetails.md) contém muitos valores.|
|MaximumAssigneesInTasks|A propriedade `assignments` no recurso [plannerTask](plannerTask.md) contém muitos valores.|

### <a name="412-precondition-failed"></a>412 Falha na Pré-condição 

Todas as solicitações `POST`, `PATCH` e `DELETE` na API do Planner exigem que o cabeçalho `If-Match` seja especificado com o último valor da etag visto do recurso que está sujeito à solicitação. Além disso, o código de status 412 pode ser retornado se o valor da etag especificado na solicitação já não corresponder a uma versão do recurso no serviço. Nesse caso, os clientes devem ler o recurso novamente e obter uma nova etag.

