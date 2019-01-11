---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
localization_priority: Normal
ms.openlocfilehash: 2b5e084294c528a83f80b0c49badbf8f1e96ca41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889723"
---
# <a name="image-resource-type"></a><span data-ttu-id="ab809-102">Tipo de recurso Image</span><span class="sxs-lookup"><span data-stu-id="ab809-102">Image resource type</span></span>

> <span data-ttu-id="ab809-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ab809-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab809-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ab809-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab809-p102">O recurso **Image** agrupa propriedades relacionadas a imagens em uma única estrutura. Se um [**DriveItem**](driveitem.md) tiver uma faceta **image** não nula, o item representa uma imagem bitmap.</span><span class="sxs-lookup"><span data-stu-id="ab809-p102">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="ab809-107">**Observação:** se o serviço não puder determinar a largura e a altura da imagem, o recurso **Image** poderá ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="ab809-107">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab809-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab809-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="ab809-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab809-109">Properties</span></span>

| <span data-ttu-id="ab809-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab809-110">Property</span></span>   | <span data-ttu-id="ab809-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab809-111">Type</span></span>  | <span data-ttu-id="ab809-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab809-112">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="ab809-113">**height**</span><span class="sxs-lookup"><span data-stu-id="ab809-113">**height**</span></span> | <span data-ttu-id="ab809-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ab809-114">Int32</span></span> | <span data-ttu-id="ab809-p103">Opcional. A altura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab809-p103">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="ab809-118">**width**</span><span class="sxs-lookup"><span data-stu-id="ab809-118">**width**</span></span>  | <span data-ttu-id="ab809-119">Int32</span><span class="sxs-lookup"><span data-stu-id="ab809-119">Int32</span></span> | <span data-ttu-id="ab809-p104">Opcional. A largura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab809-p104">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="ab809-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="ab809-123">Remarks</span></span>

<span data-ttu-id="ab809-124">No OneDrive for Business, esse recurso retorna em itens que devem ser imagens com base na extensão de arquivo.</span><span class="sxs-lookup"><span data-stu-id="ab809-124">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="ab809-125">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ab809-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
