---
title: tipo de recurso audioSourceLevel
description: Configuração de nível para outras fontes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c91a4c57b283f7669b2be22bba5de5d958b437ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535573"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="561bd-103">tipo de recurso audioSourceLevel</span><span class="sxs-lookup"><span data-stu-id="561bd-103">audioSourceLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="561bd-104">Configuração de nível para outras fontes.</span><span class="sxs-lookup"><span data-stu-id="561bd-104">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="561bd-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="561bd-105">Properties</span></span>

| <span data-ttu-id="561bd-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="561bd-106">Property</span></span>               | <span data-ttu-id="561bd-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="561bd-107">Type</span></span>    | <span data-ttu-id="561bd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="561bd-108">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="561bd-109">duckOthers</span><span class="sxs-lookup"><span data-stu-id="561bd-109">duckOthers</span></span>             | <span data-ttu-id="561bd-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="561bd-110">Boolean</span></span> | <span data-ttu-id="561bd-111">Permite que essa fonte para o pato de outras fontes enquanto ativa.</span><span class="sxs-lookup"><span data-stu-id="561bd-111">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="561bd-112">Se for definido como true, o nível de pato precisará ser definido.</span><span class="sxs-lookup"><span data-stu-id="561bd-112">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="561bd-113">level</span><span class="sxs-lookup"><span data-stu-id="561bd-113">level</span></span>                  | <span data-ttu-id="561bd-114">Int64</span><span class="sxs-lookup"><span data-stu-id="561bd-114">Int64</span></span>   | <span data-ttu-id="561bd-115">O nível de pato da origem se `duckOthers` estiver definido como `true`.</span><span class="sxs-lookup"><span data-stu-id="561bd-115">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="561bd-116">participante</span><span class="sxs-lookup"><span data-stu-id="561bd-116">participant</span></span>            | <span data-ttu-id="561bd-117">String</span><span class="sxs-lookup"><span data-stu-id="561bd-117">String</span></span>  | <span data-ttu-id="561bd-118">O fluxo de áudio do participante de origem.</span><span class="sxs-lookup"><span data-stu-id="561bd-118">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="561bd-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="561bd-119">JSON representation</span></span>

<span data-ttu-id="561bd-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="561bd-120">The following is a JSON representation of the resource.</span></span>

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
