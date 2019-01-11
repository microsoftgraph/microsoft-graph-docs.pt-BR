---
title: tipo de recurso de mediaConfig
description: A configuração de mídia usada para conectar a uma chamada.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: ec76adf2d3a508ebe2518ed0010a1c653daca546
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867344"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="4dffb-103">tipo de recurso de mediaConfig</span><span class="sxs-lookup"><span data-stu-id="4dffb-103">mediaConfig resource type</span></span>

> <span data-ttu-id="4dffb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4dffb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4dffb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4dffb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4dffb-106">A configuração de mídia usada para conectar a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="4dffb-106">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="4dffb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4dffb-107">Properties</span></span>

| <span data-ttu-id="4dffb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4dffb-108">Property</span></span>       | <span data-ttu-id="4dffb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4dffb-109">Type</span></span>    | <span data-ttu-id="4dffb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dffb-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4dffb-111">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="4dffb-111">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="4dffb-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dffb-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="4dffb-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4dffb-113">JSON representation</span></span>

<span data-ttu-id="4dffb-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4dffb-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
  ],
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
