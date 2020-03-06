---
title: tipo de recurso resourceReference
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: aa00eb06ac239b4f93a200e72ecbe88c99d6189c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532866"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="fbea3-103">tipo de recurso resourceReference</span><span class="sxs-lookup"><span data-stu-id="fbea3-103">resourceReference resource type</span></span>

<span data-ttu-id="fbea3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbea3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fbea3-105">Tipo complexo contendo as propriedades de [officeGraphInsights](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="fbea3-105">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbea3-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbea3-106">JSON representation</span></span>

<span data-ttu-id="fbea3-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fbea3-107">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="fbea3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbea3-108">Properties</span></span>

| <span data-ttu-id="fbea3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbea3-109">Property</span></span>      | <span data-ttu-id="fbea3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbea3-110">Type</span></span>      | <span data-ttu-id="fbea3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbea3-111">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="fbea3-112">webUrl</span><span class="sxs-lookup"><span data-stu-id="fbea3-112">webUrl</span></span>        | <span data-ttu-id="fbea3-113">String</span><span class="sxs-lookup"><span data-stu-id="fbea3-113">String</span></span>    | <span data-ttu-id="fbea3-114">Uma URL que conduz ao item referenciado.</span><span class="sxs-lookup"><span data-stu-id="fbea3-114">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="fbea3-115">id</span><span class="sxs-lookup"><span data-stu-id="fbea3-115">id</span></span>            | <span data-ttu-id="fbea3-116">String</span><span class="sxs-lookup"><span data-stu-id="fbea3-116">String</span></span>    | <span data-ttu-id="fbea3-117">O identificador exclusivo do item.</span><span class="sxs-lookup"><span data-stu-id="fbea3-117">The item's unique identifier.</span></span>           |
| <span data-ttu-id="fbea3-118">type</span><span class="sxs-lookup"><span data-stu-id="fbea3-118">type</span></span>          | <span data-ttu-id="fbea3-119">String</span><span class="sxs-lookup"><span data-stu-id="fbea3-119">String</span></span>    | <span data-ttu-id="fbea3-120">Um valor String que pode ser usado para classificar o item, como "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="fbea3-120">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
