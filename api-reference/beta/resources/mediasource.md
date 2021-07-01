---
author: MarcMroz
description: O recurso mediaSource contém metadados sobre a origem do item de unidade de mídia (áudio ou vídeo).
title: Tipo de recurso mediaSource
localization_priority: Normal
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: c0b2f93095d7e7a4b9176073cc8688b5eb473cd3
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236296"
---
# <a name="mediasource-resouce-type"></a><span data-ttu-id="baa68-103">tipo de resouce mediaSource</span><span class="sxs-lookup"><span data-stu-id="baa68-103">mediaSource resouce type</span></span>

<span data-ttu-id="baa68-104">O **recurso mediaSource** contém metadados sobre a origem do item de unidade de mídia (áudio ou vídeo).</span><span class="sxs-lookup"><span data-stu-id="baa68-104">The **mediaSource** resource contains metadata about the source of media (audio or video) drive item.</span></span>

<span data-ttu-id="baa68-105">Ele está disponível na propriedade de mídia dos [recursos driveItem.][item-resource]</span><span class="sxs-lookup"><span data-stu-id="baa68-105">It is available on the media property of [driveItem][item-resource] resources.</span></span>

## <a name="properties"></a><span data-ttu-id="baa68-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="baa68-106">Properties</span></span>

| <span data-ttu-id="baa68-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="baa68-107">Property</span></span>                 | <span data-ttu-id="baa68-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="baa68-108">Type</span></span>                       | <span data-ttu-id="baa68-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="baa68-109">Description</span></span>                                                                                      |
| :----------------------- | :------------------------  | :----------------------------------------------------------------------------------------------- |
| <span data-ttu-id="baa68-110">**contentCategory**</span><span class="sxs-lookup"><span data-stu-id="baa68-110">**contentCategory**</span></span>      | <span data-ttu-id="baa68-111">mediaSourceContentCategory</span><span class="sxs-lookup"><span data-stu-id="baa68-111">mediaSourceContentCategory</span></span> | <span data-ttu-id="baa68-112">Valor de enumeração que indica a categoria de conteúdo de mídia.</span><span class="sxs-lookup"><span data-stu-id="baa68-112">Enumeration value that indicates the media content category.</span></span>                                     |

### <a name="mediasourcecontentcategory-values"></a><span data-ttu-id="baa68-113">valores mediaSourceContentCategory</span><span class="sxs-lookup"><span data-stu-id="baa68-113">mediaSourceContentCategory values</span></span>

| <span data-ttu-id="baa68-114">Valor</span><span class="sxs-lookup"><span data-stu-id="baa68-114">Value</span></span>               | <span data-ttu-id="baa68-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="baa68-115">Description</span></span>                                         |
|:------------------- |:----------------------------------------------------|
| <span data-ttu-id="baa68-116">meeting</span><span class="sxs-lookup"><span data-stu-id="baa68-116">meeting</span></span>             | <span data-ttu-id="baa68-117">A mídia é uma reunião.</span><span class="sxs-lookup"><span data-stu-id="baa68-117">The media is a meeting.</span></span>                             |
| <span data-ttu-id="baa68-118">liveStream</span><span class="sxs-lookup"><span data-stu-id="baa68-118">liveStream</span></span>          | <span data-ttu-id="baa68-119">A mídia é uma transmissão ao vivo.</span><span class="sxs-lookup"><span data-stu-id="baa68-119">The media is a live stream.</span></span>                         |
| <span data-ttu-id="baa68-120">presentation</span><span class="sxs-lookup"><span data-stu-id="baa68-120">presentation</span></span>        | <span data-ttu-id="baa68-121">A mídia é uma apresentação.</span><span class="sxs-lookup"><span data-stu-id="baa68-121">The media is a presentation.</span></span>                        |
| <span data-ttu-id="baa68-122">screenRecording</span><span class="sxs-lookup"><span data-stu-id="baa68-122">screenRecording</span></span>     | <span data-ttu-id="baa68-123">A mídia é uma gravação de tela.</span><span class="sxs-lookup"><span data-stu-id="baa68-123">The media is a screen recording.</span></span>                    |
| <span data-ttu-id="baa68-124">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="baa68-124">unknownFutureValue</span></span>  | <span data-ttu-id="baa68-125">Valor do marcador para compatibilidade futura.</span><span class="sxs-lookup"><span data-stu-id="baa68-125">Marker value for future compatibility.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="baa68-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="baa68-126">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "contentCategory"
  ],
  "@odata.type": "microsoft.graph.mediaSource"
}-->

```json
{
  "contentCategory" : "string"
}
```

## <a name="see-also"></a><span data-ttu-id="baa68-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="baa68-127">See also</span></span>

<span data-ttu-id="baa68-128">Para obter mais informações sobre as facetas em um driveItem, [consulte driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="baa68-128">For more information about the facets on a driveItem, see [driveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The mediaSource facet provides information about drive item source.",
  "keywords": "mediaSource,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/MediaSource"
} -->
