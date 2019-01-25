---
title: tipo de recurso de privilegedApproval
description: Representa uma aprovação solicitada no gerenciamento de identidades privilegiado para entrar em uma função.
localization_priority: Normal
ms.openlocfilehash: 283236d945e9a71a4ae0461bbefe66260efa88a4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516886"
---
# <a name="privilegedapproval-resource-type"></a>tipo de recurso de privilegedApproval

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma aprovação solicitada no gerenciamento de identidades privilegiado para entrar em uma função.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter privilegedApproval](../api/privilegedapproval-get.md) | [privilegedApproval](privilegedapproval.md) |Leia as propriedades e os relacionamentos do objeto privilegedApproval.|
|[Objetos de privilegedApproval List](../api/privilegedapproval-list.md) | coleção [privilegedApproval](privilegedapproval.md)|Obtenha a coleção de privilegedApproval.|
|[Criar privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |Crie objeto privilegedApproval. |
|[Atualizar privilegedApproval](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |Atualize o objeto privilegedApproval. |
|[Myrequests](../api/privilegedapproval-myrequests.md)|[privilegedApproval](privilegedapproval.md)|Obtenha as solicitações de aprovação do solicitador.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|approvalDuration|Duration||
|approvalState|string| Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.|
|approvalType|String||
|approverReason|String||
|endDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String| Somente leitura.|
|requestorReason|String||
|roleId|String||
|startDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|userId|Cadeia de caracteres||

## <a name="relationships"></a>Relacionamento
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| Somente leitura. Anulável.|
|Solicitação|[privilegedRoleAssignmentRequest](privilegedroleassignmentrequest.md)| Somente leitura. A solicitação de atribuição de função para este objeto de aprovação|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedApproval"
}-->

```json
{
  "approvalDuration": "string (timestamp)",
  "approvalState": "string",
  "approvalType": "string",
  "approverReason": "String",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "requestorReason": "String",
  "roleId": "String",
  "startDateTime": "String (timestamp)",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedapproval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
