---
title: tipo de recurso rubricQualityFeedbackModel
description: Comentários relacionados a uma qualidade específica de um educationRubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 22c69292441f4b71238e820229e9d733bd9cabb9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520995"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a>tipo de recurso rubricQualityFeedbackModel

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Comentários relacionados a uma [qualidade](rubricquality.md) específica de um [educationRubric](educationrubric.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|comentários|[itemBody](itembody.md)|Comentários específicos para uma qualidade desse amostra rubric.|
|qualityid|String|A ID do [rubricQuality](rubricquality.md) ao qual este comentário está relacionado.|

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