---
title: tipo de recurso educationAssignmentGrade
description: " no entanto, todos os tipos de gradação (pontos, passar/falhar e assim por diante) são subclasses dessa"
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9680a298c405a81648ba0a5fe95cdf0df0c841bb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502743"
---
# <a name="educationassignmentgrade-resource-type"></a>tipo de recurso educationAssignmentGrade

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o objeto **graduação** em um envio. Este é um tipo abstrato que nunca será instanciado; no entanto, todos os tipos de gradação (pontos, passar/falhar e assim por diante) são subclasses desse tipo de recurso. Esse objeto também controla quem está fazendo a gradação. Isso é usado na propriedade **enmisse.**


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|gradedBy|[identitySet](identityset.md)| Usuário que fazia a gradação. |
|gradedDateTime|DateTimeOffset| Momento no momento em que a classificação foi aplicada a este objeto de envio. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|

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
