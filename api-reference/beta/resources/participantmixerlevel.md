---
title: tipo de recurso participantMixerLevel
description: Configuração dos níveis de mixer para um determinado participante de áudio
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cc305274d619a3686d4d391516947f1d06b92745
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006582"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="83487-103">tipo de recurso participantMixerLevel</span><span class="sxs-lookup"><span data-stu-id="83487-103">participantMixerLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83487-104">Configuração dos níveis de mixer para um determinado participante de áudio</span><span class="sxs-lookup"><span data-stu-id="83487-104">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="83487-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83487-105">Properties</span></span>

| <span data-ttu-id="83487-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83487-106">Property</span></span>               | <span data-ttu-id="83487-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="83487-107">Type</span></span>                                                      | <span data-ttu-id="83487-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="83487-108">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="83487-109">pato</span><span class="sxs-lookup"><span data-stu-id="83487-109">ducking</span></span>                | [<span data-ttu-id="83487-110">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="83487-110">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="83487-111">Configuração do phasing (entrada e saída) de outras fontes para essa combinação personalizada partipant.</span><span class="sxs-lookup"><span data-stu-id="83487-111">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="83487-112">exclusivemode</span><span class="sxs-lookup"><span data-stu-id="83487-112">exclusiveMode</span></span>          | <span data-ttu-id="83487-113">booliano</span><span class="sxs-lookup"><span data-stu-id="83487-113">boolean</span></span>                                                   | <span data-ttu-id="83487-114">Se as fontes sem nível de fonte explícita devem ser removidas da mistura.</span><span class="sxs-lookup"><span data-stu-id="83487-114">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="83487-115">participante</span><span class="sxs-lookup"><span data-stu-id="83487-115">participant</span></span>            | <span data-ttu-id="83487-116">String</span><span class="sxs-lookup"><span data-stu-id="83487-116">String</span></span>                                                    | <span data-ttu-id="83487-117">O participante para o qual o mixer está sendo configurado.</span><span class="sxs-lookup"><span data-stu-id="83487-117">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="83487-118">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="83487-118">sourceLevels</span></span>           | <span data-ttu-id="83487-119">coleção [audioSourceLevel](audiosourcelevel.md)</span><span class="sxs-lookup"><span data-stu-id="83487-119">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="83487-120">Configuração de nível para outras fontes.</span><span class="sxs-lookup"><span data-stu-id="83487-120">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="83487-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83487-121">JSON representation</span></span>

<span data-ttu-id="83487-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83487-122">The following is a JSON representation of the resource.</span></span>

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

## <a name="example---mixer-level"></a><span data-ttu-id="83487-123">Exemplo-nível do mixer</span><span class="sxs-lookup"><span data-stu-id="83487-123">Example - Mixer level</span></span>

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
