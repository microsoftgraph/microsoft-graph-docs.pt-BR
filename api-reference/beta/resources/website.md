---
title: tipo de recurso site
description: Representa um site da Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ebdfef4a8ee4e11c2993dbd97a735c6e01960b6b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519425"
---
# <a name="website-resource-type"></a><span data-ttu-id="a33d9-103">tipo de recurso site</span><span class="sxs-lookup"><span data-stu-id="a33d9-103">website resource type</span></span>

<span data-ttu-id="a33d9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a33d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a33d9-105">Representa um site da Web.</span><span class="sxs-lookup"><span data-stu-id="a33d9-105">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="a33d9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a33d9-106">Properties</span></span>
| <span data-ttu-id="a33d9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a33d9-107">Property</span></span>     | <span data-ttu-id="a33d9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a33d9-108">Type</span></span>   |<span data-ttu-id="a33d9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a33d9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a33d9-110">type</span><span class="sxs-lookup"><span data-stu-id="a33d9-110">type</span></span>|<span data-ttu-id="a33d9-111">String</span><span class="sxs-lookup"><span data-stu-id="a33d9-111">String</span></span>| <span data-ttu-id="a33d9-112">Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="a33d9-112">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="a33d9-113">address</span><span class="sxs-lookup"><span data-stu-id="a33d9-113">address</span></span>|<span data-ttu-id="a33d9-114">string</span><span class="sxs-lookup"><span data-stu-id="a33d9-114">string</span></span>|<span data-ttu-id="a33d9-115">A URL do site.</span><span class="sxs-lookup"><span data-stu-id="a33d9-115">The URL of the website.</span></span>|
|<span data-ttu-id="a33d9-116">displayName</span><span class="sxs-lookup"><span data-stu-id="a33d9-116">displayName</span></span>|<span data-ttu-id="a33d9-117">string</span><span class="sxs-lookup"><span data-stu-id="a33d9-117">string</span></span>|<span data-ttu-id="a33d9-118">O nome de exibição do site da Web.</span><span class="sxs-lookup"><span data-stu-id="a33d9-118">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a33d9-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a33d9-119">JSON representation</span></span>

<span data-ttu-id="a33d9-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a33d9-120">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
