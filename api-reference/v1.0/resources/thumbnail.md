---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Miniatura
ms.openlocfilehash: ff111f44101bb03b3d8475e2567d6e1b2b4a753d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004361"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="f5fb1-102">Tipo de recurso thumbnail</span><span class="sxs-lookup"><span data-stu-id="f5fb1-102">Thumbnail resource type</span></span>

<span data-ttu-id="f5fb1-103">O tipo de recurso **thumbnail** representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.</span><span class="sxs-lookup"><span data-stu-id="f5fb1-103">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5fb1-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5fb1-104">JSON representation</span></span>

<span data-ttu-id="f5fb1-105">Veja a seguir uma representação JSON de um recurso **thumbnail**.</span><span class="sxs-lookup"><span data-stu-id="f5fb1-105">Here is a JSON representation of the **thumbnail** resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "content",
    "height",
    "width",
    "sourceItemId"
  ],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,
  "content": "stream"
}
```

## <a name="properties"></a><span data-ttu-id="f5fb1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5fb1-106">Properties</span></span>

| <span data-ttu-id="f5fb1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5fb1-107">Property</span></span>     | <span data-ttu-id="f5fb1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5fb1-108">Type</span></span>   | <span data-ttu-id="f5fb1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5fb1-109">Description</span></span>
| :----------- | :----- | :----------------------------------------------------
| <span data-ttu-id="f5fb1-110">height</span><span class="sxs-lookup"><span data-stu-id="f5fb1-110">height</span></span>       | <span data-ttu-id="f5fb1-111">Int32</span><span class="sxs-lookup"><span data-stu-id="f5fb1-111">Int32</span></span>  | <span data-ttu-id="f5fb1-112">A altura da miniatura em pixels.</span><span class="sxs-lookup"><span data-stu-id="f5fb1-112">The height of the thumbnail, in pixels.</span></span>
| <span data-ttu-id="f5fb1-113">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="f5fb1-113">sourceItemId</span></span> | <span data-ttu-id="f5fb1-114">String</span><span class="sxs-lookup"><span data-stu-id="f5fb1-114">String</span></span> | <span data-ttu-id="f5fb1-p101">O identificador exclusivo do item que disponibilizou a miniatura. Só estará disponível quando for solicitada uma miniatura da pasta.</span><span class="sxs-lookup"><span data-stu-id="f5fb1-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span>
| <span data-ttu-id="f5fb1-117">url</span><span class="sxs-lookup"><span data-stu-id="f5fb1-117">url</span></span>          | <span data-ttu-id="f5fb1-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5fb1-118">String</span></span> | <span data-ttu-id="f5fb1-119">A URL usada para buscar o conteúdo da miniatura.</span><span class="sxs-lookup"><span data-stu-id="f5fb1-119">The URL used to fetch the thumbnail content.</span></span>
| <span data-ttu-id="f5fb1-120">width</span><span class="sxs-lookup"><span data-stu-id="f5fb1-120">width</span></span>        | <span data-ttu-id="f5fb1-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f5fb1-121">Int32</span></span>  | <span data-ttu-id="f5fb1-122">A largura da miniatura em pixels.</span><span class="sxs-lookup"><span data-stu-id="f5fb1-122">The width of the thumbnail, in pixels.</span></span>
| <span data-ttu-id="f5fb1-123">content</span><span class="sxs-lookup"><span data-stu-id="f5fb1-123">content</span></span>      | <span data-ttu-id="f5fb1-124">Fluxo</span><span class="sxs-lookup"><span data-stu-id="f5fb1-124">Stream</span></span> | <span data-ttu-id="f5fb1-125">O fluxo de conteúdo da miniatura.</span><span class="sxs-lookup"><span data-stu-id="f5fb1-125">The content stream for the thumbnail.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
