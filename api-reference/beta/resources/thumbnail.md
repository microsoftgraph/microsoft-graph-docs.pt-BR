---
author: JeremyKelley
description: O tipo de recurso thumbnail representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.
ms.date: 09/10/2017
title: Thumbnail
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 53001d2459af4dc382501e33930bc8aca55a26b2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519761"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="a1773-103">Tipo de recurso thumbnail</span><span class="sxs-lookup"><span data-stu-id="a1773-103">Thumbnail resource type</span></span>

<span data-ttu-id="a1773-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a1773-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1773-105">O tipo de recurso **thumbnail** representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.</span><span class="sxs-lookup"><span data-stu-id="a1773-105">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1773-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a1773-106">JSON representation</span></span>

<span data-ttu-id="a1773-107">Veja a seguir uma representação JSON de um recurso **thumbnail**.</span><span class="sxs-lookup"><span data-stu-id="a1773-107">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a1773-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a1773-108">Properties</span></span>

| <span data-ttu-id="a1773-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1773-109">Property</span></span>     | <span data-ttu-id="a1773-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1773-110">Type</span></span>   | <span data-ttu-id="a1773-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1773-111">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a1773-112">height</span><span class="sxs-lookup"><span data-stu-id="a1773-112">height</span></span>       | <span data-ttu-id="a1773-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a1773-113">Int32</span></span>  | <span data-ttu-id="a1773-114">A altura da miniatura em pixels.</span><span class="sxs-lookup"><span data-stu-id="a1773-114">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="a1773-115">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="a1773-115">sourceItemId</span></span> | <span data-ttu-id="a1773-116">String</span><span class="sxs-lookup"><span data-stu-id="a1773-116">String</span></span> | <span data-ttu-id="a1773-p101">O identificador exclusivo do item que disponibilizou a miniatura. Só estará disponível quando for solicitada uma miniatura da pasta.</span><span class="sxs-lookup"><span data-stu-id="a1773-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="a1773-119">url</span><span class="sxs-lookup"><span data-stu-id="a1773-119">url</span></span>          | <span data-ttu-id="a1773-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1773-120">String</span></span> | <span data-ttu-id="a1773-121">A URL usada para buscar o conteúdo da miniatura.</span><span class="sxs-lookup"><span data-stu-id="a1773-121">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="a1773-122">width</span><span class="sxs-lookup"><span data-stu-id="a1773-122">width</span></span>        | <span data-ttu-id="a1773-123">Int32</span><span class="sxs-lookup"><span data-stu-id="a1773-123">Int32</span></span>  | <span data-ttu-id="a1773-124">A largura da miniatura em pixels.</span><span class="sxs-lookup"><span data-stu-id="a1773-124">The width of the thumbnail, in pixels.</span></span>                                                                                      |
| <span data-ttu-id="a1773-125">conteúdo</span><span class="sxs-lookup"><span data-stu-id="a1773-125">content</span></span> | <span data-ttu-id="a1773-126">Fluxo</span><span class="sxs-lookup"><span data-stu-id="a1773-126">Stream</span></span> | <span data-ttu-id="a1773-127">O fluxo de conteúdo da miniatura.</span><span class="sxs-lookup"><span data-stu-id="a1773-127">The content stream for the thumbnail.</span></span> |


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
