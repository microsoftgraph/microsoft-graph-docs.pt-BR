---
author: JeremyKelley
ms.author: jeremyke
title: tipo de recurso do álbum
description: Faceta descrevendo um pacote que é um álbum de fotos.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3bb5391557c3dfb0a97702a0e78de60c0a4876c7
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932638"
---
# <a name="album-resource-type"></a><span data-ttu-id="16658-103">tipo de recurso do álbum</span><span class="sxs-lookup"><span data-stu-id="16658-103">album resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16658-104">Um álbum de fotos é uma maneira de agrupar virtualmente o [driveItems][driveItem] com facetas de [fotos][] em um [pacote][].</span><span class="sxs-lookup"><span data-stu-id="16658-104">A photo album is a way to virtually group [driveItems][driveItem] with [photo][] facets together in a [bundle][].</span></span> <span data-ttu-id="16658-105">Os pacotes desse tipo terão a propriedade **Album** definida no recurso [Bundle][] .</span><span class="sxs-lookup"><span data-stu-id="16658-105">Bundles of this type will have the **album** property set on the [bundle][] resource.</span></span>

## <a name="properties"></a><span data-ttu-id="16658-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16658-106">Properties</span></span>

| <span data-ttu-id="16658-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="16658-107">Property name</span></span>     | <span data-ttu-id="16658-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="16658-108">Type</span></span>   | <span data-ttu-id="16658-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="16658-109">Description</span></span>
|:------------------|:-------|:------------------------------------------------
| <span data-ttu-id="16658-110">coverImageItemId</span><span class="sxs-lookup"><span data-stu-id="16658-110">coverImageItemId</span></span> | <span data-ttu-id="16658-111">String</span><span class="sxs-lookup"><span data-stu-id="16658-111">String</span></span> | <span data-ttu-id="16658-112">Identificador exclusivo do [driveItem][] que é a tampa do álbum.</span><span class="sxs-lookup"><span data-stu-id="16658-112">Unique identifier of the [driveItem][] that is the cover of the album.</span></span>

<span data-ttu-id="16658-113">**Observação:** Se um **coverImageItemId** não tiver sido definido antes, as miniaturas de um álbum serão escolhidas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="16658-113">**Note:** If a **coverImageItemId** has not been set before, the thumbnails for an album are chosen automatically.</span></span>
<span data-ttu-id="16658-114">Após o **coverImageItemId** ter sido definido, as miniaturas de um álbum sempre serão o item associado a essa ID. Você pode substituir a capa padrão, CORRIGIndo o [][pacote] de itens do pacote e definindo a propriedade **coverImageItemId** no `album` para a ID de uma imagem contida no álbum.</span><span class="sxs-lookup"><span data-stu-id="16658-114">After **coverImageItemId** has been set, the thumbnails for an album will always be the item associated with that id. You can override the default cover by PATCHing the [bundle item][bundle] and setting the **coverImageItemId** property on the `album` to the id of an image contained within the album.</span></span>
<span data-ttu-id="16658-115">Para remover uma tampa de conjunto personalizado, você pode definir a propriedade **coverImageItemId** como NULL, e um padrão será escolhido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="16658-115">To remove a custom-set cover, you can set the **coverImageItemId** property to null, and a default one will be chosen automatically again.</span></span>

## <a name="json-representation"></a><span data-ttu-id="16658-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16658-116">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.album" } -->

```json
{
  "coverImageItemId": "string"
}
```

[pacote]: bundle.md
[bundle]: bundle.md
[driveItem]: driveItem.md
[photo]: photo.md
