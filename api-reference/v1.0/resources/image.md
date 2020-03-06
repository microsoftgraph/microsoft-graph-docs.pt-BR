---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Image
localization_priority: Normal
description: O recurso Image agrupa propriedades relacionadas a imagens em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b270d7ed2cacc5da5926d77d651878f9b0598093
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532886"
---
# <a name="image-resource-type"></a><span data-ttu-id="83798-103">Tipo de recurso Image</span><span class="sxs-lookup"><span data-stu-id="83798-103">Image resource type</span></span>

<span data-ttu-id="83798-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83798-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83798-p101">O recurso **Image** agrupa propriedades relacionadas a imagens em uma única estrutura. Se um [**DriveItem**](driveitem.md) tiver uma faceta **image** não nula, o item representa uma imagem bitmap.</span><span class="sxs-lookup"><span data-stu-id="83798-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="83798-107">**Observação:** se o serviço não puder determinar a largura e a altura da imagem, o recurso **Image** poderá ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="83798-107">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="83798-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83798-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="83798-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83798-109">Properties</span></span>

| <span data-ttu-id="83798-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83798-110">Property</span></span>   | <span data-ttu-id="83798-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="83798-111">Type</span></span>  | <span data-ttu-id="83798-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="83798-112">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="83798-113">**height**</span><span class="sxs-lookup"><span data-stu-id="83798-113">**height**</span></span> | <span data-ttu-id="83798-114">Int32</span><span class="sxs-lookup"><span data-stu-id="83798-114">Int32</span></span> | <span data-ttu-id="83798-p102">Opcional. A altura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="83798-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="83798-118">**width**</span><span class="sxs-lookup"><span data-stu-id="83798-118">**width**</span></span>  | <span data-ttu-id="83798-119">Int32</span><span class="sxs-lookup"><span data-stu-id="83798-119">Int32</span></span> | <span data-ttu-id="83798-p103">Opcional. A largura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="83798-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="83798-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="83798-123">Remarks</span></span>

<span data-ttu-id="83798-124">No OneDrive for Business, esse recurso retorna em itens que devem ser imagens com base na extensão de arquivo.</span><span class="sxs-lookup"><span data-stu-id="83798-124">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="83798-125">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="83798-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
