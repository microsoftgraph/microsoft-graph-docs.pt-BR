---
title: tipo de recurso de resourceReference
description: Tipo complexo que contém propriedades de ideias.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4fa4563904472fad9fc28fa4acb10b77887b5872
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642755"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="8abc5-103">tipo de recurso de resourceReference</span><span class="sxs-lookup"><span data-stu-id="8abc5-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8abc5-104">Tipo complexo que contém propriedades de [ideias](insights.md).</span><span class="sxs-lookup"><span data-stu-id="8abc5-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8abc5-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8abc5-105">JSON representation</span></span>

<span data-ttu-id="8abc5-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="8abc5-106">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="8abc5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8abc5-107">Properties</span></span>

| <span data-ttu-id="8abc5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8abc5-108">Property</span></span>      | <span data-ttu-id="8abc5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8abc5-109">Type</span></span>      | <span data-ttu-id="8abc5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8abc5-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="8abc5-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="8abc5-111">webUrl</span></span>        | <span data-ttu-id="8abc5-112">String</span><span class="sxs-lookup"><span data-stu-id="8abc5-112">String</span></span>    | <span data-ttu-id="8abc5-113">Uma URL, levando a item referenciado.</span><span class="sxs-lookup"><span data-stu-id="8abc5-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="8abc5-114">id</span><span class="sxs-lookup"><span data-stu-id="8abc5-114">id</span></span>            | <span data-ttu-id="8abc5-115">String</span><span class="sxs-lookup"><span data-stu-id="8abc5-115">String</span></span>    | <span data-ttu-id="8abc5-116">Identificador exclusivo do item.</span><span class="sxs-lookup"><span data-stu-id="8abc5-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="8abc5-117">type</span><span class="sxs-lookup"><span data-stu-id="8abc5-117">type</span></span>          | <span data-ttu-id="8abc5-118">String</span><span class="sxs-lookup"><span data-stu-id="8abc5-118">String</span></span>    | <span data-ttu-id="8abc5-119">Um valor de cadeia de caracteres que pode ser usado para classificar o item, como "microsoft.graph.driveItem"</span><span class="sxs-lookup"><span data-stu-id="8abc5-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
