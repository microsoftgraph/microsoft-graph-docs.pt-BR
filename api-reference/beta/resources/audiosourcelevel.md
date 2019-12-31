---
title: tipo de recurso audioSourceLevel
description: Configuração de nível para outras fontes.
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 35997bfcae7f33cc9bf8e62121c5dc2a724c95be
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913741"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="b32bc-103">tipo de recurso audioSourceLevel</span><span class="sxs-lookup"><span data-stu-id="b32bc-103">audioSourceLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b32bc-104">Configuração de nível para outras fontes.</span><span class="sxs-lookup"><span data-stu-id="b32bc-104">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="b32bc-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b32bc-105">Properties</span></span>

| <span data-ttu-id="b32bc-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b32bc-106">Property</span></span>               | <span data-ttu-id="b32bc-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b32bc-107">Type</span></span>    | <span data-ttu-id="b32bc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b32bc-108">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b32bc-109">duckOthers</span><span class="sxs-lookup"><span data-stu-id="b32bc-109">duckOthers</span></span>             | <span data-ttu-id="b32bc-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="b32bc-110">Boolean</span></span> | <span data-ttu-id="b32bc-111">Permite que essa fonte para o pato de outras fontes enquanto ativa.</span><span class="sxs-lookup"><span data-stu-id="b32bc-111">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="b32bc-112">Se for definido como true, o nível de pato precisará ser definido.</span><span class="sxs-lookup"><span data-stu-id="b32bc-112">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="b32bc-113">antes</span><span class="sxs-lookup"><span data-stu-id="b32bc-113">level</span></span>                  | <span data-ttu-id="b32bc-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b32bc-114">Int64</span></span>   | <span data-ttu-id="b32bc-115">O nível de pato da origem se `duckOthers` estiver definido como `true`.</span><span class="sxs-lookup"><span data-stu-id="b32bc-115">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="b32bc-116">participante</span><span class="sxs-lookup"><span data-stu-id="b32bc-116">participant</span></span>            | <span data-ttu-id="b32bc-117">String</span><span class="sxs-lookup"><span data-stu-id="b32bc-117">String</span></span>  | <span data-ttu-id="b32bc-118">O fluxo de áudio do participante de origem.</span><span class="sxs-lookup"><span data-stu-id="b32bc-118">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="b32bc-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b32bc-119">JSON representation</span></span>

<span data-ttu-id="b32bc-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b32bc-120">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
