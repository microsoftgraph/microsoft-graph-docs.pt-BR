---
title: tipo de recurso site
description: Representa um site da Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: AAmatino
ms.openlocfilehash: 4c283d77119c0272aaafa964db62bb35ad747a10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973467"
---
# <a name="website-resource-type"></a><span data-ttu-id="158de-103">tipo de recurso site</span><span class="sxs-lookup"><span data-stu-id="158de-103">website resource type</span></span>

<span data-ttu-id="158de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="158de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="158de-105">Representa um site da Web.</span><span class="sxs-lookup"><span data-stu-id="158de-105">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="158de-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="158de-106">Properties</span></span>
| <span data-ttu-id="158de-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="158de-107">Property</span></span>     | <span data-ttu-id="158de-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="158de-108">Type</span></span>   |<span data-ttu-id="158de-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="158de-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="158de-110">tipo</span><span class="sxs-lookup"><span data-stu-id="158de-110">type</span></span>|<span data-ttu-id="158de-111">String</span><span class="sxs-lookup"><span data-stu-id="158de-111">String</span></span>| <span data-ttu-id="158de-112">Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="158de-112">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="158de-113">address</span><span class="sxs-lookup"><span data-stu-id="158de-113">address</span></span>|<span data-ttu-id="158de-114">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="158de-114">string</span></span>|<span data-ttu-id="158de-115">A URL do site.</span><span class="sxs-lookup"><span data-stu-id="158de-115">The URL of the website.</span></span>|
|<span data-ttu-id="158de-116">displayName</span><span class="sxs-lookup"><span data-stu-id="158de-116">displayName</span></span>|<span data-ttu-id="158de-117">string</span><span class="sxs-lookup"><span data-stu-id="158de-117">string</span></span>|<span data-ttu-id="158de-118">O nome de exibição do site da Web.</span><span class="sxs-lookup"><span data-stu-id="158de-118">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="158de-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="158de-119">JSON representation</span></span>

<span data-ttu-id="158de-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="158de-120">Here is a JSON representation of the resource.</span></span>

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


