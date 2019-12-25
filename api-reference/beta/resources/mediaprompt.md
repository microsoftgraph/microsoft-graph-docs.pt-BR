---
title: tipo de recurso mediaPrompt
description: Contém informações sobre o arquivo de áudio a ser reproduzido e outras configurações adicionais.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ba04bda06fa4adfe158046e5e0b251e770e5ee38
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866704"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="c72c7-103">tipo de recurso mediaPrompt</span><span class="sxs-lookup"><span data-stu-id="c72c7-103">mediaPrompt resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c72c7-104">Contém informações sobre o arquivo de áudio a ser reproduzido e outras configurações adicionais.</span><span class="sxs-lookup"><span data-stu-id="c72c7-104">Contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="c72c7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c72c7-105">Properties</span></span>

| <span data-ttu-id="c72c7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c72c7-106">Property</span></span>    | <span data-ttu-id="c72c7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c72c7-107">Type</span></span>                      | <span data-ttu-id="c72c7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c72c7-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="c72c7-109">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="c72c7-109">mediaInfo</span></span>   | [<span data-ttu-id="c72c7-110">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="c72c7-110">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="c72c7-111">As informações de mídia.</span><span class="sxs-lookup"><span data-stu-id="c72c7-111">The media information.</span></span>                                                          |

## <a name="json-representation"></a><span data-ttu-id="c72c7-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c72c7-112">JSON representation</span></span>

<span data-ttu-id="c72c7-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c72c7-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a><span data-ttu-id="c72c7-114">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c72c7-114">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "@odata.type": "#microsoft.graph.mediaPrompt",
  "mediaInfo": {
    "@odata.type": "#microsoft.graph.mediaInfo",
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
