---
title: tipo de recurso privilegedRoleAssignmentRequest
description: Representa a solicitação de operações de atribuição de função no gerenciamento de identidade do Privilegd.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 5daeeee6f784c31f1e15843a8a1903ca41565118
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070506"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a>tipo de recurso privilegedRoleAssignmentRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a solicitação de operações de atribuição de função no gerenciamento de identidade do Privilegd.

`privilegedRoleAssignmentRequest` é uma entidade com modelo de tíquete usada para gerenciar o ciclo de vida das atribuições de função. Ele representa a intenção/decisão dos usuários e administradores, e também fornece a flexibilidade para permitir a implementação de Schduling recorrentes, Gates de aprovação e assim por diante, em comparação com a exposição e operações diretas, `POST` `LIST` bem como `MY` e `Cancel` funções `governanceRoleAssignment` .

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[List](../api/privilegedroleassignmentrequest-list.md) | coleção [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|Listar solicitações de atribuição de função.|
|[Create](../api/privilegedroleassignmentrequest-post.md)|  [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|Criar uma solicitação para gerenciar o ciclo de vida da atribuição de função nova ou existente.|
|[Cancel](../api/privilegedroleassignmentrequest-cancel.md)|  |Cancelar uma solicitação de atribuição de função pendente.|
|[Pessoal](../api/privilegedroleassignmentrequest-my.md)|  |Obter solicitação de atribuição de função para o requstor atual.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura. A ID da solicitação de atribuição de função.|
|assignmentstate|Cadeia de caracteres| O estado da atribuição. O valor pode ser `Eligible` para atribuição qualificada `Active` -se for diretamente atribuído `Active` por administradores ou ativado em uma atribuição qualificada pelos usuários.|
|duration|Cadeia de caracteres| A duração de uma atribuição de função.|
|motivo|Cadeia de caracteres| O motivo da atribuição de função.|
|requestedDateTime|DateTimeOffset| Somente leitura. O tempo de criação da solicitação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|roleId|Cadeia de caracteres| A ID da função.|
|Cronograma|[governanceSchedule](governanceschedule.md)| O objeto Schedule da solicitação de atribuição de função.|
|status|String| Somente leitura. o status da solicitação de atribuição de função. O valor pode ser,,,,,,,,, `NotStarted` `Completed` `RequestedApproval` `Scheduled` `Approved` `ApprovalDenied` `ApprovalAborted` `Cancelling` `Cancelled` `Revoked` `RequestExpired` .|
|ticketNumber|Cadeia de caracteres| O ticketNumber da atribuição de função. |
|ticketSystem|Cadeia de caracteres| O ticketSystem da atribuição de função.|
|tipo|Cadeia de caracteres| Representando o tipo da operação na atribuição de função. O valor pode ser `AdminAdd` : os administradores adicionam usuários a funções; `UserAdd` : os usuários adicionam atribuições de função.|
|userId|Cadeia de caracteres| A ID do usuário.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|roleInfo|[privilegedRole](privilegedrole.md)| O objeto roleInfo da solicitação de atribuição de função.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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
  "suppressions": []
}
-->


