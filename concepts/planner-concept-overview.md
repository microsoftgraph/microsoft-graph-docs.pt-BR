---
title: Visão geral da API de tarefas e planos do Planner
description: O Planner oferece uma maneira simples e visual para as equipes organizarem o trabalho. Os clientes podem usar o Planner para criar planos, organizar e atribuir tarefas, compartilhar o progresso e colaborar em conteúdo.  O Planner fornece várias experiências interativas, incluindo um quadro de tarefas, uma página de gráficos e uma visualização de horários, assim como integrações em todo o Microsoft 365.
author: TarkanSevilmis
ms.localizationpriority: high
ms.prod: planner
ms.openlocfilehash: fe8102634efa3fd4bd2f561e4ec0858564ca7f21
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089288"
---
# <a name="planner-tasks-and-plans-api-overview"></a>Visão geral da API de tarefas e planos do Planner
O Planner oferece uma maneira simples e visual para as equipes organizarem o trabalho. Os clientes podem usar o Planner para criar planos, organizar e atribuir tarefas, compartilhar o progresso e colaborar em conteúdo.  O Planner fornece várias experiências interativas, incluindo um quadro de tarefas, uma página de gráficos e uma visualização de horários, assim como integrações em todo o Microsoft 365.

**Quadro de tarefas do Microsoft 365 Planner**

![Instantâneo de um painel de tarefas do Microsoft 365 Planner](images/plannerboard.png "Imagem do painel do Planner")


## <a name="why-integrate-with-planner-tasks"></a>Por que se integrar com tarefas do Planner?
O Planner fornece recursos de acompanhamento de tarefas para experiências de colaboração no Microsoft 365. Se os seus cenários exigem o acompanhamento de tarefas e a organização do trabalho de uma equipe ou um grupo de usuários finais, o Planner é o serviço certo para você. A integração do Planner pode ajudá-lo a alcançar os milhões de usuários que colaboram no Microsoft 365. 

### <a name="organize-your-teams-work"></a>Organize o trabalho de sua equipe
O Planner oferece um espaço compartilhado onde você pode criar uma equipe, [criar tarefas](/graph/api/planner-post-tasks?view=graph-rest-1.0) e atribuí-las aos outros membros da equipe. O Planner torna fácil para todos saber quem está fazendo o quê e se as coisas estão no prazo. Você pode atualizar tarefas com mais informações, como datas de vencimento, andamento e descrições, e então organizar mais tarefas com rótulos de categoria e buckets personalizáveis.   

### <a name="collaborate-across-microsoft-365"></a>Colabore no Microsoft 365
O Planner se integra às experiências de colaboração do Microsoft 365. Além dos clientes Web e móveis do Planner, os usuários podem visualizar e atualizar os planos e tarefas do Planner no SharePoint e do Microsoft Teams.  

O próprio Planner também é baseado no Microsoft Graph e no serviço de grupo do Microsoft 365. Os arquivos que você carrega e anexa às tarefas do Planner são armazenados no SharePoint. Os comentários do Planner são baseados em conversas em grupo do Outlook.

<!-- Add image
Note: Put an image here showing the relationship between Planner and other things
-->

### <a name="automate-the-creation-of-plans-and-tasks"></a>Automatizar a criação de tarefas e planos
Você está trabalhando em um processo ou tipo de projeto repetido? Você pode usar a API do Planner para automatizar a criação de um plano e uma lista de tarefas.  
 
## <a name="top-planner-api-tasks"></a>Principais tarefas da API do Planner

|Operação|URL|
|:--------|:--|
|Ver todos os [planos](/graph/api/resources/plannerplan?view=graph-rest-beta) para um grupo|GET [https://graph.microsoft.com/v1.0/groups/{id}/planner/plans](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|Ver [tarefas](/graph/api/resources/plannertask?view=graph-rest-beta) em um plano|GET [https://graph.microsoft.com/v1.0/planner/plans/{id}/tasks](https://developer.microsoft.com/graph/graph-explorer?request=planner/plans/{id}/tasks&version=v1.0)|
|Ver todas as [minhas tarefas](/graph/api/planneruser-list-tasks?view=graph-rest-beta) atribuídas a mim nos planos|GET [https://graph.microsoft.com/v1.0/me/planner/tasks/](https://developer.microsoft.com/graph/graph-explorer?request=me/planner/tasks/&version=v1.0)|
|[Criar uma nova tarefa](/graph/api/planner-post-tasks?view=graph-rest-1.0)|POST [https://graph.microsoft.com/v1.0/planner/tasks](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|[Atualizar uma tarefa](/graph/api/plannertask-update?view=graph-rest-1.0)|PATCH [https://graph.microsoft.com/v1.0/planner/tasks/{task-id}](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|[Excluir uma tarefa](/graph/api/plannertask-delete?view=graph-rest-1.0)|EXCLUIR [https://graph.microsoft.com/v1.0/planner/tasks/{id}](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

- [API do Planner no Microsoft Graph v1.0](/graph/api/resources/planner-overview?view=graph-rest-1.0)
- [API do Planner no Microsoft Graph beta](/graph/api/resources/planner-overview?view=graph-rest-beta)


## <a name="next-steps"></a>Próximas etapas

- [Usar a API do Planner](/graph/api/resources/planner-overview?view=graph-rest-1.0)
- [Trabalhar com planos](/graph/api/resources/planner-overview?view=graph-rest-1.0#plans)
- [Trabalhar com tarefas](/graph/api/resources/planner-overview?view=graph-rest-1.0#tasks)
