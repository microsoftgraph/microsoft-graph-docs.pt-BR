---
title: tipo de recurso de privilegedRoleAssignmentRequest
description: Representa a solicitação para operações de atribuição de função no gerenciamento de identidades Privilegd.
localization_priority: Normal
ms.openlocfilehash: a0cb0bc03d8bb2436e45139bc9db5322cc3970cf
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571741"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a>tipo de recurso de privilegedRoleAssignmentRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a solicitação para operações de atribuição de função no gerenciamento de identidades Privilegd.

`privilegedRoleAssignmentRequest`uma entidade modelada de tíquete é usada para gerenciar o ciclo de vida de atribuições de função. Ele representa a intenção/decisão dos usuários e administradores e também oferece flexibilidade para permitir a implementação de schduling recorrente, entradas de aprovação e assim por diante, em relação ao diretamente expondo `POST` e `LIST` operações bem como `MY` e `Cancel` funciona em `governanceRoleAssignment`.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[List](../api/privilegedroleassignmentrequest-list.md) | coleção [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)|Lista solicitações de atribuição de função.|
|[Create](../api/privilegedroleassignmentrequest-post.md)|  [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)|Crie uma solicitação para gerenciar o ciclo de vida de atribuição de função de novo ou existente.|
|[Cancel](../api/privilegedroleassignmentrequest-cancel.md)|  |Cancele uma solicitação de atribuição de função pendente.|
|[Pessoal](../api/privilegedroleassignmentrequest-my.md)|  |Obtenha a solicitação de atribuição de função para o solicitante atual.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura. A identificação da solicitação de atribuição de função.|
|assignmentState|String| O estado da atribuição. O valor pode ser `Eligible` para atribuição elegível `Active` - se ele é atribuído diretamente `Active` pelos administradores, ou ativado em uma atribuição elegível pelos usuários.|
|duration|String| A duração de uma atribuição de função.|
|motivo|String| O motivo para a atribuição de função.|
|requestedDateTime|DateTimeOffset| Somente leitura. A solicitação criar horário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|roleId|String| A identificação da função.|
|agenda|[microsoft.graph.governanceSchedule](governanceschedule.md)| O objeto de agendamento da solicitação de atribuição de função.|
|status|String| Leitura-only.The o status da solicitação de atribuição de função. O valor pode ser `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.|
|ticketNumber|String| TicketNumber para a atribuição de função. |
|ticketSystem|String| TicketSystem para a atribuição de função.|
|type|String| Representando o o tipo da operação na atribuição de função. O valor pode ser `AdminAdd`: administradores adicionar usuários às funções; `UserAdd`: Os usuários adicionar atribuições de função.|
|userId|String| A identificação do usuário.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|roleInfo|[privilegedRole](privilegedrole.md)| O objeto roleInfo da solicitação de atribuição de função.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
}-->

```json
{
  "assignmentState": "String",
  "duration": "String",
  "id": "String (identifier)",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "roleId": "String",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": "String",
  "ticketNumber": "String",
  "ticketSystem": "String",
  "type": "String",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedroleassignmentrequest.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
