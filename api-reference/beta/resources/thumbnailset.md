---
author: JeremyKelley
description: O recurso ThumbnailSet é uma coleção com chave dos recursos thumbnail.
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: bb8c286cd8c3827317edc9a24e4d14dbe963a05d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964341"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="4dea5-103">Tipo de recurso ThumbnailSet</span><span class="sxs-lookup"><span data-stu-id="4dea5-103">ThumbnailSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dea5-p101">O recurso **ThumbnailSet** é uma coleção com chave dos recursos [thumbnail](thumbnail.md). Ele é usado para representar um conjunto de miniaturas associado a um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="4dea5-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4dea5-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4dea5-106">JSON representation</span></span>

<span data-ttu-id="4dea5-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4dea5-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="4dea5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4dea5-108">Properties</span></span>

| <span data-ttu-id="4dea5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4dea5-109">Property</span></span> | <span data-ttu-id="4dea5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4dea5-110">Type</span></span>                      | <span data-ttu-id="4dea5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dea5-111">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="4dea5-112">id</span><span class="sxs-lookup"><span data-stu-id="4dea5-112">id</span></span>       | <span data-ttu-id="4dea5-113">String</span><span class="sxs-lookup"><span data-stu-id="4dea5-113">String</span></span>                    | <span data-ttu-id="4dea5-p102">A id de dentro do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4dea5-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="4dea5-116">large</span><span class="sxs-lookup"><span data-stu-id="4dea5-116">large</span></span>    | [<span data-ttu-id="4dea5-117">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="4dea5-117">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="4dea5-118">Uma miniatura em escala 1920 x 1920.</span><span class="sxs-lookup"><span data-stu-id="4dea5-118">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="4dea5-119">medium</span><span class="sxs-lookup"><span data-stu-id="4dea5-119">medium</span></span>   | [<span data-ttu-id="4dea5-120">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="4dea5-120">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="4dea5-121">Uma miniatura em escala 176 x 176.</span><span class="sxs-lookup"><span data-stu-id="4dea5-121">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="4dea5-122">small</span><span class="sxs-lookup"><span data-stu-id="4dea5-122">small</span></span>    | [<span data-ttu-id="4dea5-123">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="4dea5-123">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="4dea5-124">Uma miniatura cortada em 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="4dea5-124">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="4dea5-125">source</span><span class="sxs-lookup"><span data-stu-id="4dea5-125">source</span></span>   | [<span data-ttu-id="4dea5-126">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="4dea5-126">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="4dea5-127">Uma imagem em miniatura personalizada ou a imagem original usada para gerar outras miniaturas.</span><span class="sxs-lookup"><span data-stu-id="4dea5-127">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet",
  "suppressions": []
}
-->
