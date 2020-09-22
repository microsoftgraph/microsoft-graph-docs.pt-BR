---
title: tipo de recurso site
description: Representa um site.
localization_priority: Normal
author: AAmatino
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fbdb96a9a19a9edef98d73916dcbd01dd6ba9e66
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015236"
---
# <a name="website-resource-type"></a><span data-ttu-id="cd163-103">tipo de recurso site</span><span class="sxs-lookup"><span data-stu-id="cd163-103">website resource type</span></span>

<span data-ttu-id="cd163-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd163-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd163-105">Representa um site.</span><span class="sxs-lookup"><span data-stu-id="cd163-105">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="cd163-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd163-106">Properties</span></span>
| <span data-ttu-id="cd163-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd163-107">Property</span></span>     | <span data-ttu-id="cd163-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd163-108">Type</span></span>   |<span data-ttu-id="cd163-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd163-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd163-110">type</span><span class="sxs-lookup"><span data-stu-id="cd163-110">type</span></span>|<span data-ttu-id="cd163-111">websiteType</span><span class="sxs-lookup"><span data-stu-id="cd163-111">websiteType</span></span>| <span data-ttu-id="cd163-112">Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="cd163-112">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="cd163-113">address</span><span class="sxs-lookup"><span data-stu-id="cd163-113">address</span></span>|<span data-ttu-id="cd163-114">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd163-114">string</span></span>|<span data-ttu-id="cd163-115">A URL do site.</span><span class="sxs-lookup"><span data-stu-id="cd163-115">The URL of the website.</span></span>|
|<span data-ttu-id="cd163-116">displayName</span><span class="sxs-lookup"><span data-stu-id="cd163-116">displayName</span></span>|<span data-ttu-id="cd163-117">string</span><span class="sxs-lookup"><span data-stu-id="cd163-117">string</span></span>|<span data-ttu-id="cd163-118">O nome de exibição do site da Web.</span><span class="sxs-lookup"><span data-stu-id="cd163-118">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd163-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd163-119">JSON representation</span></span>

<span data-ttu-id="cd163-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd163-120">The following is a JSON representation of the resource.</span></span>

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

