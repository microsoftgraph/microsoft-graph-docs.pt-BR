---
title: tipo de recurso de audioSourceLevel
description: Configuração de nível de outras fontes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c91a4c57b283f7669b2be22bba5de5d958b437ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528372"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="bb8e8-103">tipo de recurso de audioSourceLevel</span><span class="sxs-lookup"><span data-stu-id="bb8e8-103">audioSourceLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb8e8-104">Configuração de nível de outras fontes.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-104">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="bb8e8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb8e8-105">Properties</span></span>

| <span data-ttu-id="bb8e8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb8e8-106">Property</span></span>               | <span data-ttu-id="bb8e8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb8e8-107">Type</span></span>    | <span data-ttu-id="bb8e8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb8e8-108">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="bb8e8-109">duckOthers</span><span class="sxs-lookup"><span data-stu-id="bb8e8-109">duckOthers</span></span>             | <span data-ttu-id="bb8e8-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb8e8-110">Boolean</span></span> | <span data-ttu-id="bb8e8-111">Habilita a essa fonte para jantar de outras fontes enquanto estão ativos.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-111">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="bb8e8-112">Se definido como true, desviando nível deve ser definido.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-112">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="bb8e8-113">nível</span><span class="sxs-lookup"><span data-stu-id="bb8e8-113">level</span></span>                  | <span data-ttu-id="bb8e8-114">Int64</span><span class="sxs-lookup"><span data-stu-id="bb8e8-114">Int64</span></span>   | <span data-ttu-id="bb8e8-115">Desviando nível da fonte se `duckOthers` estiver definida como `true`.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-115">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="bb8e8-116">participante</span><span class="sxs-lookup"><span data-stu-id="bb8e8-116">participant</span></span>            | <span data-ttu-id="bb8e8-117">String</span><span class="sxs-lookup"><span data-stu-id="bb8e8-117">String</span></span>  | <span data-ttu-id="bb8e8-118">O fluxo de áudio participante do código-fonte.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-118">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="bb8e8-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb8e8-119">JSON representation</span></span>

<span data-ttu-id="bb8e8-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb8e8-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioSourceLevel"
}-->
```json
{
  "duckOthers": true,
  "level": 100,
  "participant": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audiosourcelevel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
