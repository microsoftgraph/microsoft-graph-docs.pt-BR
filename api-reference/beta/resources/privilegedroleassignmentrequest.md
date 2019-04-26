---
title: tipo de recurso privilegedRoleAssignmentRequest
description: Representa a solicitação de operações de atribuição de função no gerenciamento de identidade do Privilegd.
localization_priority: Normal
ms.openlocfilehash: ead028d61fcbf6fe7cebf13291c0ba5231f0ba22
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344254"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a>tipo de recurso privilegedRoleAssignmentRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a solicitação de operações de atribuição de função no gerenciamento de identidade do Privilegd.

`privilegedRoleAssignmentRequest`é uma entidade com modelo de tíquete usada para gerenciar o ciclo de vida das atribuições de função. Ele representa a intenção/decisão dos usuários e administradores, e também fornece a flexibilidade para permitir a implementação de Schduling recorrentes, Gates de aprovação e assim por diante, em comparação com as `POST` operações `LIST` e exposição diretas, bem como `MY` e `Cancel` funções em `governanceRoleAssignment`.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[List](../api/privilegedroleassignmentrequest-list.md) | coleção [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|Listar solicitações de atribuição de função.|
|[Criar](../api/privilegedroleassignmentrequest-post.md)|  [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|Criar uma solicitação para gerenciar o ciclo de vida da atribuição de função nova ou existente.|
|[Cancel](../api/privilegedroleassignmentrequest-cancel.md)|  |Cancelar uma solicitação de atribuição de função pendente.|
|[Pessoal](../api/privilegedroleassignmentrequest-my.md)|  |Obter solicitação de atribuição de função para o requstor atual.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura. A ID da solicitação de atribuição de função.|
|assignmentstate|String| O estado da atribuição. O valor pode ser `Eligible` para atribuição `Active` qualificada-se for diretamente atribuído `Active` por administradores ou ativado em uma atribuição qualificada pelos usuários.|
|duration|String| A duração de uma atribuição de função.|
|motivos|String| O motivo da atribuição de função.|
|requestedDateTime|DateTimeOffset| Somente leitura. O tempo de criação da solicitação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|roleId|String| A ID da função.|
|futebol|[governanceSchedule](governanceschedule.md)| O objeto Schedule da solicitação de atribuição de função.|
|status|String| Somente leitura. o status da solicitação de atribuição de função. O valor pode ser `NotStarted`,`Completed`,`RequestedApproval``Scheduled``Approved``ApprovalDenied``ApprovalAborted``Cancelling`,,,,,,,`RequestExpired``Cancelled``Revoked`|
|ticketNumber|String| O ticketNumber da atribuição de função. |
|ticketSystem|String| O ticketSystem da atribuição de função.|
|type|String| Representando o tipo da operação na atribuição de função. O valor pode ser `AdminAdd`: os administradores adicionam usuários a funções; `UserAdd`: Os usuários adicionam atribuições de função.|
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
