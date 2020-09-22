---
title: tipo de recurso participantMixerLevel
description: Configuração dos níveis de mixer para um determinado participante de áudio
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fdec09b80eddfc4a4ea3f87425c211ed49f22ded
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998233"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="785f8-103">tipo de recurso participantMixerLevel</span><span class="sxs-lookup"><span data-stu-id="785f8-103">participantMixerLevel resource type</span></span>

<span data-ttu-id="785f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="785f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="785f8-105">Configuração dos níveis de mixer para um determinado participante de áudio</span><span class="sxs-lookup"><span data-stu-id="785f8-105">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="785f8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="785f8-106">Properties</span></span>

| <span data-ttu-id="785f8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="785f8-107">Property</span></span>               | <span data-ttu-id="785f8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="785f8-108">Type</span></span>                                                      | <span data-ttu-id="785f8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="785f8-109">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="785f8-110">pato</span><span class="sxs-lookup"><span data-stu-id="785f8-110">ducking</span></span>                | [<span data-ttu-id="785f8-111">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="785f8-111">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="785f8-112">Configuração do phasing (entrada e saída) de outras fontes para essa combinação personalizada partipant.</span><span class="sxs-lookup"><span data-stu-id="785f8-112">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="785f8-113">exclusivemode</span><span class="sxs-lookup"><span data-stu-id="785f8-113">exclusiveMode</span></span>          | <span data-ttu-id="785f8-114">booliano</span><span class="sxs-lookup"><span data-stu-id="785f8-114">boolean</span></span>                                                   | <span data-ttu-id="785f8-115">Se as fontes sem nível de fonte explícita devem ser removidas da mistura.</span><span class="sxs-lookup"><span data-stu-id="785f8-115">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="785f8-116">participante</span><span class="sxs-lookup"><span data-stu-id="785f8-116">participant</span></span>            | <span data-ttu-id="785f8-117">String</span><span class="sxs-lookup"><span data-stu-id="785f8-117">String</span></span>                                                    | <span data-ttu-id="785f8-118">O participante para o qual o mixer está sendo configurado.</span><span class="sxs-lookup"><span data-stu-id="785f8-118">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="785f8-119">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="785f8-119">sourceLevels</span></span>           | <span data-ttu-id="785f8-120">coleção [audioSourceLevel](audiosourcelevel.md)</span><span class="sxs-lookup"><span data-stu-id="785f8-120">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="785f8-121">Configuração de nível para outras fontes.</span><span class="sxs-lookup"><span data-stu-id="785f8-121">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="785f8-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="785f8-122">JSON representation</span></span>

<span data-ttu-id="785f8-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="785f8-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": { "@odata.type": "#microsoft.graph.audioDuckingConfiguration" },
  "exclusiveMode": true,
  "participant": "String",
  "sourceLevels": [ { "@odata.type": "#microsoft.graph.audioSourceLevel" } ]
}
```

## <a name="example---mixer-level"></a><span data-ttu-id="785f8-124">Exemplo-nível do mixer</span><span class="sxs-lookup"><span data-stu-id="785f8-124">Example - Mixer level</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": {
    "@odata.type": "#microsoft.graph.audioDuckingParameters",
    "rampActive": 1000,
    "rampInactive": 1000,
    "lowerLevel": 20,
    "upperLevel": 100
  },
  "exclusiveMode": true,
  "participant": "123456W77E24E4D85F80597083CB830",
  "sourceLevels": [
    {
      "@odata.type": "#microsoft.graph.audioSourceLevel",
      "duckOthers": false,
      "level": 100,
      "participant": "8A34A46B3D174ADC8DCEDC4E7D572698"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantMixerLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


