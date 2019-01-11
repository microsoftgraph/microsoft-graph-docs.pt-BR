---
title: tipo de recurso site
description: Representa um site.
localization_priority: Normal
ms.openlocfilehash: 1ffbee8a67527aac97bb4f60b7f8b1637ba1ebe5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851363"
---
# <a name="website-resource-type"></a><span data-ttu-id="b1104-103">tipo de recurso site</span><span class="sxs-lookup"><span data-stu-id="b1104-103">website resource type</span></span>

<span data-ttu-id="b1104-104">Representa um site.</span><span class="sxs-lookup"><span data-stu-id="b1104-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="b1104-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1104-105">Properties</span></span>
| <span data-ttu-id="b1104-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1104-106">Property</span></span>     | <span data-ttu-id="b1104-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1104-107">Type</span></span>   |<span data-ttu-id="b1104-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1104-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1104-109">type</span><span class="sxs-lookup"><span data-stu-id="b1104-109">type</span></span>|<span data-ttu-id="b1104-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="b1104-110">websiteType</span></span>| <span data-ttu-id="b1104-111">Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="b1104-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="b1104-112">address</span><span class="sxs-lookup"><span data-stu-id="b1104-112">address</span></span>|<span data-ttu-id="b1104-113">string</span><span class="sxs-lookup"><span data-stu-id="b1104-113">string</span></span>|<span data-ttu-id="b1104-114">A URL do site.</span><span class="sxs-lookup"><span data-stu-id="b1104-114">The URL of the website.</span></span>|
|<span data-ttu-id="b1104-115">displayName</span><span class="sxs-lookup"><span data-stu-id="b1104-115">displayName</span></span>|<span data-ttu-id="b1104-116">string</span><span class="sxs-lookup"><span data-stu-id="b1104-116">string</span></span>|<span data-ttu-id="b1104-117">O nome de exibição do site da Web.</span><span class="sxs-lookup"><span data-stu-id="b1104-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1104-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1104-118">JSON representation</span></span>

<span data-ttu-id="b1104-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1104-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
