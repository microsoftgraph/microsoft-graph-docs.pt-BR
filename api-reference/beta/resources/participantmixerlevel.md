---
title: tipo de recurso de participantMixerLevel
description: Configuração do mixer níveis para determinados participante de áudio
ms.openlocfilehash: 920c22cf423391d2efcdf7177fdc7491250d0f19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040791"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="662ac-103">tipo de recurso de participantMixerLevel</span><span class="sxs-lookup"><span data-stu-id="662ac-103">participantMixerLevel resource type</span></span>

> <span data-ttu-id="662ac-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="662ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="662ac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="662ac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="662ac-106">Configuração do mixer níveis para determinados participante de áudio</span><span class="sxs-lookup"><span data-stu-id="662ac-106">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="662ac-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="662ac-107">Properties</span></span>

| <span data-ttu-id="662ac-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="662ac-108">Property</span></span>               | <span data-ttu-id="662ac-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="662ac-109">Type</span></span>                                                      | <span data-ttu-id="662ac-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="662ac-110">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="662ac-111">desviando</span><span class="sxs-lookup"><span data-stu-id="662ac-111">ducking</span></span>                | [<span data-ttu-id="662ac-112">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="662ac-112">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="662ac-113">Configuração do desviando (Introdução gradual e sair) de outras fontes para este partipant mistura personalizada.</span><span class="sxs-lookup"><span data-stu-id="662ac-113">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="662ac-114">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="662ac-114">exclusiveMode</span></span>          | <span data-ttu-id="662ac-115">booliano</span><span class="sxs-lookup"><span data-stu-id="662ac-115">boolean</span></span>                                                   | <span data-ttu-id="662ac-116">Se fontes sem nível de origem explícitas devem ser removidas da combinação.</span><span class="sxs-lookup"><span data-stu-id="662ac-116">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="662ac-117">participante</span><span class="sxs-lookup"><span data-stu-id="662ac-117">participant</span></span>            | <span data-ttu-id="662ac-118">String</span><span class="sxs-lookup"><span data-stu-id="662ac-118">String</span></span>                                                    | <span data-ttu-id="662ac-119">O participante para quem o mixer está sendo configurado.</span><span class="sxs-lookup"><span data-stu-id="662ac-119">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="662ac-120">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="662ac-120">sourceLevels</span></span>           | <span data-ttu-id="662ac-121">coleção [audioSourceLevel](audiosourcelevel.md)</span><span class="sxs-lookup"><span data-stu-id="662ac-121">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="662ac-122">Configuração de nível de outras fontes.</span><span class="sxs-lookup"><span data-stu-id="662ac-122">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="662ac-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="662ac-123">JSON representation</span></span>

<span data-ttu-id="662ac-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="662ac-124">The following is a JSON representation of the resource.</span></span>

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

## <a name="example---mixer-level"></a><span data-ttu-id="662ac-125">Exemplo - nível Mixer</span><span class="sxs-lookup"><span data-stu-id="662ac-125">Example - Mixer level</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "participantMixerLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
