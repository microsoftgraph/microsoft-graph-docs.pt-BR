---
title: Tipo de recurso unifiedRoleAssignmentScheduleRequest
description: Representa a solicitação de operações de atribuição de função ativa por meio do Azure AD Privileged Identity Management.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b8d07bf69d7b31ee5cdbb0f9aaa34be5a21e5bfb
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299071"
---
# <a name="unifiedroleassignmentschedulerequest-resource-type"></a>Tipo de recurso unifiedRoleAssignmentScheduleRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a solicitação de operações de atribuição de função ativa por meio do Azure AD Privileged Identity Management.

`unifiedRoleAssignmentScheduleRequest` é uma entidade modelo de tíquete usada para gerenciar o ciclo de vida das atribuições de função ativa no diretório. Ele representa a intenção/decisão dos usuários e administradores e também oferece a flexibilidade para habilitar a implementação de agendamento recorrente, portais de aprovação e assim por diante, em comparação com a exposição direta , e operações em e `POST` `PUT` `DELETE` `unifiedRoleAssignmentSchedule` `unifiedRoleAssignmentInstance` .

Os administradores podem usar para criar atribuições de função ativa `unifiedRoleAssignmentScheduleRequest` com ou sem hora de início e término. Embora um administrador qualificado possa usá-lo para criar uma solicitação para ativar uma atribuição de função qualificada. 


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleAssignmentScheduleRequests](../api/unifiedroleassignmentschedulerequest-list.md)|[Coleção unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Obter uma lista dos [objetos unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) e suas propriedades.|
|[Criar unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-post-unifiedroleassignmentschedulerequests.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Crie um novo [objeto unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)|
|[Obter unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-get.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Leia as propriedades e as relações de [um objeto unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)|
|[Atualizar unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-update.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Atualize as propriedades de [um objeto unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)|
|[filterByCurrentUser](../api/unifiedroleassignmentschedulerequest-filterbycurrentuser.md)|[Coleção unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Obter uma lista dos [objetos unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) e suas propriedades relacionadas a um usuário específico.|
|[cancel](../api/unifiedroleassignmentschedulerequest-cancel.md)|Nenhum|Cancela um [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) imediatamente e marca-o para exclusão em 30 dias|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|Cadeia de caracteres|Representando o tipo da operação na atribuição de função. O valor pode ser <ul><li>`AdminAdd`: Os administradores atribuem usuários/grupos a funções;</li><li>`UserAdd`: Os usuários ativam atribuições qualificadas;</li><li> `AdminUpdate`: Os administradores alteram as atribuições de função existentes</li><li>`AdminRemove`: Os administradores removem usuários/grupos de funções;<li>`UserRemove`: Os usuários desativam as atribuições ativas;<li>`UserExtend`: Os usuários solicitam estender suas atribuições de expiração;</li><li>`AdminExtend`: Os administradores estendem atribuições expiradas.</li><li>`UserRenew`: Os usuários solicitam a renovação de suas atribuições expiradas;</li><li>`AdminRenew`: Os administradores estendem atribuições expiradas.</li></ul>|
|appScopeId|Cadeia de caracteres|ID do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use "/" para o escopo de todo o locatário. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.|
|directoryScopeId|Cadeia de caracteres|ID do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.|
|id|Cadeia de caracteres|O identificador exclusivo para unifiedRoleAssignmentScheduleRequest. Chave, não anulada, somente leitura.|
|isValidationOnly|Booliano|Um booleano que determina se a chamada é uma validação ou uma chamada real. De definir essa propriedade somente se você quiser verificar se uma ativação está sujeita a regras adicionais, como MFA, antes de realmente enviar a solicitação.|
|justification|Cadeia de caracteres|Uma mensagem fornecida por usuários e administradores ao criar a solicitação sobre por que ela é necessária.|
|principalId|Cadeia de caracteres| Objectid da entidade à qual a atribuição está sendo concedida.|
|roleDefinitionId|Cadeia de caracteres|ID do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O objeto schedule da solicitação de atribuição de função.|
|targetScheduleId|Cadeia de caracteres|ID do objeto schedule anexado à atribuição.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|O objeto ticketInfo anexado à solicitação de atribuição de função que inclui detalhes do número do tíquete e do sistema de tíquetes.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Se a solicitação for de um administrador qualificado para ativar uma função, esse parâmetro mostrará a atribuição qualificada relacionada para essa ativação.|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência ao objeto de diretório que é o escopo da atribuição. Fornecido para que os chamadores possam obter o objeto de diretório `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
|principal|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência à entidade que está recebendo uma atribuição de função por meio da solicitação. Fornecido para que os chamadores possam obter a entidade principal `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Propriedade indicando a funçãoDefinition para a qual a atribuição se destina. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função. roleDefinition.Id será expandido automaticamente.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleRequest",
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

