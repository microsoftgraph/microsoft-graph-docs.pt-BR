---
title: Visão geral dos grupos do Microsoft 365 no Microsoft Graph
description: 'Os grupos do Microsoft 365 fornecem o serviço de associação de base para os usuários compartilharem conversas, arquivos, anotações, calendários, planos e muitos outros ativos. '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.custom: scenarios:getting-started
ms.openlocfilehash: 0ea28b5f4ff69faba5146ebc790703e423d9e8ba
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896109"
---
# <a name="overview-of-microsoft-365-groups-in-microsoft-graph"></a>Visão geral dos grupos do Microsoft 365 no Microsoft Graph

Os grupos do Microsoft 365 fornecem o serviço de associação de base para os usuários compartilharem conversas, arquivos, anotações, calendários, planos e muitos outros ativos. 


> [!VIDEO https://www.youtube-nocookie.com/embed/WB9w6QM9xIU]

## <a name="why-integrate-with-microsoft-365-groups"></a>Por que se integrar aos grupos do Microsoft 365?   

Os grupos formam a base que permite a colaboração e a integração de usuários em diversos serviços para oferecer suporte a cenários avançados no planejamento de tarefas, trabalho em equipe, treinamentos, etc. Quando você se integra com os grupos do Microsoft 365, seu aplicativo pode dar suporte a milhões de usuários à medida que eles fazem a transição entre várias experiências no Microsoft 365 Suite e além disso.  
 
### <a name="create-groups-to-facilitate-teamwork-across-services"></a>Criar grupos para facilitar o trabalho em equipe em todos os serviços 
 
Você pode usar a API do Microsoft Graph para criar, gerenciar ou excluir grupos em todo o ciclo de vida de colaboração. Por exemplo, é possível fazer o seguinte:  
 
- Usar a API [Criar grupo](/graph/api/group-post-groups?view=graph-rest-1.0) para provisionar um novo grupo. Em seguida, o grupo é disponibilizado em diversos aplicativos, como Outlook, SharePoint, Microsoft Teams, Planner e até mesmo no Microsoft Stream. O Microsoft Graph é sincronizado nesses serviços conectados para fornecer acesso perfeito a todos os membros do grupo.  
 
    **Todos os grupos do Microsoft 365 são integrados a um conjunto padrão de serviços do Microsoft 365**

    ![Diagrama mostrando a integração de grupo do Microsoft 365 com arquivos, observações, tarefas, sites, conversas e calendário](images/office365-groups-concept-overview-related-services-infographic.png)  

- Permite que os membros indiquem que um grupo é um dos seus [favoritos](/graph/api/group-addfavorite?view=graph-rest-1.0) ou que [o removam dos favoritos](/graph/api/group-removefavorite?view=graph-rest-1.0), caso queiram. 
- [Criar](/graph/api/group-post-conversations?view=graph-rest-1.0), [obter](/graph/api/group-get-conversation?view=graph-rest-1.0) ou [excluir](/graph/api/group-delete-conversation?view=graph-rest-1.0) conversas em grupo do seu aplicativo personalizado. 
- Programe [eventos](/graph/api/resources/event?view=graph-rest-1.0) de calendário no calendário do grupo. 
- Obtenha informações sobre [o site do SharePoint](/graph/api/resources/site?view=graph-rest-1.0) que está associado a um grupo, como as [listas](/graph/api/list-list?view=graph-rest-1.0) ou [subsites](/graph/api/site-list-subsites?view=graph-rest-1.0) da biblioteca de documentos. 
- [Criar um plano](/graph/api/planner-post-buckets?view=graph-rest-1.0) no Planner pertencente a um grupo. O plano oferece uma maneira visual de acompanhar o trabalho em equipe, permitindo que você [crie tarefas](/graph/api/planner-post-tasks?view=graph-rest-1.0) que possam ser [organizadas em buckets](/graph/api/planner-post-buckets?view=graph-rest-1.0). 
- Acesse o bloco de anotações do [OneNote](/graph/api/resources/onenote?view=graph-rest-1.0) associado a um grupo, que pode ser usado para a coleta de anotações da reunião e para a organização das ideias. 
  
    **Microsoft 365 grupos e conversas no Outlook na Web**

    ![Captura de tela do Outlook na Web com os grupos listados na pasta Grupos](images/office365-groups-concept-overview-groups-in-outlook.png) 

- [Habilite um grupo do Microsoft Teams](/graph/api/team-put-teams?view=graph-rest-beta) (visualização) para permitir que os membros do grupo se envolvam em chat persistente.  
- [Excluir grupos](/graph/api/group-delete?view=graph-rest-1.0). Quando um grupo é excluído, todo o conteúdo associado também o é, evitando sites, conversas ou planos órfãos. 
 
### <a name="manage-group-membership-seamlessly"></a>Gerenciar facilmente a associação a um grupo 
 
Os grupos do Microsoft 365 são conjuntos de usuários que compartilham o acesso a recursos nos serviços Microsoft ou em seu aplicativo. Como os membros do grupo são gerenciados centralmente, qualquer alteração feita na associação afetará todos os serviços associados ao grupo. Você pode usar o Microsoft Graph para executar as seguintes tarefas de associação a grupos:
 
- [Adicione](/graph/api/group-post-members?view=graph-rest-1.0) e [remova](/graph/api/group-delete-members?view=graph-rest-1.0) membros de um grupo existente. 
- Obtenha uma [lista de proprietários](/graph/api/group-list-owners?view=graph-rest-1.0) ou uma [lista de membros](/graph/api/group-list-members?view=graph-rest-1.0) para um grupo. Isso ajuda a comunicar quem tem acesso ao conteúdo do grupo ou quem pode precisar realizar tarefas administrativas, como a renovação do grupo ou a aprovação de uma solicitação de ingresso. 
- Designe os grupos como **Públicos**, tornando o conteúdo do grupo visível para qualquer pessoa na mesma organização ou **Particular**, tornando o conteúdo do grupo visível somente para os membros, por meio da operação [grupo de atualização](/graph/api/group-update?view=graph-rest-1.0). 
- [Remova os proprietários](/graph/api/group-delete-owners?view=graph-rest-1.0) que não tiverem mais responsabilidades em um grupo específico a partir da lista de proprietários do grupo. 
 
### <a name="establish-and-maintain-group-policy-settings"></a>Definir e manter as configurações de política de grupo 
 
À medida que o número de grupos criados em uma organização começa a crescer, o Microsoft Graph oferece suporte ao controle do uso e do ciclo de vida do grupo. Você pode aplicar políticas de grupo a todos os grupos de uma organização. Você pode usar a API do Microsoft Graph para:

- Configure uma ampla variedade de [configurações de política de grupo](/graph/api/resources/groupsetting?view=graph-rest-1.0) que ajudam a definir comportamentos, como excluir automaticamente os grupos, a menos que sejam renovados por um proprietário e impondo políticas de nomenclatura nos grupos do Microsoft 365. 
- [Renovar](/graph/api/group-renew?view=graph-rest-1.0) os grupos que estão prestes a expirar para permitir que os membros da equipe continuem com a colaboração e o acesso ao conteúdo. Se o grupo não for renovado de acordo com a política de validade estabelecida, o grupo é excluído automaticamente. 
- [Restaurar](/graph/api/directory-deleteditems-restore?view=graph-rest-1.0) os grupos excluídos.

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

- [API de Grupos no Microsoft Graph v1.0](/graph/api/resources/groups-overview?view=graph-rest-1.0)
- [API de Grupos no Microsoft Graph beta](/graph/api/resources/groups-overview?view=graph-rest-beta)


## <a name="next-steps"></a>Próximas etapas

- Experimente alguns exemplos de solicitações de API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer). 
- Saiba mais sobre como [usar a API de grupos](/graph/api/resources/groups-overview?view=graph-rest-1.0) no Microsoft Graph.
