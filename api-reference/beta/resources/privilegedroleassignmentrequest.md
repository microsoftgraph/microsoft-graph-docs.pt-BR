---
title: Tipo de recurso privilegedRoleAssignmentRequest
description: Representa a solicitação de operações de atribuição de função em Gerenciamento de Identidade Privilegd.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: b6e7a9c4a761b699ffe4128a62fd69a75a0662df
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722257"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a>Tipo de recurso privilegedRoleAssignmentRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a solicitação de operações de atribuição de função em Gerenciamento de Identidade Privilegd.

`privilegedRoleAssignmentRequest` é uma entidade modelada por tíquete usada para gerenciar o ciclo de vida das atribuições de função. Ele representa a intenção/decisão dos usuários e administradores e também oferece a flexibilidade para habilitar a implementação de esquemas `POST` `LIST` `MY` `Cancel` recorrentes, portais de aprovação e assim por diante, em comparação com a exposição direta e operações, bem como e funções em `governanceRoleAssignment` .

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[List](../api/privilegedroleassignmentrequest-list.md) | [Coleção privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|Listar solicitações de atribuição de função.|
|[Create](../api/privilegedroleassignmentrequest-post.md)|  [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|Crie uma solicitação para gerenciar o ciclo de vida da atribuição de função existente ou nova.|
|[Cancel](../api/privilegedroleassignmentrequest-cancel.md)|  |Cancele uma solicitação de atribuição de função pendente.|
|[Pessoal](../api/privilegedroleassignmentrequest-my.md)|  |Obter solicitação de atribuição de função para o requstor atual.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura. A id da solicitação de atribuição de função.|
|assignmentState|Cadeia de caracteres| O estado da atribuição. O valor pode ser para atribuição qualificada - se ele for atribuído diretamente pelos administradores ou ativado em uma atribuição qualificada `Eligible` `Active` pelos `Active` usuários.|
|duração|Cadeia de caracteres| A duração de uma atribuição de função.|
|motivo|Cadeia de caracteres| O motivo da atribuição de função.|
|requestedDateTime|DateTimeOffset| Somente leitura. A solicitação cria tempo. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|roleId|Cadeia de caracteres| A id da função.|
|Cronograma|[governanceSchedule](governanceschedule.md)| O objeto schedule da solicitação de atribuição de função.|
|status|Cadeia de caracteres| Somente leitura.O status da solicitação de atribuição de função. O valor pode `NotStarted` ser , , , , , , , , `Completed` , , , `RequestedApproval` `Scheduled` `Approved` `ApprovalDenied` `ApprovalAborted` `Cancelling` `Cancelled` `Revoked` `RequestExpired` .|
|ticketNumber|Cadeia de caracteres| O ticketNumber para a atribuição de função. |
|ticketSystem|Cadeia de caracteres| O ticketSystem para a atribuição de função.|
|tipo|Cadeia de caracteres| Representando o tipo da operação na atribuição de função. O valor pode ser `AdminAdd` : Administradores adicionam usuários a funções; `UserAdd` : Os usuários adicionam atribuições de função.|
|userId|Cadeia de caracteres| A id do usuário.|

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


