---
title: tipo de recurso mediaPrompt
description: Esse tipo de recurso contém informações sobre o arquivo de áudio a ser reproduzido e outras configurações adicionais.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 37329364ccfcb4b70de04ebfe8344ea407ce2bc7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965516"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="31eb0-103">tipo de recurso mediaPrompt</span><span class="sxs-lookup"><span data-stu-id="31eb0-103">mediaPrompt resource type</span></span>

<span data-ttu-id="31eb0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31eb0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="31eb0-105">Esse tipo de recurso contém informações sobre o arquivo de áudio a ser reproduzido e outras configurações adicionais.</span><span class="sxs-lookup"><span data-stu-id="31eb0-105">This resource type contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="31eb0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31eb0-106">Properties</span></span>

| <span data-ttu-id="31eb0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31eb0-107">Property</span></span>    | <span data-ttu-id="31eb0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="31eb0-108">Type</span></span>                      | <span data-ttu-id="31eb0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="31eb0-109">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="31eb0-110">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="31eb0-110">mediaInfo</span></span>   | [<span data-ttu-id="31eb0-111">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="31eb0-111">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="31eb0-112">As informações de mídia</span><span class="sxs-lookup"><span data-stu-id="31eb0-112">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="31eb0-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31eb0-113">JSON representation</span></span>

<span data-ttu-id="31eb0-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31eb0-114">The following is a JSON representation of the resource.</span></span>

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

