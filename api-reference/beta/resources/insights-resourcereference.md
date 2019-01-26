---
title: tipo de recurso de resourceReference
description: Tipo complexo que contém propriedades de ideias.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 8cc7e686aebd531a25b6c1637fcf99338df09396
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572294"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="9ee21-103">tipo de recurso de resourceReference</span><span class="sxs-lookup"><span data-stu-id="9ee21-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ee21-104">Tipo complexo que contém propriedades de [ideias](insights.md).</span><span class="sxs-lookup"><span data-stu-id="9ee21-104">Complex type containing properties of [insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ee21-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ee21-105">JSON representation</span></span>

<span data-ttu-id="9ee21-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9ee21-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueLegacyExtendedProperty",
    "multiValueLegacyExtendedProperty"
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

## <a name="properties"></a><span data-ttu-id="9ee21-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ee21-107">Properties</span></span>

| <span data-ttu-id="9ee21-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ee21-108">Property</span></span>      | <span data-ttu-id="9ee21-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ee21-109">Type</span></span>      | <span data-ttu-id="9ee21-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ee21-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="9ee21-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="9ee21-111">webUrl</span></span>        | <span data-ttu-id="9ee21-112">String</span><span class="sxs-lookup"><span data-stu-id="9ee21-112">String</span></span>    | <span data-ttu-id="9ee21-113">Uma URL, levando a item referenciado.</span><span class="sxs-lookup"><span data-stu-id="9ee21-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="9ee21-114">id</span><span class="sxs-lookup"><span data-stu-id="9ee21-114">id</span></span>            | <span data-ttu-id="9ee21-115">String</span><span class="sxs-lookup"><span data-stu-id="9ee21-115">String</span></span>    | <span data-ttu-id="9ee21-116">Identificador exclusivo do item.</span><span class="sxs-lookup"><span data-stu-id="9ee21-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="9ee21-117">type</span><span class="sxs-lookup"><span data-stu-id="9ee21-117">type</span></span>          | <span data-ttu-id="9ee21-118">String</span><span class="sxs-lookup"><span data-stu-id="9ee21-118">String</span></span>    | <span data-ttu-id="9ee21-119">Um valor de cadeia de caracteres que pode ser usado para classificar o item, como "microsoft.graph.driveItem"</span><span class="sxs-lookup"><span data-stu-id="9ee21-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
