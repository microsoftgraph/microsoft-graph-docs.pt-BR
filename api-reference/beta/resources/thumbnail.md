---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Miniatura
ms.openlocfilehash: 8e56612185028891cf380d3240c999af78ff4740
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036644"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="4ab6f-102">Tipo de recurso thumbnail</span><span class="sxs-lookup"><span data-stu-id="4ab6f-102">Thumbnail resource type</span></span>

> <span data-ttu-id="4ab6f-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4ab6f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ab6f-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4ab6f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ab6f-105">O tipo de recurso **thumbnail** representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.</span><span class="sxs-lookup"><span data-stu-id="4ab6f-105">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ab6f-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ab6f-106">JSON representation</span></span>

<span data-ttu-id="4ab6f-107">Veja a seguir uma representação JSON de um recurso **thumbnail**.</span><span class="sxs-lookup"><span data-stu-id="4ab6f-107">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="4ab6f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ab6f-108">Properties</span></span>

| <span data-ttu-id="4ab6f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ab6f-109">Property</span></span>     | <span data-ttu-id="4ab6f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ab6f-110">Type</span></span>   | <span data-ttu-id="4ab6f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ab6f-111">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="4ab6f-112">height</span><span class="sxs-lookup"><span data-stu-id="4ab6f-112">height</span></span>       | <span data-ttu-id="4ab6f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab6f-113">Int32</span></span>  | <span data-ttu-id="4ab6f-114">A altura da miniatura em pixels.</span><span class="sxs-lookup"><span data-stu-id="4ab6f-114">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="4ab6f-115">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="4ab6f-115">sourceItemId</span></span> | <span data-ttu-id="4ab6f-116">String</span><span class="sxs-lookup"><span data-stu-id="4ab6f-116">String</span></span> | <span data-ttu-id="4ab6f-p102">O identificador exclusivo do item que disponibilizou a miniatura. Só estará disponível quando for solicitada uma miniatura da pasta.</span><span class="sxs-lookup"><span data-stu-id="4ab6f-p102">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="4ab6f-119">url</span><span class="sxs-lookup"><span data-stu-id="4ab6f-119">url</span></span>          | <span data-ttu-id="4ab6f-120">String</span><span class="sxs-lookup"><span data-stu-id="4ab6f-120">String</span></span> | <span data-ttu-id="4ab6f-121">A URL usada para buscar o conteúdo da miniatura.</span><span class="sxs-lookup"><span data-stu-id="4ab6f-121">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="4ab6f-122">width</span><span class="sxs-lookup"><span data-stu-id="4ab6f-122">width</span></span>        | <span data-ttu-id="4ab6f-123">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab6f-123">Int32</span></span>  | <span data-ttu-id="4ab6f-124">A largura da miniatura em pixels.</span><span class="sxs-lookup"><span data-stu-id="4ab6f-124">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="4ab6f-125">Relações</span><span class="sxs-lookup"><span data-stu-id="4ab6f-125">Relationships</span></span>

| <span data-ttu-id="4ab6f-126">Nome</span><span class="sxs-lookup"><span data-stu-id="4ab6f-126">Name</span></span>    | <span data-ttu-id="4ab6f-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ab6f-127">Type</span></span>   | <span data-ttu-id="4ab6f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ab6f-128">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="4ab6f-129">content</span><span class="sxs-lookup"><span data-stu-id="4ab6f-129">content</span></span> | <span data-ttu-id="4ab6f-130">Fluxo</span><span class="sxs-lookup"><span data-stu-id="4ab6f-130">Stream</span></span> | <span data-ttu-id="4ab6f-131">O fluxo de conteúdo da miniatura.</span><span class="sxs-lookup"><span data-stu-id="4ab6f-131">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
