---
title: tipo de recurso resourceReference
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c75eab84dea4e0f9134185fd9679770369073bf4
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844335"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="d5c79-103">tipo de recurso resourceReference</span><span class="sxs-lookup"><span data-stu-id="d5c79-103">resourceReference resource type</span></span>

<span data-ttu-id="d5c79-104">Tipo complexo contendo as propriedades de [officeGraphInsights](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="d5c79-104">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5c79-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5c79-105">JSON representation</span></span>

<span data-ttu-id="d5c79-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d5c79-106">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="d5c79-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5c79-107">Properties</span></span>

| <span data-ttu-id="d5c79-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5c79-108">Property</span></span>      | <span data-ttu-id="d5c79-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5c79-109">Type</span></span>      | <span data-ttu-id="d5c79-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5c79-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="d5c79-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="d5c79-111">webUrl</span></span>        | <span data-ttu-id="d5c79-112">String</span><span class="sxs-lookup"><span data-stu-id="d5c79-112">String</span></span>    | <span data-ttu-id="d5c79-113">Uma URL que conduz ao item referenciado.</span><span class="sxs-lookup"><span data-stu-id="d5c79-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="d5c79-114">id</span><span class="sxs-lookup"><span data-stu-id="d5c79-114">id</span></span>            | <span data-ttu-id="d5c79-115">String</span><span class="sxs-lookup"><span data-stu-id="d5c79-115">String</span></span>    | <span data-ttu-id="d5c79-116">O identificador exclusivo do item.</span><span class="sxs-lookup"><span data-stu-id="d5c79-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="d5c79-117">type</span><span class="sxs-lookup"><span data-stu-id="d5c79-117">type</span></span>          | <span data-ttu-id="d5c79-118">String</span><span class="sxs-lookup"><span data-stu-id="d5c79-118">String</span></span>    | <span data-ttu-id="d5c79-119">Um valor String que pode ser usado para classificar o item, como "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="d5c79-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
