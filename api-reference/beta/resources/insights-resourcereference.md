---
title: tipo de recurso resourceReference
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4fa4563904472fad9fc28fa4acb10b77887b5872
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549703"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="a2730-103">tipo de recurso resourceReference</span><span class="sxs-lookup"><span data-stu-id="a2730-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2730-104">Tipo complexo contendo propriedades de [](insights.md)insights.</span><span class="sxs-lookup"><span data-stu-id="a2730-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2730-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2730-105">JSON representation</span></span>

<span data-ttu-id="a2730-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a2730-106">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="a2730-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2730-107">Properties</span></span>

| <span data-ttu-id="a2730-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2730-108">Property</span></span>      | <span data-ttu-id="a2730-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2730-109">Type</span></span>      | <span data-ttu-id="a2730-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2730-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="a2730-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="a2730-111">webUrl</span></span>        | <span data-ttu-id="a2730-112">String</span><span class="sxs-lookup"><span data-stu-id="a2730-112">String</span></span>    | <span data-ttu-id="a2730-113">Uma URL que conduz ao item referenciado.</span><span class="sxs-lookup"><span data-stu-id="a2730-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="a2730-114">id</span><span class="sxs-lookup"><span data-stu-id="a2730-114">id</span></span>            | <span data-ttu-id="a2730-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2730-115">String</span></span>    | <span data-ttu-id="a2730-116">O identificador exclusivo do item.</span><span class="sxs-lookup"><span data-stu-id="a2730-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="a2730-117">type</span><span class="sxs-lookup"><span data-stu-id="a2730-117">type</span></span>          | <span data-ttu-id="a2730-118">String</span><span class="sxs-lookup"><span data-stu-id="a2730-118">String</span></span>    | <span data-ttu-id="a2730-119">Um valor String que pode ser usado para classificar o item, como "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="a2730-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
