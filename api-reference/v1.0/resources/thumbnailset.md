---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: a9d92d84c8495b8c138c34f752700ccd0aad64fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457015"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="ea481-102">Tipo de recurso ThumbnailSet</span><span class="sxs-lookup"><span data-stu-id="ea481-102">ThumbnailSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea481-p101">O recurso **ThumbnailSet** é uma coleção com chave dos recursos [thumbnail](thumbnail.md). Ele é usado para representar um conjunto de miniaturas associado a um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="ea481-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea481-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea481-105">JSON representation</span></span>

<span data-ttu-id="ea481-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea481-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ea481-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea481-107">Properties</span></span>

| <span data-ttu-id="ea481-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea481-108">Property</span></span> | <span data-ttu-id="ea481-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea481-109">Type</span></span>                      | <span data-ttu-id="ea481-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea481-110">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="ea481-111">id</span><span class="sxs-lookup"><span data-stu-id="ea481-111">id</span></span>       | <span data-ttu-id="ea481-112">String</span><span class="sxs-lookup"><span data-stu-id="ea481-112">String</span></span>                    | <span data-ttu-id="ea481-p102">A id de dentro do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea481-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="ea481-115">large</span><span class="sxs-lookup"><span data-stu-id="ea481-115">large</span></span>    | [<span data-ttu-id="ea481-116">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="ea481-116">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="ea481-117">Uma miniatura em escala 1920 x 1920.</span><span class="sxs-lookup"><span data-stu-id="ea481-117">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="ea481-118">medium</span><span class="sxs-lookup"><span data-stu-id="ea481-118">medium</span></span>   | [<span data-ttu-id="ea481-119">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="ea481-119">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="ea481-120">Uma miniatura em escala 176 x 176.</span><span class="sxs-lookup"><span data-stu-id="ea481-120">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="ea481-121">small</span><span class="sxs-lookup"><span data-stu-id="ea481-121">small</span></span>    | [<span data-ttu-id="ea481-122">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="ea481-122">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="ea481-123">Uma miniatura cortada em 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="ea481-123">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="ea481-124">source</span><span class="sxs-lookup"><span data-stu-id="ea481-124">source</span></span>   | [<span data-ttu-id="ea481-125">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="ea481-125">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="ea481-126">Uma imagem em miniatura personalizada ou a imagem original usada para gerar outras miniaturas.</span><span class="sxs-lookup"><span data-stu-id="ea481-126">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet",
  "suppressions": [
    "Error: /api-reference/beta/resources/thumbnailset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
