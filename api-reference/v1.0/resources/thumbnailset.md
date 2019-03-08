---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: a9d92d84c8495b8c138c34f752700ccd0aad64fd
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480128"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="9db19-102">Tipo de recurso ThumbnailSet</span><span class="sxs-lookup"><span data-stu-id="9db19-102">ThumbnailSet resource type</span></span>

<span data-ttu-id="9db19-p101">O recurso **ThumbnailSet** é uma coleção com chave dos recursos [thumbnail](thumbnail.md). Ele é usado para representar um conjunto de miniaturas associado a um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="9db19-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9db19-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9db19-105">JSON representation</span></span>

<span data-ttu-id="9db19-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9db19-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="9db19-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9db19-107">Properties</span></span>

| <span data-ttu-id="9db19-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9db19-108">Property</span></span> | <span data-ttu-id="9db19-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9db19-109">Type</span></span>                      | <span data-ttu-id="9db19-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9db19-110">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="9db19-111">id</span><span class="sxs-lookup"><span data-stu-id="9db19-111">id</span></span>       | <span data-ttu-id="9db19-112">String</span><span class="sxs-lookup"><span data-stu-id="9db19-112">String</span></span>                    | <span data-ttu-id="9db19-p102">A id de dentro do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9db19-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="9db19-115">large</span><span class="sxs-lookup"><span data-stu-id="9db19-115">large</span></span>    | [<span data-ttu-id="9db19-116">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="9db19-116">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="9db19-117">Uma miniatura em escala 1920 x 1920.</span><span class="sxs-lookup"><span data-stu-id="9db19-117">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="9db19-118">medium</span><span class="sxs-lookup"><span data-stu-id="9db19-118">medium</span></span>   | [<span data-ttu-id="9db19-119">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="9db19-119">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="9db19-120">Uma miniatura em escala 176 x 176.</span><span class="sxs-lookup"><span data-stu-id="9db19-120">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="9db19-121">small</span><span class="sxs-lookup"><span data-stu-id="9db19-121">small</span></span>    | [<span data-ttu-id="9db19-122">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="9db19-122">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="9db19-123">Uma miniatura cortada em 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="9db19-123">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="9db19-124">source</span><span class="sxs-lookup"><span data-stu-id="9db19-124">source</span></span>   | [<span data-ttu-id="9db19-125">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="9db19-125">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="9db19-126">Uma imagem em miniatura personalizada ou a imagem original usada para gerar outras miniaturas.</span><span class="sxs-lookup"><span data-stu-id="9db19-126">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
