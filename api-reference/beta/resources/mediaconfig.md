---
title: tipo de recurso mediaConfig
description: Uma classe base abstrata que contém a configuração de mídia usada para se conectar a uma chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 05f93ff0776795d988b66ad84c98af1d5f5bede2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971752"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="1a4de-103">tipo de recurso mediaConfig</span><span class="sxs-lookup"><span data-stu-id="1a4de-103">mediaConfig resource type</span></span>

<span data-ttu-id="1a4de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a4de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a4de-105">Uma classe base abstrata que contém a configuração de mídia usada para se conectar a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="1a4de-105">An abstract base class that contains the media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="1a4de-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a4de-106">Properties</span></span>

| <span data-ttu-id="1a4de-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a4de-107">Property</span></span>       | <span data-ttu-id="1a4de-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a4de-108">Type</span></span>    | <span data-ttu-id="1a4de-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a4de-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1a4de-110">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="1a4de-110">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="1a4de-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a4de-111">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="1a4de-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a4de-112">JSON representation</span></span>

<span data-ttu-id="1a4de-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a4de-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
   ],
  "abstract": true,
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


