---
title: tipo de recurso de privilegedRoleSummary
description: As estatísticas de resumida de uma determinada função.
localization_priority: Normal
ms.openlocfilehash: 2ed34f556f52c41729bfa108fbb6eb0c608f6b67
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513736"
---
# <a name="privilegedrolesummary-resource-type"></a>tipo de recurso de privilegedRoleSummary

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As estatísticas de resumida de uma determinada função.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |Leia as propriedades e os relacionamentos do objeto privilegedRoleSummary.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|elevatedCount|int32|O número de usuários que possuem a função atribuída e a função está ativado.|
|id|string| O identificador exclusivo para a função. Somente leitura.|
|managedCount|int32|O número de usuários que possuem a função atribuída, mas a função é desativado.|
|mfaEnabled|booliano|**true** se a ativação de função requer MFA. **false** se a ativação de função não exige MFA.|
|status|string| Os valores possíveis são: `ok` e `bad`. O valor depende a proporção entre (managedCount / usersCount). Se a taxa for menor que um limite predefinido, `ok` é retornado. Caso contrário, `bad` é retornado.|
|usersCount|int32|O número de usuários que são atribuídos com a função.|

## <a name="relationships"></a>Relacionamento
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
}-->

```json
{
  "elevatedCount": 1024,
  "id": "string (identifier)",
  "managedCount": 1024,
  "mfaEnabled": true,
  "status": "string",
  "usersCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesummary.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
