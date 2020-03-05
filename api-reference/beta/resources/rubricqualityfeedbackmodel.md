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
# <a name="rubricqualityfeedbackmodel-resource-type"></a><span data-ttu-id="ff344-103">tipo de recurso rubricQualityFeedbackModel</span><span class="sxs-lookup"><span data-stu-id="ff344-103">rubricQualityFeedbackModel resource type</span></span>

<span data-ttu-id="ff344-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ff344-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff344-105">Comentários relacionados a uma [qualidade](rubricquality.md) específica de um [educationRubric](educationrubric.md).</span><span class="sxs-lookup"><span data-stu-id="ff344-105">Feedback related to a specific [quality](rubricquality.md) of an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ff344-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff344-106">Properties</span></span>

| <span data-ttu-id="ff344-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff344-107">Property</span></span>     | <span data-ttu-id="ff344-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff344-108">Type</span></span>        | <span data-ttu-id="ff344-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff344-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff344-110">comentários</span><span class="sxs-lookup"><span data-stu-id="ff344-110">feedback</span></span>|[<span data-ttu-id="ff344-111">itemBody</span><span class="sxs-lookup"><span data-stu-id="ff344-111">itemBody</span></span>](itembody.md)|<span data-ttu-id="ff344-112">Comentários específicos para uma qualidade desse amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="ff344-112">Specific feedback for one quality of this rubric.</span></span>|
|<span data-ttu-id="ff344-113">qualityid</span><span class="sxs-lookup"><span data-stu-id="ff344-113">qualityId</span></span>|<span data-ttu-id="ff344-114">String</span><span class="sxs-lookup"><span data-stu-id="ff344-114">String</span></span>|<span data-ttu-id="ff344-115">A ID do [rubricQuality](rubricquality.md) ao qual este comentário está relacionado.</span><span class="sxs-lookup"><span data-stu-id="ff344-115">The ID of the [rubricQuality](rubricquality.md) that this feedback is related to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff344-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff344-116">JSON representation</span></span>

<span data-ttu-id="ff344-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff344-117">The following is a JSON representation of the resource.</span></span>

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