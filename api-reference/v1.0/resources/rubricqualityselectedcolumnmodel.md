---
title: Tipo de recurso rubricQualitySelectedColumnModel
description: Indica o rubricLevel selecionado pelo professor ao classificar um educationRubric.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9e69fa26d97684db4964ffba3d268ee1d1c11b44
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911373"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a><span data-ttu-id="71112-103">Tipo de recurso rubricQualitySelectedColumnModel</span><span class="sxs-lookup"><span data-stu-id="71112-103">rubricQualitySelectedColumnModel resource type</span></span>

<span data-ttu-id="71112-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71112-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71112-105">Indica o [rubricLevel](rubriclevel.md) selecionado pelo professor ao classificar [um educationRubric](educationrubric.md).</span><span class="sxs-lookup"><span data-stu-id="71112-105">Indicates the [rubricLevel](rubriclevel.md) selected by the teacher when grading an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="71112-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71112-106">Properties</span></span>

| <span data-ttu-id="71112-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71112-107">Property</span></span>     | <span data-ttu-id="71112-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="71112-108">Type</span></span>        | <span data-ttu-id="71112-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="71112-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="71112-110">columnId</span><span class="sxs-lookup"><span data-stu-id="71112-110">columnId</span></span>|<span data-ttu-id="71112-111">String</span><span class="sxs-lookup"><span data-stu-id="71112-111">String</span></span>|<span data-ttu-id="71112-112">ID do nível selecionado para essa qualidade.</span><span class="sxs-lookup"><span data-stu-id="71112-112">ID of the selected level for this quality.</span></span>|
|<span data-ttu-id="71112-113">qualityId</span><span class="sxs-lookup"><span data-stu-id="71112-113">qualityId</span></span>|<span data-ttu-id="71112-114">String</span><span class="sxs-lookup"><span data-stu-id="71112-114">String</span></span>|<span data-ttu-id="71112-115">ID da qualidade associada.</span><span class="sxs-lookup"><span data-stu-id="71112-115">ID of the associated quality.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71112-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71112-116">JSON representation</span></span>

<span data-ttu-id="71112-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71112-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel",
  "baseType": null
}-->

```json
{
  "columnId": "String",
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualitySelectedColumnModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

