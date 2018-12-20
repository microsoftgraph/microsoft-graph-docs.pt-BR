---
title: tipo de recurso de mediaConfig
description: A configuração de mídia usada para conectar a uma chamada.
author: VinodRavichandran
ms.openlocfilehash: 1b68d9236ba78ae1a83228b3382c96fc81516d1f
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380258"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="75ec5-103">tipo de recurso de mediaConfig</span><span class="sxs-lookup"><span data-stu-id="75ec5-103">mediaConfig resource type</span></span>

> <span data-ttu-id="75ec5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="75ec5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75ec5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="75ec5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75ec5-106">A configuração de mídia usada para conectar a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="75ec5-106">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="75ec5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75ec5-107">Properties</span></span>

| <span data-ttu-id="75ec5-108">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="75ec5-108">Property</span></span>       | <span data-ttu-id="75ec5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="75ec5-109">Type</span></span>    | <span data-ttu-id="75ec5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="75ec5-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="75ec5-111">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="75ec5-111">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="75ec5-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="75ec5-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="75ec5-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75ec5-113">JSON representation</span></span>

<span data-ttu-id="75ec5-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75ec5-114">The following is a JSON representation of the resource.</span></span>

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