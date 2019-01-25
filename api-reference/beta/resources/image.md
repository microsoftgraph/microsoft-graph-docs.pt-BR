---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
localization_priority: Normal
ms.openlocfilehash: 588f5185cba3012ce3dce77a9707aa23be2bf0cc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513925"
---
# <a name="image-resource-type"></a><span data-ttu-id="81c66-102">Tipo de recurso Image</span><span class="sxs-lookup"><span data-stu-id="81c66-102">Image resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81c66-p101">O recurso **Image** agrupa propriedades relacionadas a imagens em uma única estrutura. Se um [**DriveItem**](driveitem.md) tiver uma faceta **image** não nula, o item representa uma imagem bitmap.</span><span class="sxs-lookup"><span data-stu-id="81c66-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="81c66-105">**Observação:** se o serviço não puder determinar a largura e a altura da imagem, o recurso **Image** poderá ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="81c66-105">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="81c66-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81c66-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="81c66-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81c66-107">Properties</span></span>

| <span data-ttu-id="81c66-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81c66-108">Property</span></span>   | <span data-ttu-id="81c66-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="81c66-109">Type</span></span>  | <span data-ttu-id="81c66-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="81c66-110">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="81c66-111">**height**</span><span class="sxs-lookup"><span data-stu-id="81c66-111">**height**</span></span> | <span data-ttu-id="81c66-112">Int32</span><span class="sxs-lookup"><span data-stu-id="81c66-112">Int32</span></span> | <span data-ttu-id="81c66-p102">Opcional. A altura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81c66-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="81c66-116">**width**</span><span class="sxs-lookup"><span data-stu-id="81c66-116">**width**</span></span>  | <span data-ttu-id="81c66-117">Int32</span><span class="sxs-lookup"><span data-stu-id="81c66-117">Int32</span></span> | <span data-ttu-id="81c66-p103">Opcional. A largura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81c66-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="81c66-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="81c66-121">Remarks</span></span>

<span data-ttu-id="81c66-122">No OneDrive for Business, esse recurso retorna em itens que devem ser imagens com base na extensão de arquivo.</span><span class="sxs-lookup"><span data-stu-id="81c66-122">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="81c66-123">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="81c66-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image",
  "suppressions": [
    "Error: /api-reference/beta/resources/image.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
