---
title: tipo de recurso audioSourceLevel
description: Configuração de nível para outras fontes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bc2b0c11b18a3cf8120cab0bb9c745ae8880cfc6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339019"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="9430e-103">tipo de recurso audioSourceLevel</span><span class="sxs-lookup"><span data-stu-id="9430e-103">audioSourceLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9430e-104">Configuração de nível para outras fontes.</span><span class="sxs-lookup"><span data-stu-id="9430e-104">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="9430e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9430e-105">Properties</span></span>

| <span data-ttu-id="9430e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9430e-106">Property</span></span>               | <span data-ttu-id="9430e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9430e-107">Type</span></span>    | <span data-ttu-id="9430e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9430e-108">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9430e-109">duckOthers</span><span class="sxs-lookup"><span data-stu-id="9430e-109">duckOthers</span></span>             | <span data-ttu-id="9430e-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="9430e-110">Boolean</span></span> | <span data-ttu-id="9430e-111">Permite que essa fonte para o pato de outras fontes enquanto ativa.</span><span class="sxs-lookup"><span data-stu-id="9430e-111">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="9430e-112">Se for definido como true, o nível de pato precisará ser definido.</span><span class="sxs-lookup"><span data-stu-id="9430e-112">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="9430e-113">antes</span><span class="sxs-lookup"><span data-stu-id="9430e-113">level</span></span>                  | <span data-ttu-id="9430e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="9430e-114">Int64</span></span>   | <span data-ttu-id="9430e-115">O nível de pato da origem se `duckOthers` estiver definido como `true`.</span><span class="sxs-lookup"><span data-stu-id="9430e-115">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="9430e-116">participante</span><span class="sxs-lookup"><span data-stu-id="9430e-116">participant</span></span>            | <span data-ttu-id="9430e-117">String</span><span class="sxs-lookup"><span data-stu-id="9430e-117">String</span></span>  | <span data-ttu-id="9430e-118">O fluxo de áudio do participante de origem.</span><span class="sxs-lookup"><span data-stu-id="9430e-118">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="9430e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9430e-119">JSON representation</span></span>

<span data-ttu-id="9430e-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9430e-120">The following is a JSON representation of the resource.</span></span>

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
