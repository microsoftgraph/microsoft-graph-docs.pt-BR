---
title: tipo de recurso site
description: Representa um site.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6a59022426392bbf3a94c6fb82b941131db3c1d8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033380"
---
# <a name="website-resource-type"></a><span data-ttu-id="196b6-103">tipo de recurso site</span><span class="sxs-lookup"><span data-stu-id="196b6-103">website resource type</span></span>

<span data-ttu-id="196b6-104">Representa um site.</span><span class="sxs-lookup"><span data-stu-id="196b6-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="196b6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="196b6-105">Properties</span></span>
| <span data-ttu-id="196b6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="196b6-106">Property</span></span>     | <span data-ttu-id="196b6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="196b6-107">Type</span></span>   |<span data-ttu-id="196b6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="196b6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="196b6-109">type</span><span class="sxs-lookup"><span data-stu-id="196b6-109">type</span></span>|<span data-ttu-id="196b6-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="196b6-110">websiteType</span></span>| <span data-ttu-id="196b6-111">Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="196b6-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="196b6-112">address</span><span class="sxs-lookup"><span data-stu-id="196b6-112">address</span></span>|<span data-ttu-id="196b6-113">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="196b6-113">string</span></span>|<span data-ttu-id="196b6-114">A URL do site.</span><span class="sxs-lookup"><span data-stu-id="196b6-114">The URL of the website.</span></span>|
|<span data-ttu-id="196b6-115">displayName</span><span class="sxs-lookup"><span data-stu-id="196b6-115">displayName</span></span>|<span data-ttu-id="196b6-116">string</span><span class="sxs-lookup"><span data-stu-id="196b6-116">string</span></span>|<span data-ttu-id="196b6-117">O nome de exibição do site da Web.</span><span class="sxs-lookup"><span data-stu-id="196b6-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="196b6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="196b6-118">JSON representation</span></span>

<span data-ttu-id="196b6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="196b6-119">The following is a JSON representation of the resource.</span></span>

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
