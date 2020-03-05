---
title: tipo de recurso mediaConfig
description: Uma classe base abstrata que contém a configuração de mídia usada para se conectar a uma chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: eccf818abe2fd2b38fb2a3ee708b5dbf2a33fbf3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522775"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="f23f4-103">tipo de recurso mediaConfig</span><span class="sxs-lookup"><span data-stu-id="f23f4-103">mediaConfig resource type</span></span>

<span data-ttu-id="f23f4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f23f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f23f4-105">Uma classe base abstrata que contém a configuração de mídia usada para se conectar a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="f23f4-105">An abstract base class that contains the media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="f23f4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f23f4-106">Properties</span></span>

| <span data-ttu-id="f23f4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f23f4-107">Property</span></span>       | <span data-ttu-id="f23f4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f23f4-108">Type</span></span>    | <span data-ttu-id="f23f4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f23f4-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f23f4-110">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="f23f4-110">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="f23f4-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="f23f4-111">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="f23f4-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f23f4-112">JSON representation</span></span>

<span data-ttu-id="f23f4-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f23f4-113">The following is a JSON representation of the resource.</span></span>

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
