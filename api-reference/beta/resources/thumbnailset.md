---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
ms.openlocfilehash: d88e19242ea6c271e206a4c1a582fdbbfac8877b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034366"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="85843-102">Tipo de recurso ThumbnailSet</span><span class="sxs-lookup"><span data-stu-id="85843-102">ThumbnailSet resource type</span></span>

> <span data-ttu-id="85843-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="85843-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85843-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="85843-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85843-p102">O recurso **ThumbnailSet** é uma coleção com chave dos recursos [thumbnail](thumbnail.md). Ele é usado para representar um conjunto de miniaturas associado a um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="85843-p102">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85843-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85843-107">JSON representation</span></span>

<span data-ttu-id="85843-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85843-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="85843-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85843-109">Properties</span></span>

| <span data-ttu-id="85843-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85843-110">Property</span></span> | <span data-ttu-id="85843-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="85843-111">Type</span></span>                      | <span data-ttu-id="85843-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="85843-112">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="85843-113">id</span><span class="sxs-lookup"><span data-stu-id="85843-113">id</span></span>       | <span data-ttu-id="85843-114">String</span><span class="sxs-lookup"><span data-stu-id="85843-114">String</span></span>                    | <span data-ttu-id="85843-p103">A id de dentro do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85843-p103">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="85843-117">large</span><span class="sxs-lookup"><span data-stu-id="85843-117">large</span></span>    | [<span data-ttu-id="85843-118">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="85843-118">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="85843-119">Uma miniatura em escala 1920 x 1920.</span><span class="sxs-lookup"><span data-stu-id="85843-119">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="85843-120">medium</span><span class="sxs-lookup"><span data-stu-id="85843-120">medium</span></span>   | [<span data-ttu-id="85843-121">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="85843-121">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="85843-122">Uma miniatura em escala 176 x 176.</span><span class="sxs-lookup"><span data-stu-id="85843-122">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="85843-123">small</span><span class="sxs-lookup"><span data-stu-id="85843-123">small</span></span>    | [<span data-ttu-id="85843-124">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="85843-124">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="85843-125">Uma miniatura cortada em 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="85843-125">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="85843-126">source</span><span class="sxs-lookup"><span data-stu-id="85843-126">source</span></span>   | [<span data-ttu-id="85843-127">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="85843-127">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="85843-128">Uma imagem em miniatura personalizada ou a imagem original usada para gerar outras miniaturas.</span><span class="sxs-lookup"><span data-stu-id="85843-128">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
