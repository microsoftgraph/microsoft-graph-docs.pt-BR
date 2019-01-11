---
title: tipo de recurso site
description: Representa um site da web.
localization_priority: Normal
ms.openlocfilehash: 15cc926ad1c251fd169ccdb0b1374df7f434a645
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826114"
---
# <a name="website-resource-type"></a><span data-ttu-id="918e4-103">tipo de recurso site</span><span class="sxs-lookup"><span data-stu-id="918e4-103">website resource type</span></span>

> <span data-ttu-id="918e4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="918e4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="918e4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="918e4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="918e4-106">Representa um site da web.</span><span class="sxs-lookup"><span data-stu-id="918e4-106">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="918e4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="918e4-107">Properties</span></span>
| <span data-ttu-id="918e4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="918e4-108">Property</span></span>     | <span data-ttu-id="918e4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="918e4-109">Type</span></span>   |<span data-ttu-id="918e4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="918e4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="918e4-111">type</span><span class="sxs-lookup"><span data-stu-id="918e4-111">type</span></span>|<span data-ttu-id="918e4-112">String</span><span class="sxs-lookup"><span data-stu-id="918e4-112">String</span></span>| <span data-ttu-id="918e4-113">Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="918e4-113">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="918e4-114">endereço</span><span class="sxs-lookup"><span data-stu-id="918e4-114">address</span></span>|<span data-ttu-id="918e4-115">string</span><span class="sxs-lookup"><span data-stu-id="918e4-115">string</span></span>|<span data-ttu-id="918e4-116">A URL do site.</span><span class="sxs-lookup"><span data-stu-id="918e4-116">The URL of the website.</span></span>|
|<span data-ttu-id="918e4-117">displayName</span><span class="sxs-lookup"><span data-stu-id="918e4-117">displayName</span></span>|<span data-ttu-id="918e4-118">string</span><span class="sxs-lookup"><span data-stu-id="918e4-118">string</span></span>|<span data-ttu-id="918e4-119">O nome de exibição do site da Web.</span><span class="sxs-lookup"><span data-stu-id="918e4-119">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="918e4-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="918e4-120">JSON representation</span></span>

<span data-ttu-id="918e4-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="918e4-121">Here is a JSON representation of the resource.</span></span>

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
