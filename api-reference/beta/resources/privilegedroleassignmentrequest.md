---
title: Tipo de recurso privilegedRoleAssignmentRequest
description: Representa a solicitação para operações de atribuição de função no Privilegd Identity Management.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: a22049c1f3de095e7146a1e9cd901db8d6f5fd6a
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398851"
---
# <a name="privilegedroleassignmentrequest-resource-type-deprecated"></a>Tipo de recurso privilegedRoleAssignmentRequest (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2AADRoles-deprecation](../../includes/pim-v2AADRoles-deprecation.md)]

Representa a solicitação para operações de atribuição de função Privileged Identity Management (PIM).

`privilegedRoleAssignmentRequest` é uma entidade modelada por tíquete usada para gerenciar o ciclo de vida das atribuições de função. Ele representa a intenção/decisão dos usuários e administradores e também fornece a flexibilidade para habilitar a implementação de esquemas recorrentes, portões de aprovação e assim por diante, `POST` `Cancel` `LIST` `MY` em comparação com a exposição direta e operações, bem como funções em .`governanceRoleAssignment`

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[Listar](../api/privilegedroleassignmentrequest-list.md) | [coleção privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|Listar solicitações de atribuição de função.|
|[Criar](../api/privilegedroleassignmentrequest-post.md)|  [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|Crie uma solicitação para gerenciar o ciclo de vida da atribuição de função existente ou nova.|
|[Cancel](../api/privilegedroleassignmentrequest-cancel.md)|  |Cancele uma solicitação de atribuição de função pendente.|
|[Pessoal](../api/privilegedroleassignmentrequest-my.md)|  |Obtenha a solicitação de atribuição de função para o repositório atual.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura. A ID da solicitação de atribuição de função.|
|assignmentState|Cadeia de caracteres| O estado da atribuição. O valor pode ser `Eligible` para `Active` atribuição qualificada - `Active` se ele for atribuído diretamente por administradores ou ativado em uma atribuição qualificada pelos usuários.|
|duração|Cadeia de caracteres| A duração de uma atribuição de função.|
|motivo|Cadeia de caracteres| O motivo da atribuição de função.|
|requestedDateTime|DateTimeOffset| Somente leitura. A hora de criação da solicitação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|roleId|Cadeia de caracteres| A ID da função.|
|Cronograma|[governanceSchedule](governanceschedule.md)| O objeto de agendamento da solicitação de atribuição de função.|
|status|Cadeia de caracteres| Somente leitura. O status da solicitação de atribuição de função. O valor pode ser `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,,`Cancelling`,`Cancelled`,`Revoked`,.`RequestExpired`|
|ticketNumber|Cadeia de caracteres| O ticketNumber para a atribuição de função. |
|ticketSystem|Cadeia de caracteres| O ticketSystem para a atribuição de função.|
|type|Cadeia de caracteres| Representando o tipo da operação na atribuição de função. O valor pode ser: administradores `AdminAdd`adicionam usuários a funções;`UserAdd`: os usuários adicionam atribuições de função.|
|userId|Cadeia de caracteres| A ID do usuário.|

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


