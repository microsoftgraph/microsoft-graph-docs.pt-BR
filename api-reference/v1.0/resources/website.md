---
title: tipo de recurso site
description: Representa um site.
localization_priority: Normal
ms.openlocfilehash: 1ffbee8a67527aac97bb4f60b7f8b1637ba1ebe5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457022"
---
# <a name="website-resource-type"></a><span data-ttu-id="698c3-103">tipo de recurso site</span><span class="sxs-lookup"><span data-stu-id="698c3-103">website resource type</span></span>

<span data-ttu-id="698c3-104">Representa um site.</span><span class="sxs-lookup"><span data-stu-id="698c3-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="698c3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="698c3-105">Properties</span></span>
| <span data-ttu-id="698c3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="698c3-106">Property</span></span>     | <span data-ttu-id="698c3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="698c3-107">Type</span></span>   |<span data-ttu-id="698c3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="698c3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="698c3-109">type</span><span class="sxs-lookup"><span data-stu-id="698c3-109">type</span></span>|<span data-ttu-id="698c3-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="698c3-110">websiteType</span></span>| <span data-ttu-id="698c3-111">Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="698c3-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="698c3-112">address</span><span class="sxs-lookup"><span data-stu-id="698c3-112">address</span></span>|<span data-ttu-id="698c3-113">string</span><span class="sxs-lookup"><span data-stu-id="698c3-113">string</span></span>|<span data-ttu-id="698c3-114">A URL do site.</span><span class="sxs-lookup"><span data-stu-id="698c3-114">The URL of the website.</span></span>|
|<span data-ttu-id="698c3-115">displayName</span><span class="sxs-lookup"><span data-stu-id="698c3-115">displayName</span></span>|<span data-ttu-id="698c3-116">string</span><span class="sxs-lookup"><span data-stu-id="698c3-116">string</span></span>|<span data-ttu-id="698c3-117">O nome de exibição do site da Web.</span><span class="sxs-lookup"><span data-stu-id="698c3-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="698c3-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="698c3-118">JSON representation</span></span>

<span data-ttu-id="698c3-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="698c3-119">The following is a JSON representation of the resource.</span></span>

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
