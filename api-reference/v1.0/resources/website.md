---
title: tipo de recurso site
description: Representa um site.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f6d630a2cde87415cb8229f7d320cb32bc6260d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446734"
---
# <a name="website-resource-type"></a><span data-ttu-id="22b61-103">tipo de recurso site</span><span class="sxs-lookup"><span data-stu-id="22b61-103">website resource type</span></span>

<span data-ttu-id="22b61-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="22b61-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22b61-105">Representa um site.</span><span class="sxs-lookup"><span data-stu-id="22b61-105">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="22b61-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22b61-106">Properties</span></span>
| <span data-ttu-id="22b61-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22b61-107">Property</span></span>     | <span data-ttu-id="22b61-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="22b61-108">Type</span></span>   |<span data-ttu-id="22b61-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="22b61-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22b61-110">type</span><span class="sxs-lookup"><span data-stu-id="22b61-110">type</span></span>|<span data-ttu-id="22b61-111">websiteType</span><span class="sxs-lookup"><span data-stu-id="22b61-111">websiteType</span></span>| <span data-ttu-id="22b61-112">Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="22b61-112">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="22b61-113">address</span><span class="sxs-lookup"><span data-stu-id="22b61-113">address</span></span>|<span data-ttu-id="22b61-114">string</span><span class="sxs-lookup"><span data-stu-id="22b61-114">string</span></span>|<span data-ttu-id="22b61-115">A URL do site.</span><span class="sxs-lookup"><span data-stu-id="22b61-115">The URL of the website.</span></span>|
|<span data-ttu-id="22b61-116">displayName</span><span class="sxs-lookup"><span data-stu-id="22b61-116">displayName</span></span>|<span data-ttu-id="22b61-117">string</span><span class="sxs-lookup"><span data-stu-id="22b61-117">string</span></span>|<span data-ttu-id="22b61-118">O nome de exibição do site da Web.</span><span class="sxs-lookup"><span data-stu-id="22b61-118">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22b61-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22b61-119">JSON representation</span></span>

<span data-ttu-id="22b61-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22b61-120">The following is a JSON representation of the resource.</span></span>

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
