---
title: Tipo de recurso unifiedRoleAssignmentScheduleRequest
description: Representa a solicitação de operações de atribuição de função ativa por meio do Azure AD Privileged Identity Management.
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 540f3a0e4f9fa7017dafebb1a7ee5bc51def9788
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454000"
---
# <a name="unifiedroleassignmentschedulerequest-resource-type"></a>Tipo de recurso unifiedRoleAssignmentScheduleRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a solicitação de operações de atribuição de função ativa Azure Active Directory (Azure AD) Privileged Identity Management.

**unifiedRoleAssignmentScheduleRequest** é uma entidade modelada por tíquete usada para gerenciar o ciclo de vida das atribuições de função ativa no diretório. Ele representa a intenção ou a decisão dos usuários e administradores e também oferece a flexibilidade para habilitar a implementação de agendamento recorrente, portais de aprovação e assim por diante, em comparação com a exposição direta , e operações em e `POST` `PUT` `DELETE` `unifiedRoleAssignmentSchedule` `unifiedRoleAssignmentInstance` .

Os administradores podem usar para criar atribuições de função ativa `unifiedRoleAssignmentScheduleRequest` com ou sem hora de início e término. Embora um administrador possa usá-lo para criar uma solicitação para ativar uma atribuição de função qualificada representada por [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md).

Herda da [solicitação](request.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleAssignmentScheduleRequests](../api/unifiedroleassignmentschedulerequest-list.md)|[Coleção unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Obter uma lista dos [objetos unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) e suas propriedades.|
|[Criar unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-post-unifiedroleassignmentschedulerequests.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Crie um novo [objeto unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)|
|[Obter unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-get.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Leia as propriedades e as relações de [um objeto unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)|
|[filterByCurrentUser](../api/unifiedroleassignmentschedulerequest-filterbycurrentuser.md)|[Coleção unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Obter uma lista dos [objetos unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) e suas propriedades relacionadas a um usuário específico.|
|[cancel](../api/unifiedroleassignmentschedulerequest-cancel.md)|Nenhum|Cancela um [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) imediatamente e marca-o para exclusão em 30 dias|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|Cadeia de caracteres|Representa o tipo da operação na atribuição de função. Os valores possíveis são: <ul><li>`AdminAssign`: Para que os administradores atribuam funções a usuários ou grupos.</li><li>`AdminRemove`: Para que os administradores removam usuários ou grupos de funções.</li><li> `AdminUpdate`: Para que os administradores alterem as atribuições de função existentes.</li><li>`AdminExtend`: Para que os administradores estendam atribuições expiradas.</li><li>`AdminRenew`: Para que os administradores renovem atribuições expiradas.</li><li>`SelfActivate`: Para que os usuários ativem suas atribuições.</li><li>`SelfDeactivate`: Para que os usuários desativem suas atribuições ativas.</li><li>`SelfExtend`: Para que os usuários solicitem estender suas atribuições de expiração.</li><li>`SelfRenew`: Para que os usuários solicitem a renovação de suas atribuições expiradas.</li></ul>|
|approvalId|Cadeia de caracteres|O identificador da aprovação da solicitação. Herdado da [solicitação](request.md).|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando o escopo de atribuição for específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. Use `/` para escopos de aplicativos de todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas.|
|completedDateTime|DateTimeOffset|A data de conclusão da solicitação. Herdado da [solicitação](request.md).|
|createdBy|[identitySet](identityset.md)|O usuário que criou essa solicitação. Herdado da [solicitação](request.md).|
|createdDateTime|DateTimeOffset|A data de criação da solicitação. Herdado da [solicitação](request.md).|
|customData|Cadeia de caracteres|Campo de texto livre para definir quaisquer dados personalizados para a solicitação. Não usado. Herdado da [solicitação](request.md).|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo.|
|id|Cadeia de caracteres|O identificador exclusivo para unifiedRoleAssignmentScheduleRequest. Chave, não anulada, somente leitura.|
|isValidationOnly|Booliano|Um booleano que determina se a chamada é uma validação ou uma chamada real. De definir essa propriedade somente se você quiser verificar se uma ativação está sujeita a regras adicionais, como MFA, antes de realmente enviar a solicitação.|
|justification|Cadeia de caracteres|Uma mensagem fornecida por usuários e administradores ao criar a solicitação sobre por que ela é necessária.|
|principalId|Cadeia de caracteres| Identificador da entidade à qual a atribuição está sendo concedida.|
|roleDefinitionId|Cadeia de caracteres|Identificador do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O objeto schedule da solicitação de atribuição de função.|
|status|Cadeia de caracteres|O objeto schedule da solicitação de atribuição de função. Herdado da [solicitação](request.md).|
|targetScheduleId|Cadeia de caracteres|Identificador do objeto schedule anexado à atribuição.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|O objeto ticketInfo anexado à solicitação de atribuição de função que inclui detalhes do número do tíquete e do sistema de tíquetes.|

## <a name="relationships"></a>Relacionamentos
|Relação|Tipo|Descrição|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Se a solicitação for de um administrador qualificado para ativar uma função, esse parâmetro mostrará a atribuição qualificada relacionada para essa ativação.|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência ao objeto de diretório que é o escopo da atribuição. Fornecido para que os chamadores possam obter o objeto de diretório `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
|principal|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência à entidade que está recebendo uma atribuição de função por meio da solicitação. Fornecido para que os chamadores possam obter a entidade principal `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Propriedade indicando a funçãoDefinition para a qual a atribuição se destina. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função. roleDefinition.Id será expandido automaticamente.|
|targetSchedule|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)| Propriedade indicando o cronograma de uma atribuição de função qualificada. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest",
  "baseType": "microsoft.graph.request",
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

