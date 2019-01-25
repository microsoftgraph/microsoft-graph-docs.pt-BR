---
title: tipo de recurso de educationFeedback
description: Os comentários feitos durante um professor para um estudante. Essa propriedade representa a parte de texto dos comentários, juntamente com quem.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 90e55b20b371d04bc3c6d45bb84fe6bf42157a2f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515633"
---
# <a name="educationfeedback-resource-type"></a>tipo de recurso de educationFeedback

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os comentários feitos durante um professor para um estudante. Essa propriedade representa a parte de texto dos comentários, juntamente com quem.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|feedbackBy|[identitySet](identityset.md)|Usuário que criou o feedback.|
|feedbackDateTime|DateTimeOffset|Momento específico quando o feedback dado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|texto|[itemBody](itembody.md)|Comentários|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedback"
}-->

```json
{
  "feedbackBy": {"@odata.type": "microsoft.graph.identitySet"},
  "feedbackDateTime": "String (timestamp)",
  "text": {"@odata.type": "microsoft.graph.itemBody"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfeedback.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
