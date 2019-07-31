---
author: JeremyKelley
description: O recurso Image agrupa propriedades relacionadas a imagens em uma única estrutura.
ms.date: 09/10/2017
title: Image
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c41925443820b96098c03de00f4c3741da0cec95
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973510"
---
# <a name="image-resource-type"></a><span data-ttu-id="b404f-103">Tipo de recurso Image</span><span class="sxs-lookup"><span data-stu-id="b404f-103">Image resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b404f-p101">O recurso **Image** agrupa propriedades relacionadas a imagens em uma única estrutura. Se um [**DriveItem**](driveitem.md) tiver uma faceta **image** não nula, o item representa uma imagem bitmap.</span><span class="sxs-lookup"><span data-stu-id="b404f-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="b404f-106">**Observação:** se o serviço não puder determinar a largura e a altura da imagem, o recurso **Image** poderá ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="b404f-106">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b404f-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b404f-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="b404f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b404f-108">Properties</span></span>

| <span data-ttu-id="b404f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b404f-109">Property</span></span>   | <span data-ttu-id="b404f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b404f-110">Type</span></span>  | <span data-ttu-id="b404f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b404f-111">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="b404f-112">**height**</span><span class="sxs-lookup"><span data-stu-id="b404f-112">**height**</span></span> | <span data-ttu-id="b404f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b404f-113">Int32</span></span> | <span data-ttu-id="b404f-p102">Opcional. A altura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b404f-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="b404f-117">**width**</span><span class="sxs-lookup"><span data-stu-id="b404f-117">**width**</span></span>  | <span data-ttu-id="b404f-118">Int32</span><span class="sxs-lookup"><span data-stu-id="b404f-118">Int32</span></span> | <span data-ttu-id="b404f-p103">Opcional. A largura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b404f-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="b404f-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="b404f-122">Remarks</span></span>

<span data-ttu-id="b404f-123">No OneDrive for Business, esse recurso retorna em itens que devem ser imagens com base na extensão de arquivo.</span><span class="sxs-lookup"><span data-stu-id="b404f-123">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="b404f-124">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b404f-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image",
  "suppressions": []
}
-->
