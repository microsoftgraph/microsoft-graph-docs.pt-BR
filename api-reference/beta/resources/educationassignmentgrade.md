---
title: tipo de recurso educationAssignmentGrade
description: " no entanto, todos os tipos de gradação (pontos, passar/falhar e assim por diante) são subclasses dessa"
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 41e981d268718a94e6b28df6b43c4c2f931b7ad2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013745"
---
# <a name="educationassignmentgrade-resource-type"></a>tipo de recurso educationAssignmentGrade

Namespace: Microsoft Graph

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


