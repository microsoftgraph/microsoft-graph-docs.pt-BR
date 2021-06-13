---
title: Tipo de recurso educationAssignmentGrade
description: Representa o **objeto Grade** em um Envio.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 39b415fd459b832ac3a7bfb2d66daf32d584d634
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911337"
---
# <a name="educationassignmentgrade-resource-type"></a>Tipo de recurso educationAssignmentGrade

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o **objeto Grade** em um Envio. 

Esse é um tipo abstrato que nunca será instaurou; no entanto, todos os tipos de classificação (pontos, passagem/falha e assim por diante) são subclasses desse tipo de recurso. Esse objeto também rastreia quem está fazendo a classificação. Isso é usado na **propriedade submission.grade.**


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|gradedBy|[identitySet](identityset.md)| Usuário que fez a classificação. |
|gradedDateTime|DateTimeOffset| Momento no tempo em que a nota foi aplicada a esse objeto de envio. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


