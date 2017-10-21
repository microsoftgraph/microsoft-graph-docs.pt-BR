---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Miniatura
ms.openlocfilehash: 065c6ae7bbd4f6aca3172afd4399f0a1b5ff3d25
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="6180f-102">Tipo de recurso thumbnail</span><span class="sxs-lookup"><span data-stu-id="6180f-102">Thumbnail resource type</span></span>

<span data-ttu-id="6180f-103">O tipo de recurso **thumbnail** representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.</span><span class="sxs-lookup"><span data-stu-id="6180f-103">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6180f-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6180f-104">JSON representation</span></span>

<span data-ttu-id="6180f-105">Veja a seguir uma representação JSON de um recurso **thumbnail**.</span><span class="sxs-lookup"><span data-stu-id="6180f-105">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6180f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6180f-106">Properties</span></span>

| <span data-ttu-id="6180f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6180f-107">Property</span></span>     | <span data-ttu-id="6180f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6180f-108">Type</span></span>   | <span data-ttu-id="6180f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6180f-109">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6180f-110">height</span><span class="sxs-lookup"><span data-stu-id="6180f-110">height</span></span>       | <span data-ttu-id="6180f-111">Int32</span><span class="sxs-lookup"><span data-stu-id="6180f-111">Int32</span></span>  | <span data-ttu-id="6180f-112">A altura da miniatura em pixels.</span><span class="sxs-lookup"><span data-stu-id="6180f-112">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="6180f-113">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="6180f-113">sourceItemId</span></span> | <span data-ttu-id="6180f-114">String</span><span class="sxs-lookup"><span data-stu-id="6180f-114">String</span></span> | <span data-ttu-id="6180f-p101">O identificador exclusivo do item que disponibilizou a miniatura. Só estará disponível quando for solicitada uma miniatura da pasta.</span><span class="sxs-lookup"><span data-stu-id="6180f-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="6180f-117">url</span><span class="sxs-lookup"><span data-stu-id="6180f-117">url</span></span>          | <span data-ttu-id="6180f-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6180f-118">String</span></span> | <span data-ttu-id="6180f-119">A URL usada para buscar o conteúdo da miniatura.</span><span class="sxs-lookup"><span data-stu-id="6180f-119">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="6180f-120">width</span><span class="sxs-lookup"><span data-stu-id="6180f-120">width</span></span>        | <span data-ttu-id="6180f-121">Int32</span><span class="sxs-lookup"><span data-stu-id="6180f-121">Int32</span></span>  | <span data-ttu-id="6180f-122">A largura da miniatura em pixels.</span><span class="sxs-lookup"><span data-stu-id="6180f-122">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="6180f-123">Relações</span><span class="sxs-lookup"><span data-stu-id="6180f-123">Relationships</span></span>

| <span data-ttu-id="6180f-124">Nome</span><span class="sxs-lookup"><span data-stu-id="6180f-124">Name</span></span>    | <span data-ttu-id="6180f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="6180f-125">Type</span></span>   | <span data-ttu-id="6180f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6180f-126">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="6180f-127">content</span><span class="sxs-lookup"><span data-stu-id="6180f-127">content</span></span> | <span data-ttu-id="6180f-128">Fluxo</span><span class="sxs-lookup"><span data-stu-id="6180f-128">Stream</span></span> | <span data-ttu-id="6180f-129">O fluxo de conteúdo da miniatura.</span><span class="sxs-lookup"><span data-stu-id="6180f-129">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
