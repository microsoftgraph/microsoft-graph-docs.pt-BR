---
title: Tipo de recurso unifiedRoleEligibilityScheduleRequest
description: Representa a solicitação de operações de atribuição de função qualificadas por meio do Azure AD Privileged Identity Management.
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ce25402cb8d16cb16cd38630005b7afe0659bbe5
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510089"
---
# <a name="unifiedroleeligibilityschedulerequest-resource-type"></a>Tipo de recurso unifiedRoleEligibilityScheduleRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a solicitação de atribuição de função qualificada por meio do Azure AD Privileged Identity Management.

**unifiedRoleEligibilityScheduleRequest** é uma entidade modelada por tíquete usada para gerenciar o ciclo de vida das atribuições de função qualificadas no diretório. Ele representa a intenção ou a decisão dos usuários e administradores e também oferece a flexibilidade para habilitar a implementação de agendamento recorrente, portas de aprovação e assim por diante, `POST`em comparação com a exposição direta , `PUT`e `DELETE` operações em **unifiedRoleEligibilitySchedule** e **unifiedRoleEligibilityInstance** resources.

Os administradores podem usar **unifiedRoleEligibilityScheduleRequest'** para criar e/ou atualizar atribuições de função qualificadas com ou sem hora de início e término. Embora administradores qualificados, podem usá-lo para criar uma solicitação para estender ou renovar suas atribuições qualificadas.

Herda da [solicitação](request.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleEligibilityScheduleRequests](../api/unifiedroleeligibilityschedulerequest-list.md)|[Coleção unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Obter uma lista dos [objetos unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) e suas propriedades.|
|[Criar unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-post-unifiedroleeligibilityschedulerequests.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Crie um novo [objeto unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) .|
|[Obter unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-get.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Leia as propriedades e as relações de [um objeto unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) .|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedulerequest-filterbycurrentuser.md)|[Coleção unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Obter uma lista dos [objetos unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) e suas propriedades relacionadas a um usuário específico.|
|[cancel](../api/unifiedroleeligibilityschedulerequest-cancel.md)|Nenhum|Cancela um [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) imediatamente e marca-o para exclusão em 30 dias|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|Cadeia de caracteres|Representa o tipo da operação na atribuição de qualificação de função. Os valores possíveis são: <ul><li>`AdminAssign`: Para que os administradores atribuam qualificação de função a usuários ou grupos a funções.</li><li>`AdminExtend`: Para que os administradores estendam atribuições expiradas.</li><li>`AdminUpdate`: Para que os administradores alterem as atribuições de função existentes.</li><li>`AdminRenew`: Para que os administradores renovem atribuições expiradas.</li><li>`AdminRemove`: Para que os administradores removam usuários ou grupos de funções qualificadas.</li><li>`UserAdd`: Para que os usuários ativem suas atribuições qualificadas.</li><li>`UserExtend`: Para que os usuários solicitem estender suas atribuições qualificadas expiradas.</li><li>`UserRemove`: Para que os usuários desativem suas atribuições elegíveis ativas.</li><li>`UserRenew`: Para que os usuários solicitem a renovação de suas atribuições qualificadas expiradas.</li></ul>|
|approvalId|Cadeia de caracteres|O identificador da aprovação da solicitação. Herdado da [solicitação](request.md).|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando o escopo de atribuição for específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. Use `/` para escopos de aplicativos de todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas.|
|completedDateTime|DateTimeOffset|A data de conclusão da solicitação. Herdado da [solicitação](request.md).|
|createdBy|[identitySet](identityset.md)|O usuário que criou essa solicitação. Herdado da [solicitação](request.md).|
|createdDateTime|DateTimeOffset|A data de criação da solicitação. Herdado da [solicitação](request.md).|
|customData|Cadeia de caracteres|Campo de texto livre para definir quaisquer dados personalizados para a solicitação. Não usado. Herdado da [solicitação](request.md).|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo.|
|id|String|O identificador exclusivo para unifiedRoleEligibilityScheduleRequest. Somente leitura.|
|isValidationOnly|Booliano|Um booleano que determina se a chamada é uma validação ou uma chamada real. De definir essa propriedade somente se você quiser verificar se uma ativação está sujeita a regras adicionais, como MFA, antes de realmente enviar a solicitação.|
|justification|Cadeia de caracteres|Uma mensagem fornecida por usuários e administradores ao criar a solicitação sobre por que ela é necessária.|
|principalId|String| Identificador da entidade à qual a atribuição está sendo concedida. Por exemplo, um usuário ou um grupo. Para grupos, eles devem ser atribuídos a funções, ou seja, **o isAssignableToRole** da propriedade group definida como `true`.|
|roleDefinitionId|Cadeia de caracteres|Identificador do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O objeto schedule da solicitação de atribuição de função.|
|status|Cadeia de caracteres|O objeto schedule da solicitação de qualificação de função. Herdado da [solicitação](request.md).|
|targetScheduleId|Cadeia de caracteres|O período de tempo para o qual a atribuição de qualificação é válida.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Os detalhes do número do tíquete e do sistema de tíquetes anexados à solicitação de atribuição de função.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência ao objeto de diretório que é o escopo da atribuição. Fornecido para que os chamadores possam obter o objeto de diretório usando `$expand` ao mesmo tempo que obter a atribuição de função. Somente leitura.|
|principal|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência à entidade que está recebendo uma atribuição de função por meio da solicitação. Fornecido para que os chamadores possam obter a entidade principal `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Propriedade indicando a funçãoDefinition para a qual a atribuição se destina. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função. roleDefinition.Id será expandido automaticamente.|
|targetSchedule|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)| Propriedade indicando o cronograma de uma atribuição de função qualificada. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest",
  "baseType": "microsoft.graph.request",
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

