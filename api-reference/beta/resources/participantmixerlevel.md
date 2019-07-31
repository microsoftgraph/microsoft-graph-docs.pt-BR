---
title: tipo de recurso participantMixerLevel
description: Configuração dos níveis de mixer para um determinado participante de áudio
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 27ddc297f779d1a40350bd4cc24015a2c60dd9ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966225"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="1b65a-103">tipo de recurso participantMixerLevel</span><span class="sxs-lookup"><span data-stu-id="1b65a-103">participantMixerLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b65a-104">Configuração dos níveis de mixer para um determinado participante de áudio</span><span class="sxs-lookup"><span data-stu-id="1b65a-104">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="1b65a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b65a-105">Properties</span></span>

| <span data-ttu-id="1b65a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b65a-106">Property</span></span>               | <span data-ttu-id="1b65a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b65a-107">Type</span></span>                                                      | <span data-ttu-id="1b65a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b65a-108">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1b65a-109">pato</span><span class="sxs-lookup"><span data-stu-id="1b65a-109">ducking</span></span>                | [<span data-ttu-id="1b65a-110">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="1b65a-110">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="1b65a-111">Configuração do phasing (entrada e saída) de outras fontes para essa combinação personalizada partipant.</span><span class="sxs-lookup"><span data-stu-id="1b65a-111">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="1b65a-112">exclusivemode</span><span class="sxs-lookup"><span data-stu-id="1b65a-112">exclusiveMode</span></span>          | <span data-ttu-id="1b65a-113">booliano</span><span class="sxs-lookup"><span data-stu-id="1b65a-113">boolean</span></span>                                                   | <span data-ttu-id="1b65a-114">Se as fontes sem nível de fonte explícita devem ser removidas da mistura.</span><span class="sxs-lookup"><span data-stu-id="1b65a-114">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="1b65a-115">participante</span><span class="sxs-lookup"><span data-stu-id="1b65a-115">participant</span></span>            | <span data-ttu-id="1b65a-116">String</span><span class="sxs-lookup"><span data-stu-id="1b65a-116">String</span></span>                                                    | <span data-ttu-id="1b65a-117">O participante para o qual o mixer está sendo configurado.</span><span class="sxs-lookup"><span data-stu-id="1b65a-117">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="1b65a-118">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="1b65a-118">sourceLevels</span></span>           | <span data-ttu-id="1b65a-119">coleção [audioSourceLevel](audiosourcelevel.md)</span><span class="sxs-lookup"><span data-stu-id="1b65a-119">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="1b65a-120">Configuração de nível para outras fontes.</span><span class="sxs-lookup"><span data-stu-id="1b65a-120">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="1b65a-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b65a-121">JSON representation</span></span>

<span data-ttu-id="1b65a-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b65a-122">The following is a JSON representation of the resource.</span></span>

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

## <a name="example---mixer-level"></a><span data-ttu-id="1b65a-123">Exemplo-nível do mixer</span><span class="sxs-lookup"><span data-stu-id="1b65a-123">Example - Mixer level</span></span>

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
