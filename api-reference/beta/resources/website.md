---
title: tipo de recurso site
description: Representa um site da Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: AAmatino
ms.openlocfilehash: 758d802a67979c4e43aefcdb4e8a3998be15b993
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809296"
---
# <a name="website-resource-type"></a><span data-ttu-id="a7c6e-103">tipo de recurso site</span><span class="sxs-lookup"><span data-stu-id="a7c6e-103">website resource type</span></span>

<span data-ttu-id="a7c6e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7c6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7c6e-105">Representa um site da Web.</span><span class="sxs-lookup"><span data-stu-id="a7c6e-105">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="a7c6e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7c6e-106">Properties</span></span>
| <span data-ttu-id="a7c6e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7c6e-107">Property</span></span>     | <span data-ttu-id="a7c6e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7c6e-108">Type</span></span>   |<span data-ttu-id="a7c6e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7c6e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7c6e-110">type</span><span class="sxs-lookup"><span data-stu-id="a7c6e-110">type</span></span>|<span data-ttu-id="a7c6e-111">String</span><span class="sxs-lookup"><span data-stu-id="a7c6e-111">String</span></span>| <span data-ttu-id="a7c6e-112">Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="a7c6e-112">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="a7c6e-113">address</span><span class="sxs-lookup"><span data-stu-id="a7c6e-113">address</span></span>|<span data-ttu-id="a7c6e-114">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7c6e-114">string</span></span>|<span data-ttu-id="a7c6e-115">A URL do site.</span><span class="sxs-lookup"><span data-stu-id="a7c6e-115">The URL of the website.</span></span>|
|<span data-ttu-id="a7c6e-116">displayName</span><span class="sxs-lookup"><span data-stu-id="a7c6e-116">displayName</span></span>|<span data-ttu-id="a7c6e-117">string</span><span class="sxs-lookup"><span data-stu-id="a7c6e-117">string</span></span>|<span data-ttu-id="a7c6e-118">O nome de exibição do site da Web.</span><span class="sxs-lookup"><span data-stu-id="a7c6e-118">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7c6e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7c6e-119">JSON representation</span></span>

<span data-ttu-id="a7c6e-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7c6e-120">Here is a JSON representation of the resource.</span></span>

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
