---
author: JeremyKelley
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
description: O recurso ThumbnailSet é uma coleção com chave dos recursos thumbnail.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5fe322d202b0c1b5735736ed6ca1d135839c3420
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239258"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="d65fa-103">Tipo de recurso ThumbnailSet</span><span class="sxs-lookup"><span data-stu-id="d65fa-103">ThumbnailSet resource type</span></span>

<span data-ttu-id="d65fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d65fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d65fa-p101">O recurso **ThumbnailSet** é uma coleção com chave dos recursos [thumbnail](thumbnail.md). Ele é usado para representar um conjunto de miniaturas associado a um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="d65fa-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d65fa-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d65fa-107">JSON representation</span></span>

<span data-ttu-id="d65fa-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d65fa-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d65fa-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d65fa-109">Properties</span></span>

| <span data-ttu-id="d65fa-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d65fa-110">Property</span></span> | <span data-ttu-id="d65fa-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d65fa-111">Type</span></span>                      | <span data-ttu-id="d65fa-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d65fa-112">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="d65fa-113">id</span><span class="sxs-lookup"><span data-stu-id="d65fa-113">id</span></span>       | <span data-ttu-id="d65fa-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d65fa-114">String</span></span>                    | <span data-ttu-id="d65fa-p102">A id de dentro do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d65fa-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="d65fa-117">large</span><span class="sxs-lookup"><span data-stu-id="d65fa-117">large</span></span>    | [<span data-ttu-id="d65fa-118">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="d65fa-118">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d65fa-119">Uma miniatura em escala 1920 x 1920.</span><span class="sxs-lookup"><span data-stu-id="d65fa-119">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="d65fa-120">medium</span><span class="sxs-lookup"><span data-stu-id="d65fa-120">medium</span></span>   | [<span data-ttu-id="d65fa-121">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="d65fa-121">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d65fa-122">Uma miniatura em escala 176 x 176.</span><span class="sxs-lookup"><span data-stu-id="d65fa-122">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="d65fa-123">small</span><span class="sxs-lookup"><span data-stu-id="d65fa-123">small</span></span>    | [<span data-ttu-id="d65fa-124">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="d65fa-124">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d65fa-125">Uma miniatura cortada em 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="d65fa-125">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="d65fa-126">source</span><span class="sxs-lookup"><span data-stu-id="d65fa-126">source</span></span>   | [<span data-ttu-id="d65fa-127">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="d65fa-127">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d65fa-128">Uma imagem em miniatura personalizada ou a imagem original usada para gerar outras miniaturas.</span><span class="sxs-lookup"><span data-stu-id="d65fa-128">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->

