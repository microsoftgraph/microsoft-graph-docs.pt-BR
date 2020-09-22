---
title: tipo de recurso mediaPrompt
description: Contém informações sobre o arquivo de áudio a ser reproduzido e outras configurações adicionais.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5b97e385cb14eb0315e9312c82e0ffd606adde2f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971738"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="72edc-103">tipo de recurso mediaPrompt</span><span class="sxs-lookup"><span data-stu-id="72edc-103">mediaPrompt resource type</span></span>

<span data-ttu-id="72edc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72edc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72edc-105">Contém informações sobre o arquivo de áudio a ser reproduzido e outras configurações adicionais.</span><span class="sxs-lookup"><span data-stu-id="72edc-105">Contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="72edc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72edc-106">Properties</span></span>

| <span data-ttu-id="72edc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72edc-107">Property</span></span>    | <span data-ttu-id="72edc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="72edc-108">Type</span></span>                      | <span data-ttu-id="72edc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="72edc-109">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="72edc-110">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="72edc-110">mediaInfo</span></span>   | [<span data-ttu-id="72edc-111">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="72edc-111">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="72edc-112">As informações de mídia.</span><span class="sxs-lookup"><span data-stu-id="72edc-112">The media information.</span></span>                                                          |

## <a name="json-representation"></a><span data-ttu-id="72edc-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72edc-113">JSON representation</span></span>

<span data-ttu-id="72edc-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="72edc-114">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="72edc-115">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72edc-115">Example</span></span>

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


