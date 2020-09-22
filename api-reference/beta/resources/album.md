---
author: JeremyKelley
ms.author: jeremyke
title: tipo de recurso do álbum
description: Faceta descrevendo um pacote que é um álbum de fotos.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b17a910a488e1fb5f051b4acc02d788a21d530d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067409"
---
# <a name="album-resource-type"></a><span data-ttu-id="809e4-103">tipo de recurso do álbum</span><span class="sxs-lookup"><span data-stu-id="809e4-103">album resource type</span></span>

<span data-ttu-id="809e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="809e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="809e4-105">Um álbum de fotos é uma maneira de agrupar virtualmente o [driveItems][driveItem] com facetas de [fotos][] em um [pacote][].</span><span class="sxs-lookup"><span data-stu-id="809e4-105">A photo album is a way to virtually group [driveItems][driveItem] with [photo][] facets together in a [bundle][].</span></span> <span data-ttu-id="809e4-106">Os pacotes desse tipo terão a propriedade **Album** definida no recurso [Bundle][] .</span><span class="sxs-lookup"><span data-stu-id="809e4-106">Bundles of this type will have the **album** property set on the [bundle][] resource.</span></span>

## <a name="properties"></a><span data-ttu-id="809e4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="809e4-107">Properties</span></span>

| <span data-ttu-id="809e4-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="809e4-108">Property name</span></span>     | <span data-ttu-id="809e4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="809e4-109">Type</span></span>   | <span data-ttu-id="809e4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="809e4-110">Description</span></span>
|:------------------|:-------|:------------------------------------------------
| <span data-ttu-id="809e4-111">coverImageItemId</span><span class="sxs-lookup"><span data-stu-id="809e4-111">coverImageItemId</span></span> | <span data-ttu-id="809e4-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="809e4-112">String</span></span> | <span data-ttu-id="809e4-113">Identificador exclusivo do [driveItem][] que é a tampa do álbum.</span><span class="sxs-lookup"><span data-stu-id="809e4-113">Unique identifier of the [driveItem][] that is the cover of the album.</span></span>

<span data-ttu-id="809e4-114">**Observação:** Se um **coverImageItemId** não tiver sido definido antes, as miniaturas de um álbum serão escolhidas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="809e4-114">**Note:** If a **coverImageItemId** has not been set before, the thumbnails for an album are chosen automatically.</span></span>
<span data-ttu-id="809e4-115">Após o **coverImageItemId** ter sido definido, as miniaturas de um álbum sempre serão o item associado a essa ID. Você pode substituir a capa padrão, CORRIGIndo o [bundle item][pacote] de itens do pacote e definindo a propriedade **coverImageItemId** no `album` para a ID de uma imagem contida no álbum.</span><span class="sxs-lookup"><span data-stu-id="809e4-115">After **coverImageItemId** has been set, the thumbnails for an album will always be the item associated with that id. You can override the default cover by PATCHing the [bundle item][bundle] and setting the **coverImageItemId** property on the `album` to the id of an image contained within the album.</span></span>
<span data-ttu-id="809e4-116">Para remover uma tampa de conjunto personalizado, você pode definir a propriedade **coverImageItemId** como NULL, e um padrão será escolhido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="809e4-116">To remove a custom-set cover, you can set the **coverImageItemId** property to null, and a default one will be chosen automatically again.</span></span>

## <a name="json-representation"></a><span data-ttu-id="809e4-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="809e4-117">JSON representation</span></span>

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


