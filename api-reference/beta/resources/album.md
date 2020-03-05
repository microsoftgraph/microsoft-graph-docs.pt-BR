---
author: JeremyKelley
ms.author: jeremyke
title: tipo de recurso do álbum
description: Faceta descrevendo um pacote que é um álbum de fotos.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 60d653db52f71de6fe4079df25223b393ea18da3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508356"
---
# <a name="album-resource-type"></a><span data-ttu-id="a772a-103">tipo de recurso do álbum</span><span class="sxs-lookup"><span data-stu-id="a772a-103">album resource type</span></span>

<span data-ttu-id="a772a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a772a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a772a-105">Um álbum de fotos é uma maneira de agrupar virtualmente o [driveItems][driveItem] com facetas de [fotos][] em um [pacote][].</span><span class="sxs-lookup"><span data-stu-id="a772a-105">A photo album is a way to virtually group [driveItems][driveItem] with [photo][] facets together in a [bundle][].</span></span> <span data-ttu-id="a772a-106">Os pacotes desse tipo terão a propriedade **Album** definida no recurso [Bundle][] .</span><span class="sxs-lookup"><span data-stu-id="a772a-106">Bundles of this type will have the **album** property set on the [bundle][] resource.</span></span>

## <a name="properties"></a><span data-ttu-id="a772a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a772a-107">Properties</span></span>

| <span data-ttu-id="a772a-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a772a-108">Property name</span></span>     | <span data-ttu-id="a772a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a772a-109">Type</span></span>   | <span data-ttu-id="a772a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a772a-110">Description</span></span>
|:------------------|:-------|:------------------------------------------------
| <span data-ttu-id="a772a-111">coverImageItemId</span><span class="sxs-lookup"><span data-stu-id="a772a-111">coverImageItemId</span></span> | <span data-ttu-id="a772a-112">String</span><span class="sxs-lookup"><span data-stu-id="a772a-112">String</span></span> | <span data-ttu-id="a772a-113">Identificador exclusivo do [driveItem][] que é a tampa do álbum.</span><span class="sxs-lookup"><span data-stu-id="a772a-113">Unique identifier of the [driveItem][] that is the cover of the album.</span></span>

<span data-ttu-id="a772a-114">**Observação:** Se um **coverImageItemId** não tiver sido definido antes, as miniaturas de um álbum serão escolhidas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="a772a-114">**Note:** If a **coverImageItemId** has not been set before, the thumbnails for an album are chosen automatically.</span></span>
<span data-ttu-id="a772a-115">Após o **coverImageItemId** ter sido definido, as miniaturas de um álbum sempre serão o item associado a essa ID. Você pode substituir a capa padrão, CORRIGIndo o [][pacote] de itens do pacote e definindo a propriedade **coverImageItemId** no `album` para a ID de uma imagem contida no álbum.</span><span class="sxs-lookup"><span data-stu-id="a772a-115">After **coverImageItemId** has been set, the thumbnails for an album will always be the item associated with that id. You can override the default cover by PATCHing the [bundle item][bundle] and setting the **coverImageItemId** property on the `album` to the id of an image contained within the album.</span></span>
<span data-ttu-id="a772a-116">Para remover uma tampa de conjunto personalizado, você pode definir a propriedade **coverImageItemId** como NULL, e um padrão será escolhido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="a772a-116">To remove a custom-set cover, you can set the **coverImageItemId** property to null, and a default one will be chosen automatically again.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a772a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a772a-117">JSON representation</span></span>

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
