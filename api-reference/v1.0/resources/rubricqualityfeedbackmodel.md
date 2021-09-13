---
title: Tipo de recurso rubricQualityFeedbackModel
description: Comentários relacionados a uma qualidade específica de um educationRubric.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0ca3a8877573751187f251b0a179498c44c0add8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117750"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a>Tipo de recurso rubricQualityFeedbackModel

Namespace: microsoft.graph

Comentários relacionados a uma qualidade [específica](rubricquality.md) de [um educationRubric](educationrubric.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|comentários|[itemBody](itembody.md)|Comentários específicos para uma qualidade dessa rubrica.|
|qualityId|Cadeia de caracteres|A ID da [rubricQuality](rubricquality.md) à que esse feedback está relacionado.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualityFeedbackModel",
  "baseType": null
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.itemBody"},
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualityFeedbackModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

