---
title: tipo de recurso de participantMixerLevel
description: Configuração do mixer níveis para determinados participante de áudio
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bb5d28ac45d510a715dcc5001c8ee02b8352bb8c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575416"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="8b748-103">tipo de recurso de participantMixerLevel</span><span class="sxs-lookup"><span data-stu-id="8b748-103">participantMixerLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b748-104">Configuração do mixer níveis para determinados participante de áudio</span><span class="sxs-lookup"><span data-stu-id="8b748-104">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="8b748-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b748-105">Properties</span></span>

| <span data-ttu-id="8b748-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b748-106">Property</span></span>               | <span data-ttu-id="8b748-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b748-107">Type</span></span>                                                      | <span data-ttu-id="8b748-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b748-108">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8b748-109">desviando</span><span class="sxs-lookup"><span data-stu-id="8b748-109">ducking</span></span>                | [<span data-ttu-id="8b748-110">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b748-110">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="8b748-111">Configuração do desviando (Introdução gradual e sair) de outras fontes para este partipant mistura personalizada.</span><span class="sxs-lookup"><span data-stu-id="8b748-111">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="8b748-112">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="8b748-112">exclusiveMode</span></span>          | <span data-ttu-id="8b748-113">booliano</span><span class="sxs-lookup"><span data-stu-id="8b748-113">boolean</span></span>                                                   | <span data-ttu-id="8b748-114">Se fontes sem nível de origem explícitas devem ser removidas da combinação.</span><span class="sxs-lookup"><span data-stu-id="8b748-114">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="8b748-115">participante</span><span class="sxs-lookup"><span data-stu-id="8b748-115">participant</span></span>            | <span data-ttu-id="8b748-116">String</span><span class="sxs-lookup"><span data-stu-id="8b748-116">String</span></span>                                                    | <span data-ttu-id="8b748-117">O participante para quem o mixer está sendo configurado.</span><span class="sxs-lookup"><span data-stu-id="8b748-117">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="8b748-118">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="8b748-118">sourceLevels</span></span>           | <span data-ttu-id="8b748-119">coleção [audioSourceLevel](audiosourcelevel.md)</span><span class="sxs-lookup"><span data-stu-id="8b748-119">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="8b748-120">Configuração de nível de outras fontes.</span><span class="sxs-lookup"><span data-stu-id="8b748-120">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="8b748-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b748-121">JSON representation</span></span>

<span data-ttu-id="8b748-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b748-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": { "@odata.type": "microsoft.graph.audioDuckingConfiguration" },
  "exclusiveMode": true,
  "participant": "String",
  "sourceLevels": [ { "@odata.type": "microsoft.graph.audioSourceLevel" } ]
}
```

## <a name="example---mixer-level"></a><span data-ttu-id="8b748-123">Exemplo - nível Mixer</span><span class="sxs-lookup"><span data-stu-id="8b748-123">Example - Mixer level</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/participantmixerlevel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
