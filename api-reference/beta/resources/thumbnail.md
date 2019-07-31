---
author: JeremyKelley
description: O tipo de recurso thumbnail representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.
ms.date: 09/10/2017
title: Thumbnail
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 752d46f1c8a769f9f571fd13d940586fda653a58
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007659"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="c2f51-103">Tipo de recurso thumbnail</span><span class="sxs-lookup"><span data-stu-id="c2f51-103">Thumbnail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2f51-104">O tipo de recurso **thumbnail** representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.</span><span class="sxs-lookup"><span data-stu-id="c2f51-104">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2f51-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2f51-105">JSON representation</span></span>

<span data-ttu-id="c2f51-106">Veja a seguir uma representação JSON de um recurso **thumbnail**.</span><span class="sxs-lookup"><span data-stu-id="c2f51-106">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c2f51-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2f51-107">Properties</span></span>

| <span data-ttu-id="c2f51-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2f51-108">Property</span></span>     | <span data-ttu-id="c2f51-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2f51-109">Type</span></span>   | <span data-ttu-id="c2f51-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2f51-110">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c2f51-111">height</span><span class="sxs-lookup"><span data-stu-id="c2f51-111">height</span></span>       | <span data-ttu-id="c2f51-112">Int32</span><span class="sxs-lookup"><span data-stu-id="c2f51-112">Int32</span></span>  | <span data-ttu-id="c2f51-113">A altura da miniatura em pixels.</span><span class="sxs-lookup"><span data-stu-id="c2f51-113">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="c2f51-114">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="c2f51-114">sourceItemId</span></span> | <span data-ttu-id="c2f51-115">String</span><span class="sxs-lookup"><span data-stu-id="c2f51-115">String</span></span> | <span data-ttu-id="c2f51-p101">O identificador exclusivo do item que disponibilizou a miniatura. Só estará disponível quando for solicitada uma miniatura da pasta.</span><span class="sxs-lookup"><span data-stu-id="c2f51-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="c2f51-118">url</span><span class="sxs-lookup"><span data-stu-id="c2f51-118">url</span></span>          | <span data-ttu-id="c2f51-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2f51-119">String</span></span> | <span data-ttu-id="c2f51-120">A URL usada para buscar o conteúdo da miniatura.</span><span class="sxs-lookup"><span data-stu-id="c2f51-120">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="c2f51-121">width</span><span class="sxs-lookup"><span data-stu-id="c2f51-121">width</span></span>        | <span data-ttu-id="c2f51-122">Int32</span><span class="sxs-lookup"><span data-stu-id="c2f51-122">Int32</span></span>  | <span data-ttu-id="c2f51-123">A largura da miniatura em pixels.</span><span class="sxs-lookup"><span data-stu-id="c2f51-123">The width of the thumbnail, in pixels.</span></span>                                                                                      |
| <span data-ttu-id="c2f51-124">conteúdo</span><span class="sxs-lookup"><span data-stu-id="c2f51-124">content</span></span> | <span data-ttu-id="c2f51-125">Fluxo</span><span class="sxs-lookup"><span data-stu-id="c2f51-125">Stream</span></span> | <span data-ttu-id="c2f51-126">O fluxo de conteúdo da miniatura.</span><span class="sxs-lookup"><span data-stu-id="c2f51-126">The content stream for the thumbnail.</span></span> |


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
