---
title: tipo de recurso mediaConfig
description: A configuração de mídia usada para se conectar a uma chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e4f6e940cd319d10cd3f03e3c94d0473164beb29
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562549"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="9bd5d-103">tipo de recurso mediaConfig</span><span class="sxs-lookup"><span data-stu-id="9bd5d-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bd5d-104">A configuração de mídia usada para se conectar a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-104">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="9bd5d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9bd5d-105">Properties</span></span>

| <span data-ttu-id="9bd5d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bd5d-106">Property</span></span>       | <span data-ttu-id="9bd5d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bd5d-107">Type</span></span>    | <span data-ttu-id="9bd5d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bd5d-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9bd5d-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="9bd5d-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="9bd5d-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="9bd5d-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="9bd5d-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9bd5d-111">JSON representation</span></span>

<span data-ttu-id="9bd5d-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-112">The following is a JSON representation of the resource.</span></span>

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
