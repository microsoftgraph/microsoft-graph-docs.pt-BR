---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
localization_priority: Normal
ms.openlocfilehash: 4526b8d475b36521ee08829b50931438999ca249
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830412"
---
# <a name="image-resource-type"></a><span data-ttu-id="41815-102">Tipo de recurso Image</span><span class="sxs-lookup"><span data-stu-id="41815-102">Image resource type</span></span>

<span data-ttu-id="41815-p101">O recurso **Image** agrupa propriedades relacionadas a imagens em uma única estrutura. Se um [**DriveItem**](driveitem.md) tiver uma faceta **image** não nula, o item representa uma imagem bitmap.</span><span class="sxs-lookup"><span data-stu-id="41815-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="41815-105">**Observação:** se o serviço não puder determinar a largura e a altura da imagem, o recurso **Image** poderá ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="41815-105">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="41815-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41815-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="41815-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41815-107">Properties</span></span>

| <span data-ttu-id="41815-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41815-108">Property</span></span>   | <span data-ttu-id="41815-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="41815-109">Type</span></span>  | <span data-ttu-id="41815-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="41815-110">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="41815-111">**height**</span><span class="sxs-lookup"><span data-stu-id="41815-111">**height**</span></span> | <span data-ttu-id="41815-112">Int32</span><span class="sxs-lookup"><span data-stu-id="41815-112">Int32</span></span> | <span data-ttu-id="41815-p102">Opcional. A altura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41815-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="41815-116">**width**</span><span class="sxs-lookup"><span data-stu-id="41815-116">**width**</span></span>  | <span data-ttu-id="41815-117">Int32</span><span class="sxs-lookup"><span data-stu-id="41815-117">Int32</span></span> | <span data-ttu-id="41815-p103">Opcional. A largura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41815-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="41815-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="41815-121">Remarks</span></span>

<span data-ttu-id="41815-122">No OneDrive for Business, esse recurso retorna em itens que devem ser imagens com base na extensão de arquivo.</span><span class="sxs-lookup"><span data-stu-id="41815-122">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="41815-123">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="41815-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
