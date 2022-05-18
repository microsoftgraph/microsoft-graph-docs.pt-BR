---
title: Tipo de recurso unifiedRoleEligibilityScheduleRequest
description: Representa a solicitação para operações de atribuição de função qualificadas por meio Azure AD Privileged Identity Management.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 82224699c7bbe80e9ec14e39494fd8a37c1d31be
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461349"
---
# <a name="unifiedroleeligibilityschedulerequest-resource-type"></a>Tipo de recurso unifiedRoleEligibilityScheduleRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a solicitação de atribuição de função qualificada por meio Azure AD Privileged Identity Management.

**unifiedRoleEligibilityScheduleRequest** é uma entidade modelada por tíquete usada para gerenciar o ciclo de vida de atribuições de função qualificadas no diretório. Ele representa a intenção ou decisão dos usuários e administradores e também fornece a flexibilidade para habilitar a implementação de agendamento recorrente, portões de aprovação e assim por diante, `POST`em comparação com a exposição direta , `DELETE` `PUT`e operações em **recursos unifiedRoleEligibilitySchedule** e **unifiedRoleEligibilityInstance**.

Os administradores podem usar **unifiedRoleEligibilityScheduleRequest'** para criar e/ou atualizar atribuições de função qualificadas com ou sem hora de início e término. Embora administradores qualificados, podem usá-lo para criar uma solicitação para estender ou renovar suas atribuições qualificadas.

Herda da [solicitação](request.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleEligibilityScheduleRequests](../api/rbacapplication-list-roleeligibilityschedulerequests.md)|[Coleção unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Obtenha uma lista dos [objetos unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) e suas propriedades.|
|[Criar unifiedRoleEligibilityScheduleRequest](../api/rbacapplication-post-roleeligibilityschedulerequests.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Crie um novo [objeto unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) .|
|[Obter unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-get.md)|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Leia as propriedades e as relações de um [objeto unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) .|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedulerequest-filterbycurrentuser.md)|[Coleção unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)|Obtenha uma lista dos [objetos unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) e suas propriedades relacionadas a um usuário específico.|
|[cancel](../api/unifiedroleeligibilityschedulerequest-cancel.md)|Nenhum|Cancela um [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) imediatamente e marca-o para exclusão em 30 dias|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|String|Representa o tipo da operação na atribuição de qualificação de função. Os valores possíveis são: <ul><li>`AdminAssign`: para que os administradores atribuam elegibilidade de função a usuários ou grupos a funções.</li><li>`AdminExtend`: para que os administradores estendam as atribuições de expiração.</li><li>`AdminUpdate`: para que os administradores alterem as atribuições de função existentes.</li><li>`AdminRenew`: para que os administradores renovem atribuições expiradas.</li><li>`AdminRemove`: para administradores removerem usuários ou grupos de funções qualificadas.</li><li>`UserAdd`: para que os usuários ativem suas atribuições qualificadas.</li><li>`UserExtend`: para que os usuários solicitem a extensão de suas atribuições qualificadas de expiração.</li><li>`UserRemove`: para que os usuários desativem suas atribuições qualificadas ativas.</li><li>`UserRenew`: para que os usuários solicitem a renovação de suas atribuições qualificadas expiradas.</li></ul>|
|approvalId|String|O identificador da aprovação da solicitação. Herdado da [solicitação](request.md).|
|appScopeId|String|Identificador do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas.|
|completedDateTime|DateTimeOffset|A data de conclusão da solicitação. Herdado da [solicitação](request.md).|
|createdBy|[identitySet](identityset.md)|O usuário que criou essa solicitação. Herdado da [solicitação](request.md).|
|createdDateTime|DateTimeOffset|A data de criação da solicitação. Herdado da [solicitação](request.md).|
|Customdata|String|Campo de texto livre para definir quaisquer dados personalizados para a solicitação. Não usado. Herdado da [solicitação](request.md).|
|directoryScopeId|String|Identificador do objeto de diretório que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo.|
|id|String|O identificador exclusivo para unifiedRoleEligibilityScheduleRequest. Somente leitura.|
|isValidationOnly|Booliano|Um booliano que determina se a chamada é uma validação ou uma chamada real. Defina essa propriedade somente se você quiser verificar se uma ativação está sujeita a regras adicionais, como MFA, antes de realmente enviar a solicitação.|
|Justificação|String|Uma mensagem fornecida por usuários e administradores ao criar a solicitação sobre por que ela é necessária.|
|principalId|String| Identificador da entidade de segurança à qual a atribuição está sendo concedida. Por exemplo, um usuário ou um grupo. Para grupos, eles devem ser atribuíveis a funções, ou seja, **o isAssignableToRole** da propriedade de grupo definida como `true`.|
|roleDefinitionId|String|Identificador do unifiedRoleDefinition para o que a atribuição se aplica. Somente leitura.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O objeto de agendamento da solicitação de atribuição de função.|
|status|String|O objeto de agendamento da solicitação de qualificação de função. Herdado da [solicitação](request.md).|
|targetScheduleId|String|O período de tempo para o qual a atribuição de qualificação é válida.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Os detalhes do número do tíquete e do sistema de tíquetes anexados à solicitação de atribuição de função.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Propriedade que faz referência ao objeto de diretório que é o escopo da atribuição. Fornecido para que os chamadores possam obter o objeto de `$expand` diretório usando ao mesmo tempo que obter a atribuição de função. Somente leitura.|
|principal|[directoryObject](../resources/directoryobject.md)|Propriedade que faz referência à entidade de segurança que está obtendo uma atribuição de função por meio da solicitação. Fornecido para que os chamadores possam obter a entidade de segurança `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Propriedade que indica a roleDefinition para a atribuição. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função. roleDefinition.Id será expandido automaticamente.|
|targetSchedule|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)| Propriedade que indica o agendamento de uma atribuição de função qualificada. |

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

