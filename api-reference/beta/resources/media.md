---
author: MarcMroz
description: O recurso de mídia contém metadados sobre o item de unidade de mídia (áudio ou vídeo).
title: tipo de recurso de mídia
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 488201407363469ff09220c1dcce3c15f02e3b93
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236297"
---
# <a name="media-resouce-type"></a><span data-ttu-id="9c15d-103">tipo de resouce de mídia</span><span class="sxs-lookup"><span data-stu-id="9c15d-103">media resouce type</span></span>

<span data-ttu-id="9c15d-104">Contém metadados sobre o item de unidade de mídia (áudio ou vídeo).</span><span class="sxs-lookup"><span data-stu-id="9c15d-104">Contains metadata about the media (audio or video) drive item.</span></span>

<span data-ttu-id="9c15d-105">Ele está disponível na propriedade de mídia dos [recursos driveItem.][item-resource]</span><span class="sxs-lookup"><span data-stu-id="9c15d-105">It is available on the media property of [driveItem][item-resource] resources.</span></span>


## <a name="properties"></a><span data-ttu-id="9c15d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c15d-106">Properties</span></span>

| <span data-ttu-id="9c15d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c15d-107">Property</span></span>                 | <span data-ttu-id="9c15d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c15d-108">Type</span></span>                  | <span data-ttu-id="9c15d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c15d-109">Description</span></span>                                                                                                   |
| :----------------------- | :-------------------- | :------------------------------------------------------------------------------------------------------------ 
| <span data-ttu-id="9c15d-110">**isTranscriptionShown**</span><span class="sxs-lookup"><span data-stu-id="9c15d-110">**isTranscriptionShown**</span></span> | <span data-ttu-id="9c15d-111">Booleano</span><span class="sxs-lookup"><span data-stu-id="9c15d-111">Boolean</span></span>               | <span data-ttu-id="9c15d-112">Se um arquivo tiver uma transcrição, essa configuração controlará se as legendas/transcrição fechadas do arquivo de mídia devem ser mostradas para as pessoas durante a exibição.</span><span class="sxs-lookup"><span data-stu-id="9c15d-112">If a file has a transcript, this setting controls if the closed captions / transcription for the media file should be shown to people during viewing.</span></span> <span data-ttu-id="9c15d-113">Leitura-Gravação.</span><span class="sxs-lookup"><span data-stu-id="9c15d-113">Read-Write.</span></span>                                                    |
| <span data-ttu-id="9c15d-114">**mediaSource**</span><span class="sxs-lookup"><span data-stu-id="9c15d-114">**mediaSource**</span></span>          | [<span data-ttu-id="9c15d-115">mediaSource</span><span class="sxs-lookup"><span data-stu-id="9c15d-115">mediaSource</span></span>](mediaSource.md)         | <span data-ttu-id="9c15d-116">Informações sobre a origem da mídia.</span><span class="sxs-lookup"><span data-stu-id="9c15d-116">Information about the source of media.</span></span> <span data-ttu-id="9c15d-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c15d-117">Read-only.</span></span>                                                             | 


## <a name="json-representation"></a><span data-ttu-id="9c15d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c15d-118">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.media"
}-->

```json
{
  "isTranscriptionShown" : true,
  "mediaSource": { "@odata.type": "microsoft.graph.mediaSource" }
}
```

## <a name="see-also"></a><span data-ttu-id="9c15d-119">Confira também</span><span class="sxs-lookup"><span data-stu-id="9c15d-119">See also</span></span> 

<span data-ttu-id="9c15d-120">Para obter mais informações sobre as facetas em um driveItem, [consulte driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="9c15d-120">For more information about the facets on a driveItem, see [driveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md
[mediaSource]: mediaSource.md

<!-- {
  "type": "#page.annotation",
  "description": "The media resource type provides information about the media item.",
  "keywords": "mediaItem,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/Media"
} -->
