---
author: JeremyKelley
ms.date: 09/10/2017
title: Image
localization_priority: Normal
description: O recurso Image agrupa propriedades relacionadas a imagens em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 33a85707183edc23bf42f882b937ced09e741103
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239944"
---
# <a name="image-resource-type"></a><span data-ttu-id="72afd-103">Tipo de recurso Image</span><span class="sxs-lookup"><span data-stu-id="72afd-103">Image resource type</span></span>

<span data-ttu-id="72afd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72afd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72afd-p101">O recurso **Image** agrupa propriedades relacionadas a imagens em uma única estrutura. Se um [**DriveItem**](driveitem.md) tiver uma faceta **image** não nula, o item representa uma imagem bitmap.</span><span class="sxs-lookup"><span data-stu-id="72afd-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="72afd-107">**Observação:** se o serviço não puder determinar a largura e a altura da imagem, o recurso **Image** poderá ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="72afd-107">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="72afd-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72afd-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="72afd-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72afd-109">Properties</span></span>

| <span data-ttu-id="72afd-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72afd-110">Property</span></span>   | <span data-ttu-id="72afd-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="72afd-111">Type</span></span>  | <span data-ttu-id="72afd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="72afd-112">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="72afd-113">**height**</span><span class="sxs-lookup"><span data-stu-id="72afd-113">**height**</span></span> | <span data-ttu-id="72afd-114">Int32</span><span class="sxs-lookup"><span data-stu-id="72afd-114">Int32</span></span> | <span data-ttu-id="72afd-p102">Opcional. A altura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72afd-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="72afd-118">**width**</span><span class="sxs-lookup"><span data-stu-id="72afd-118">**width**</span></span>  | <span data-ttu-id="72afd-119">Int32</span><span class="sxs-lookup"><span data-stu-id="72afd-119">Int32</span></span> | <span data-ttu-id="72afd-p103">Opcional. A largura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72afd-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="72afd-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="72afd-123">Remarks</span></span>

<span data-ttu-id="72afd-124">No OneDrive for Business, esse recurso retorna em itens que devem ser imagens com base na extensão de arquivo.</span><span class="sxs-lookup"><span data-stu-id="72afd-124">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="72afd-125">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="72afd-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->

