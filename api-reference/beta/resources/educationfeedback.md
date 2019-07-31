---
title: tipo de recurso educationFeedback
description: Comentários de um professor para um aluno. Essa propriedade representa a parte de texto do comentário junto com quem.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7300c5f2d46a3a60a104288d8ee9559e6cf5fd2c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006413"
---
# <a name="educationfeedback-resource-type"></a>tipo de recurso educationFeedback

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Comentários de um professor para um aluno. Essa propriedade representa a parte de texto do comentário junto com quem.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|feedbackBy|[identitySet](identityset.md)|Usuário que criou o comentário.|
|feedbackDateTime|DateTimeOffset|Momento no momento em que o comentário foi fornecido. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|texto|[itemBody](itembody.md)|Solicitações.|

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
  "suppressions": []
}
-->
