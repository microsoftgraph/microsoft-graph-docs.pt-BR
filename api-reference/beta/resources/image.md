---
author: JeremyKelley
description: O recurso Image agrupa propriedades relacionadas a imagens em uma única estrutura.
ms.date: 09/10/2017
title: Imagem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: fc7f63c0e7d95c8526d4663b82552541585c9ee2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016630"
---
# <a name="image-resource-type"></a><span data-ttu-id="01953-103">Tipo de recurso Image</span><span class="sxs-lookup"><span data-stu-id="01953-103">Image resource type</span></span>

<span data-ttu-id="01953-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01953-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01953-p101">O recurso **Image** agrupa propriedades relacionadas a imagens em uma única estrutura. Se um [**DriveItem**](driveitem.md) tiver uma faceta **image** não nula, o item representa uma imagem bitmap.</span><span class="sxs-lookup"><span data-stu-id="01953-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="01953-107">**Observação:** se o serviço não puder determinar a largura e a altura da imagem, o recurso **Image** poderá ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="01953-107">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="01953-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01953-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="01953-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01953-109">Properties</span></span>

| <span data-ttu-id="01953-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01953-110">Property</span></span>   | <span data-ttu-id="01953-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="01953-111">Type</span></span>  | <span data-ttu-id="01953-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="01953-112">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="01953-113">**height**</span><span class="sxs-lookup"><span data-stu-id="01953-113">**height**</span></span> | <span data-ttu-id="01953-114">Int32</span><span class="sxs-lookup"><span data-stu-id="01953-114">Int32</span></span> | <span data-ttu-id="01953-p102">Opcional. A altura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="01953-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="01953-118">**width**</span><span class="sxs-lookup"><span data-stu-id="01953-118">**width**</span></span>  | <span data-ttu-id="01953-119">Int32</span><span class="sxs-lookup"><span data-stu-id="01953-119">Int32</span></span> | <span data-ttu-id="01953-p103">Opcional. A largura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="01953-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="01953-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="01953-123">Remarks</span></span>

<span data-ttu-id="01953-124">No OneDrive for Business, esse recurso retorna em itens que devem ser imagens com base na extensão de arquivo.</span><span class="sxs-lookup"><span data-stu-id="01953-124">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="01953-125">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="01953-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


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


