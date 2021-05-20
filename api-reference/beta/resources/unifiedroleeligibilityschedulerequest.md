---
title: Tipo de recurso unifiedRoleEligibilityScheduleRequest
description: Representa a solicitação de operações de atribuição de função qualificadas por meio do Azure AD Privileged Identity Management.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 622bce02829cc245d0cbdb859a6c56b1f88a3ea5
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547124"
---
# <a name="unifiedroleeligibilityschedulerequest-resource-type"></a>Tipo de recurso unifiedRoleEligibilityScheduleRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a solicitação de operações de atribuição de função qualificadas por meio do Azure AD Privileged Identity Management.

`unifiedRoleEligibilityScheduleRequest` é uma entidade modelada por tíquete usada para gerenciar o ciclo de vida das atribuições de função qualificadas no diretório. Ele representa a intenção/decisão dos usuários e administradores e também oferece a flexibilidade para habilitar a implementação de agendamento recorrente, portais de aprovação e assim por diante, em comparação com a exposição direta , e operações em e `POST` `PUT` `DELETE` `unifiedRoleEligibilitySchedule` `unifiedRoleEligibilityInstance` .

Os administradores podem usar para criar e/ou atualizar atribuições de função `unifiedRoleEligibilityScheduleRequest` qualificadas com ou sem hora de início e término. Embora administradores qualificados, podem usá-lo para criar uma solicitação para estender ou renovar suas atribuições qualificadas.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleEligibilityScheduleRequests](../api/unifiedroleeligibilityschedulerequest-list.md)|[Coleção unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Obter uma lista dos [objetos unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) e suas propriedades.|
|[Criar unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-post-unifiedroleeligibilityschedulerequests.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Crie um novo [objeto unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)|
|[Obter unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-get.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Leia as propriedades e as relações de [um objeto unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)|
|[Atualizar unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-update.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Atualize as propriedades de [um objeto unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedulerequest-filterbycurrentuser.md)|[Coleção unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Obter uma lista dos [objetos unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) e suas propriedades relacionadas a um usuário específico.|
|[cancel](../api/unifiedroleeligibilityschedulerequest-cancel.md)|Nenhum|Cancela um [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) imediatamente e marca-o para exclusão em 30 dias|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|String|Representando o tipo da operação na atribuição de função. O valor pode ser <ul><li>`AdminAdd`: Os administradores atribuem usuários/grupos a funções;</li><li>`UserAdd`: Os usuários ativam atribuições qualificadas;</li><li> `AdminUpdate`: Os administradores alteram as atribuições de função existentes</li><li>`AdminRemove`: Os administradores removem usuários/grupos de funções;<li>`UserRemove`: Os usuários desativam as atribuições ativas;<li>`UserExtend`: Os usuários solicitam estender suas atribuições de expiração;</li><li>`AdminExtend`: Os administradores estendem atribuições expiradas.</li><li>`UserRenew`: Os usuários solicitam a renovação de suas atribuições expiradas;</li><li>`AdminRenew`: Os administradores estendem atribuições expiradas.</li></ul>|
|appScopeId|String|ID do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use "/" para o escopo de todo o locatário. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.|
|directoryScopeId|String|ID do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.|
|id|String|O identificador exclusivo para unifiedRoleEligibilityScheduleRequest.|
|isValidationOnly|Booliano|Um booleano que determina se a chamada é uma validação ou uma chamada real. De definir essa propriedade somente se você quiser verificar se uma ativação está sujeita a regras adicionais, como MFA, antes de realmente enviar a solicitação.|
|justification|String|Uma mensagem fornecida por usuários e administradores ao criar a solicitação sobre por que ela é necessária.|
|principalId|String| Objectid da entidade à qual a atribuição está sendo concedida.|
|roleDefinitionId|String|ID do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O objeto schedule da solicitação de atribuição de função.|
|targetScheduleId|String|ID do objeto schedule anexado à atribuição.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|O objeto ticketInfo anexado à solicitação de atribuição de função que inclui detalhes do número do tíquete e do sistema de tíquetes.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência ao objeto de diretório que é o escopo da atribuição. Fornecido para que os chamadores possam obter o objeto de diretório `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura.|
|principal|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência à entidade que está recebendo uma atribuição de função por meio da solicitação. Fornecido para que os chamadores possam obter a entidade principal `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Propriedade indicando a funçãoDefinition para a qual a atribuição se destina. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função. roleDefinition.Id será expandido automaticamente|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```

