---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
ms.openlocfilehash: 2ba45363b684142b91aac62d4b2a5b0d371d6b3d
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23270808"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="71a21-102">Tipo de recurso ThumbnailSet</span><span class="sxs-lookup"><span data-stu-id="71a21-102">ThumbnailSet resource type</span></span>

<span data-ttu-id="71a21-p101">O recurso **ThumbnailSet** é uma coleção com chave dos recursos [thumbnail](thumbnail.md). Ele é usado para representar um conjunto de miniaturas associado a um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="71a21-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="71a21-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71a21-105">JSON representation</span></span>

<span data-ttu-id="71a21-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71a21-106">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "source",
    "small",
    "medium",
    "large"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.thumbnailSet",
  "openType": true
}-->

```json
{
  "id": "string (identifier)",
  "large": { "@odata.type": "microsoft.graph.thumbnail" },
  "medium": { "@odata.type": "microsoft.graph.thumbnail" },
  "small": { "@odata.type": "microsoft.graph.thumbnail" },
  "source": { "@odata.type": "microsoft.graph.thumbnail" }
}
```

## <a name="properties"></a><span data-ttu-id="71a21-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71a21-107">Properties</span></span>

| <span data-ttu-id="71a21-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71a21-108">Property</span></span> | <span data-ttu-id="71a21-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="71a21-109">Type</span></span>                      | <span data-ttu-id="71a21-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="71a21-110">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="71a21-111">id</span><span class="sxs-lookup"><span data-stu-id="71a21-111">id</span></span>       | <span data-ttu-id="71a21-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71a21-112">String</span></span>                    | <span data-ttu-id="71a21-p102">A id de dentro do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71a21-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="71a21-115">large</span><span class="sxs-lookup"><span data-stu-id="71a21-115">large</span></span>    | [<span data-ttu-id="71a21-116">Miniatura</span><span class="sxs-lookup"><span data-stu-id="71a21-116">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="71a21-117">Uma miniatura em escala 1920 x 1920.</span><span class="sxs-lookup"><span data-stu-id="71a21-117">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="71a21-118">medium</span><span class="sxs-lookup"><span data-stu-id="71a21-118">medium</span></span>   | [<span data-ttu-id="71a21-119">Miniatura</span><span class="sxs-lookup"><span data-stu-id="71a21-119">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="71a21-120">Uma miniatura em escala 176 x 176.</span><span class="sxs-lookup"><span data-stu-id="71a21-120">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="71a21-121">small</span><span class="sxs-lookup"><span data-stu-id="71a21-121">small</span></span>    | [<span data-ttu-id="71a21-122">Miniatura</span><span class="sxs-lookup"><span data-stu-id="71a21-122">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="71a21-123">Uma miniatura cortada em 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="71a21-123">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="71a21-124">source</span><span class="sxs-lookup"><span data-stu-id="71a21-124">source</span></span>   | [<span data-ttu-id="71a21-125">Miniatura</span><span class="sxs-lookup"><span data-stu-id="71a21-125">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="71a21-126">Uma imagem em miniatura personalizada ou a imagem original usada para gerar outras miniaturas.</span><span class="sxs-lookup"><span data-stu-id="71a21-126">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
