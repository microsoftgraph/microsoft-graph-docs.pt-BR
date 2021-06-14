---
title: Tipo de recurso rubricQualityFeedbackModel
description: Comentários relacionados a uma qualidade específica de um educationRubric.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8f96a1fd0ce0d007c138928c316316349a7b302e
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911374"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a><span data-ttu-id="e69f1-103">Tipo de recurso rubricQualityFeedbackModel</span><span class="sxs-lookup"><span data-stu-id="e69f1-103">rubricQualityFeedbackModel resource type</span></span>

<span data-ttu-id="e69f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e69f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e69f1-105">Comentários relacionados a uma qualidade [específica](rubricquality.md) de [um educationRubric](educationrubric.md).</span><span class="sxs-lookup"><span data-stu-id="e69f1-105">Feedback related to a specific [quality](rubricquality.md) of an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e69f1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e69f1-106">Properties</span></span>

| <span data-ttu-id="e69f1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e69f1-107">Property</span></span>     | <span data-ttu-id="e69f1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e69f1-108">Type</span></span>        | <span data-ttu-id="e69f1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e69f1-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e69f1-110">comentários</span><span class="sxs-lookup"><span data-stu-id="e69f1-110">feedback</span></span>|[<span data-ttu-id="e69f1-111">itemBody</span><span class="sxs-lookup"><span data-stu-id="e69f1-111">itemBody</span></span>](itembody.md)|<span data-ttu-id="e69f1-112">Comentários específicos para uma qualidade dessa rubrica.</span><span class="sxs-lookup"><span data-stu-id="e69f1-112">Specific feedback for one quality of this rubric.</span></span>|
|<span data-ttu-id="e69f1-113">qualityId</span><span class="sxs-lookup"><span data-stu-id="e69f1-113">qualityId</span></span>|<span data-ttu-id="e69f1-114">String</span><span class="sxs-lookup"><span data-stu-id="e69f1-114">String</span></span>|<span data-ttu-id="e69f1-115">A ID da [rubricQuality](rubricquality.md) à que esse feedback está relacionado.</span><span class="sxs-lookup"><span data-stu-id="e69f1-115">The ID of the [rubricQuality](rubricquality.md) that this feedback is related to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e69f1-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e69f1-116">JSON representation</span></span>

<span data-ttu-id="e69f1-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e69f1-117">The following is a JSON representation of the resource.</span></span>

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

