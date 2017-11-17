---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
ms.openlocfilehash: c8f8d9c2232b845c746a6a215c81194e97c0431d
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="73141-102">Tipo de recurso ThumbnailSet</span><span class="sxs-lookup"><span data-stu-id="73141-102">ThumbnailSet resource type</span></span>

<span data-ttu-id="73141-p101">O recurso **ThumbnailSet** é uma coleção com chave dos recursos [thumbnail](thumbnail.md). Ele é usado para representar um conjunto de miniaturas associado a um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="73141-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="73141-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73141-105">JSON representation</span></span>

<span data-ttu-id="73141-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73141-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["source", "small", "medium", "large"],
  "openType": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->

```json
{
  "id": "string (identifier)",
  "large": { "@odata.type": "microsoft.graph.thumbnail" },
  "medium": { "@odata.type": "microsoft.graph.thumbnail" },
  "small": { "@odata.type": "microsoft.graph.thumbnail" },
  "source": { "@odata.type": "microsoft.graph.thumbnail" }
}
```

## <a name="properties"></a><span data-ttu-id="73141-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73141-107">Properties</span></span>

| <span data-ttu-id="73141-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73141-108">Property</span></span> | <span data-ttu-id="73141-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="73141-109">Type</span></span>                      | <span data-ttu-id="73141-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="73141-110">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="73141-111">id</span><span class="sxs-lookup"><span data-stu-id="73141-111">id</span></span>       | <span data-ttu-id="73141-112">String</span><span class="sxs-lookup"><span data-stu-id="73141-112">String</span></span>                    | <span data-ttu-id="73141-p102">A id de dentro do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73141-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="73141-115">large</span><span class="sxs-lookup"><span data-stu-id="73141-115">large</span></span>    | [<span data-ttu-id="73141-116">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="73141-116">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="73141-117">Uma miniatura em escala 1920 x 1920.</span><span class="sxs-lookup"><span data-stu-id="73141-117">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="73141-118">medium</span><span class="sxs-lookup"><span data-stu-id="73141-118">medium</span></span>   | [<span data-ttu-id="73141-119">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="73141-119">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="73141-120">Uma miniatura em escala 176 x 176.</span><span class="sxs-lookup"><span data-stu-id="73141-120">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="73141-121">small</span><span class="sxs-lookup"><span data-stu-id="73141-121">small</span></span>    | [<span data-ttu-id="73141-122">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="73141-122">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="73141-123">Uma miniatura cortada em 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="73141-123">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="73141-124">source</span><span class="sxs-lookup"><span data-stu-id="73141-124">source</span></span>   | [<span data-ttu-id="73141-125">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="73141-125">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="73141-126">Uma imagem em miniatura personalizada ou a imagem original usada para gerar outras miniaturas.</span><span class="sxs-lookup"><span data-stu-id="73141-126">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
