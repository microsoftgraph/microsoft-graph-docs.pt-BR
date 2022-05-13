---
title: Tipo de recurso unifiedRoleAssignmentScheduleRequest
description: Representa a solicitação para operações de atribuição de função ativa por meio Azure AD Privileged Identity Management.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 14578e3f35403bc549dbb1fa64c1a104f059f13a
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397940"
---
# <a name="unifiedroleassignmentschedulerequest-resource-type"></a>Tipo de recurso unifiedRoleAssignmentScheduleRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a solicitação para operações de atribuição de função Azure Active Directory (Azure AD) Privileged Identity Management.

**unifiedRoleAssignmentScheduleRequest** é uma entidade modelada por tíquete usada para gerenciar o ciclo de vida de atribuições de função ativas no diretório. Ele representa a intenção ou a decisão dos usuários e administradores e também fornece a flexibilidade para habilitar a implementação de agendamento recorrente, portões de aprovação e assim por diante, `POST`em comparação com a exposição direta, `PUT`e `DELETE` `unifiedRoleAssignmentSchedule` operações em e `unifiedRoleAssignmentInstance`.

Os administradores podem usar `unifiedRoleAssignmentScheduleRequest` para criar atribuições de função ativas com ou sem a hora de início e término. Embora um administrador possa usá-lo para criar uma solicitação para ativar uma atribuição de função qualificada representada por [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md).

Herda da [solicitação](request.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleAssignmentScheduleRequests](../api/unifiedroleassignmentschedulerequest-list.md)|[Coleção unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Obtenha uma lista dos [objetos unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) e suas propriedades.|
|[Criar unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-post-unifiedroleassignmentschedulerequests.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Crie um novo [objeto unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) .|
|[Obter unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-get.md)|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Leia as propriedades e as relações de um [objeto unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) .|
|[filterByCurrentUser](../api/unifiedroleassignmentschedulerequest-filterbycurrentuser.md)|[Coleção unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)|Obtenha uma lista dos [objetos unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) e suas propriedades relacionadas a um usuário específico.|
|[cancel](../api/unifiedroleassignmentschedulerequest-cancel.md)|Nenhum|Cancela um [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) imediatamente e marca-o para exclusão em 30 dias|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|Cadeia de caracteres|Representa o tipo da operação na atribuição de função. Os valores possíveis são: <ul><li>`AdminAssign`: para administradores atribuirem funções a usuários ou grupos.</li><li>`AdminRemove`: para administradores removerem usuários ou grupos de funções.</li><li> `AdminUpdate`: para que os administradores alterem as atribuições de função existentes.</li><li>`AdminExtend`: para que os administradores estendam as atribuições de expiração.</li><li>`AdminRenew`: para que os administradores renovem atribuições expiradas.</li><li>`SelfActivate`: para que os usuários ativem suas atribuições.</li><li>`SelfDeactivate`: para que os usuários desativem suas atribuições ativas.</li><li>`SelfExtend`: para que os usuários solicitem a extensão de suas atribuições de expiração.</li><li>`SelfRenew`: para que os usuários solicitem a renovação de suas atribuições expiradas.</li></ul>|
|approvalId|Cadeia de caracteres|O identificador da aprovação da solicitação. Herdado da [solicitação](request.md).|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas.|
|completedDateTime|DateTimeOffset|A data de conclusão da solicitação. Herdado da [solicitação](request.md).|
|createdBy|[identitySet](identityset.md)|O usuário que criou essa solicitação. Herdado da [solicitação](request.md).|
|createdDateTime|DateTimeOffset|A data de criação da solicitação. Herdado da [solicitação](request.md).|
|Customdata|Cadeia de caracteres|Campo de texto livre para definir quaisquer dados personalizados para a solicitação. Não usado. Herdado da [solicitação](request.md).|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto de diretório que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo.|
|id|Cadeia de caracteres|O identificador exclusivo para unifiedRoleAssignmentScheduleRequest. Chave, não anulável, somente leitura.|
|isValidationOnly|Booliano|Um booliano que determina se a chamada é uma validação ou uma chamada real. Defina essa propriedade somente se você quiser verificar se uma ativação está sujeita a regras adicionais, como MFA, antes de realmente enviar a solicitação.|
|Justificação|Cadeia de caracteres|Uma mensagem fornecida por usuários e administradores ao criar a solicitação sobre por que ela é necessária.|
|principalId|Cadeia de caracteres| Identificador da entidade de segurança à qual a atribuição está sendo concedida.|
|roleDefinitionId|Cadeia de caracteres|Identificador do unifiedRoleDefinition para o que a atribuição se aplica. Somente leitura.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O objeto de agendamento da solicitação de atribuição de função.|
|status|Cadeia de caracteres|O objeto de agendamento da solicitação de atribuição de função. Herdado da [solicitação](request.md).|
|targetScheduleId|Cadeia de caracteres|Identificador do objeto de agenda anexado à atribuição.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|O objeto ticketInfo anexado à solicitação de atribuição de função que inclui detalhes do número do tíquete e do sistema de tíquetes.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Se a solicitação for de um administrador qualificado para ativar uma função, esse parâmetro mostrará a atribuição qualificada relacionada para essa ativação.|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Propriedade que faz referência ao objeto de diretório que é o escopo da atribuição. Fornecido para que os chamadores possam obter o objeto de `$expand` diretório usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
|principal|[directoryObject](../resources/directoryobject.md)|Propriedade que faz referência à entidade de segurança que está obtendo uma atribuição de função por meio da solicitação. Fornecido para que os chamadores possam obter a entidade de segurança `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Propriedade que indica a roleDefinition para a atribuição. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função. roleDefinition.Id será expandido automaticamente.|
|targetSchedule|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)| Propriedade que indica o agendamento de uma atribuição de função qualificada. |

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

