# <a name="planner-tasks-and-plans-api-overview"></a>Visão geral da API de tarefas e planos do Planner
O Planner oferece uma maneira simples e visual para as equipes organizarem o trabalho. Os clientes podem usar o Planner para criar planos, organizar e atribuir tarefas, compartilhar o progresso e colaborar em conteúdo.  O Planner oferece várias experiências interativas, incluindo um quadro de tarefas, uma página de gráficos e um modo de exibição de agenda, bem como integrações em todo o Office 365.

**Quadro de tarefas do Office 365 Planner**

![Captura de tela de um quadro de tarefas do Office 365 Planner](images/plannerboard.png "Imagem do quadro do Planner")


## <a name="why-integrate-with-planner-tasks"></a>Por que se integrar com tarefas do Planner?
O Planner oferece funcionalidades de acompanhamento de tarefa para experiências de colaboração no Office 365. Se os seus cenários exigem o acompanhamento de tarefas e a organização do trabalho de uma equipe ou um grupo de usuários finais, o Planner é o serviço certo para você. A integração com o Planner pode ajudá-lo a alcançar milhões de usuários colaborando no Office 365. 

### <a name="organize-your-teams-work"></a>Organize o trabalho de sua equipe
O Planner oferece um espaço compartilhado onde você pode criar uma equipe, [criar tarefas](../api-reference/v1.0/api/planner_post_tasks.md) e atribuí-las aos outros membros da equipe. O Planner torna fácil para todos saber quem está fazendo o quê e se as coisas estão no prazo. Você pode atualizar tarefas com mais informações, como datas de vencimento, andamento e descrições, e então organizar mais tarefas com rótulos de categoria e buckets personalizáveis.   

### <a name="collaborate-across-office-365"></a>Colaborar no Office 365
O Planner integra as experiências de colaboração no Office 365. Além de clientes móveis e da Web do Planner, os usuários podem exibir e atualizar o planos e tarefas do Planner por meio do SharePoint e no Microsoft Teams.  

O próprio Planner também funciona com o Microsoft Graph e o serviço de grupo do Office 365. Os arquivos que você carrega e anexa às tarefas do Planner são armazenados no SharePoint. Os comentários do Planner são baseados em conversas em grupo do Outlook.

<!-- Add image
Note: Put an image here showing the relationship between Planner and other things
-->

### <a name="automate-the-creation-of-plans-and-tasks"></a>Automatizar a criação de tarefas e planos
Você está trabalhando em um processo ou tipo de projeto repetido? Você pode usar a API do Planner para automatizar a criação de um plano e uma lista de tarefas.  
 
## <a name="top-planner-api-tasks"></a>Principais tarefas da API do Planner

|Operação|URL|
|:--------|:--|
|Ver todos os [planos](../api-reference/beta/resources/plannerplan.md) para um grupo|GET [https://graph.microsoft.com/v1.0/groups/{id}/planner/plans](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|Ver [tarefas](../api-reference/beta/resources/plannertask.md) em um plano|GET [https://graph.microsoft.com/v1.0/planner/plans/{id}/tasks](https://developer.microsoft.com/en-us/graph/graph-explorer?request=planner/plans/{id}/tasks&version=v1.0)|
|Ver todas as [minhas tarefas](../api-reference/beta/api/planneruser_list_tasks.md) atribuídas a mim nos planos|GET [https://graph.microsoft.com/v1.0/me/planner/tasks/](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/planner/tasks/&version=v1.0)|
|[Criar uma nova tarefa](../api-reference/v1.0/api/planner_post_tasks.md)|POST [https://graph.microsoft.com/v1.0/planner/tasks](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|[Atualizar uma tarefa](../api-reference/v1.0/api/plannertask_update.md)|PATCH [https://graph.microsoft.com/v1.0/planner/tasks/{task-id}](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|[Excluir uma tarefa](../api-reference/v1.0/api/plannertask_delete.md)|DELETE [https://graph.microsoft.com/v1.0/planner/tasks/<id>](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|


## <a name="next-steps"></a>Próximas etapas

- [Usar a API do Planner](../api-reference/v1.0/resources/planner_overview.md)
- [Trabalhar com planos](../api-reference/v1.0/resources/planner_overview.md#plans)
- [Trabalhar com tarefas](../api-reference/v1.0/resources/planner_overview.md#tasks)
