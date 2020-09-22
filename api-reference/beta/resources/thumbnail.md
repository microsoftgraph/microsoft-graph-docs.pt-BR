---
author: JeremyKelley
description: O tipo de recurso thumbnail representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.
ms.date: 09/10/2017
title: Thumbnail
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7a4a2254b50fd074622990db478cefdbf3cfe091
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973537"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="daccc-103">Tipo de recurso thumbnail</span><span class="sxs-lookup"><span data-stu-id="daccc-103">Thumbnail resource type</span></span>

<span data-ttu-id="daccc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daccc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daccc-105">O tipo de recurso **thumbnail** representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.</span><span class="sxs-lookup"><span data-stu-id="daccc-105">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="daccc-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="daccc-106">JSON representation</span></span>

<span data-ttu-id="daccc-107">Veja a seguir uma representação JSON de um recurso **thumbnail**.</span><span class="sxs-lookup"><span data-stu-id="daccc-107">Here is a JSON representation of the **thumbnail** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a><span data-ttu-id="daccc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="daccc-108">Properties</span></span>

| <span data-ttu-id="daccc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="daccc-109">Property</span></span>     | <span data-ttu-id="daccc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="daccc-110">Type</span></span>   | <span data-ttu-id="daccc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="daccc-111">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="daccc-112">height</span><span class="sxs-lookup"><span data-stu-id="daccc-112">height</span></span>       | <span data-ttu-id="daccc-113">Int32</span><span class="sxs-lookup"><span data-stu-id="daccc-113">Int32</span></span>  | <span data-ttu-id="daccc-114">A altura da miniatura em pixels.</span><span class="sxs-lookup"><span data-stu-id="daccc-114">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="daccc-115">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="daccc-115">sourceItemId</span></span> | <span data-ttu-id="daccc-116">String</span><span class="sxs-lookup"><span data-stu-id="daccc-116">String</span></span> | <span data-ttu-id="daccc-p101">O identificador exclusivo do item que disponibilizou a miniatura. Só estará disponível quando for solicitada uma miniatura da pasta.</span><span class="sxs-lookup"><span data-stu-id="daccc-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="daccc-119">url</span><span class="sxs-lookup"><span data-stu-id="daccc-119">url</span></span>          | <span data-ttu-id="daccc-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="daccc-120">String</span></span> | <span data-ttu-id="daccc-121">A URL usada para buscar o conteúdo da miniatura.</span><span class="sxs-lookup"><span data-stu-id="daccc-121">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="daccc-122">width</span><span class="sxs-lookup"><span data-stu-id="daccc-122">width</span></span>        | <span data-ttu-id="daccc-123">Int32</span><span class="sxs-lookup"><span data-stu-id="daccc-123">Int32</span></span>  | <span data-ttu-id="daccc-124">A largura da miniatura em pixels.</span><span class="sxs-lookup"><span data-stu-id="daccc-124">The width of the thumbnail, in pixels.</span></span>                                                                                      |
| <span data-ttu-id="daccc-125">conteúdo</span><span class="sxs-lookup"><span data-stu-id="daccc-125">content</span></span> | <span data-ttu-id="daccc-126">Fluxo</span><span class="sxs-lookup"><span data-stu-id="daccc-126">Stream</span></span> | <span data-ttu-id="daccc-127">O fluxo de conteúdo da miniatura.</span><span class="sxs-lookup"><span data-stu-id="daccc-127">The content stream for the thumbnail.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail",
  "suppressions": []
}
-->


