---
title: tipo de recurso site
description: Representa um site.
ms.openlocfilehash: 14934aae418581f4c75c880be67bf51fd0bc293c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003968"
---
# <a name="website-resource-type"></a><span data-ttu-id="fcb1c-103">tipo de recurso site</span><span class="sxs-lookup"><span data-stu-id="fcb1c-103">website resource type</span></span>

<span data-ttu-id="fcb1c-104">Representa um site.</span><span class="sxs-lookup"><span data-stu-id="fcb1c-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="fcb1c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fcb1c-105">Properties</span></span>
| <span data-ttu-id="fcb1c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fcb1c-106">Property</span></span>     | <span data-ttu-id="fcb1c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcb1c-107">Type</span></span>   |<span data-ttu-id="fcb1c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcb1c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcb1c-109">type</span><span class="sxs-lookup"><span data-stu-id="fcb1c-109">type</span></span>|<span data-ttu-id="fcb1c-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="fcb1c-110">websiteType</span></span>| <span data-ttu-id="fcb1c-111">Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="fcb1c-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="fcb1c-112">address</span><span class="sxs-lookup"><span data-stu-id="fcb1c-112">address</span></span>|<span data-ttu-id="fcb1c-113">string</span><span class="sxs-lookup"><span data-stu-id="fcb1c-113">string</span></span>|<span data-ttu-id="fcb1c-114">A URL do site.</span><span class="sxs-lookup"><span data-stu-id="fcb1c-114">The URL of the website.</span></span>|
|<span data-ttu-id="fcb1c-115">displayName</span><span class="sxs-lookup"><span data-stu-id="fcb1c-115">displayName</span></span>|<span data-ttu-id="fcb1c-116">string</span><span class="sxs-lookup"><span data-stu-id="fcb1c-116">string</span></span>|<span data-ttu-id="fcb1c-117">O nome de exibição do site da Web.</span><span class="sxs-lookup"><span data-stu-id="fcb1c-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fcb1c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fcb1c-118">JSON representation</span></span>

<span data-ttu-id="fcb1c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fcb1c-119">The following is a JSON representation of the resource.</span></span>

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
