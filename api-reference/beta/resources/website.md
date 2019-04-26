---
title: tipo de recurso site
description: Representa um site da Web.
localization_priority: Normal
ms.openlocfilehash: b44fcacf77f3b2afb5cdc9dfea2340d0a1fc1cd5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339592"
---
# <a name="website-resource-type"></a><span data-ttu-id="6c8ae-103">tipo de recurso site</span><span class="sxs-lookup"><span data-stu-id="6c8ae-103">website resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c8ae-104">Representa um site da Web.</span><span class="sxs-lookup"><span data-stu-id="6c8ae-104">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="6c8ae-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c8ae-105">Properties</span></span>
| <span data-ttu-id="6c8ae-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c8ae-106">Property</span></span>     | <span data-ttu-id="6c8ae-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c8ae-107">Type</span></span>   |<span data-ttu-id="6c8ae-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c8ae-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c8ae-109">type</span><span class="sxs-lookup"><span data-stu-id="6c8ae-109">type</span></span>|<span data-ttu-id="6c8ae-110">String</span><span class="sxs-lookup"><span data-stu-id="6c8ae-110">String</span></span>| <span data-ttu-id="6c8ae-111">Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="6c8ae-111">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="6c8ae-112">address</span><span class="sxs-lookup"><span data-stu-id="6c8ae-112">address</span></span>|<span data-ttu-id="6c8ae-113">string</span><span class="sxs-lookup"><span data-stu-id="6c8ae-113">string</span></span>|<span data-ttu-id="6c8ae-114">A URL do site.</span><span class="sxs-lookup"><span data-stu-id="6c8ae-114">The URL of the website.</span></span>|
|<span data-ttu-id="6c8ae-115">displayName</span><span class="sxs-lookup"><span data-stu-id="6c8ae-115">displayName</span></span>|<span data-ttu-id="6c8ae-116">string</span><span class="sxs-lookup"><span data-stu-id="6c8ae-116">string</span></span>|<span data-ttu-id="6c8ae-117">O nome de exibição do site da Web.</span><span class="sxs-lookup"><span data-stu-id="6c8ae-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c8ae-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c8ae-118">JSON representation</span></span>

<span data-ttu-id="6c8ae-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c8ae-119">Here is a JSON representation of the resource.</span></span>

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
