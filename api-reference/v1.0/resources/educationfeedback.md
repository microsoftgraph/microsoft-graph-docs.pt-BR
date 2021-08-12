---
title: Tipo de recurso educationFeedback
description: Comentários de um professor para um aluno.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 87aba918c8766434c3bfc18e3020c2d05517d612887179f04c3bf3a427be1aef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218734"
---
# <a name="educationfeedback-resource-type"></a>Tipo de recurso educationFeedback

Namespace: microsoft.graph

Comentários de um professor para um aluno. 

Essa propriedade representa a parte de texto dos comentários juntamente com quem forneceu os comentários.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|feedbackBy|[identitySet](identityset.md)|Usuário que criou os comentários.|
|feedbackDateTime|DateTimeOffset|Momento no tempo em que os comentários foram dados. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|texto|[itemBody](itembody.md)|Feedback.|

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
  "feedbackDateTime": "String",
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


