---
title: tipo de recurso audioSourceLevel
description: Configuração de nível para outras fontes.
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: beb67d906c5f159f94ab8f64863eb383286489b2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508098"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="bc03d-103">tipo de recurso audioSourceLevel</span><span class="sxs-lookup"><span data-stu-id="bc03d-103">audioSourceLevel resource type</span></span>

<span data-ttu-id="bc03d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bc03d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc03d-105">Configuração de nível para outras fontes.</span><span class="sxs-lookup"><span data-stu-id="bc03d-105">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="bc03d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc03d-106">Properties</span></span>

| <span data-ttu-id="bc03d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc03d-107">Property</span></span>               | <span data-ttu-id="bc03d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc03d-108">Type</span></span>    | <span data-ttu-id="bc03d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc03d-109">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="bc03d-110">duckOthers</span><span class="sxs-lookup"><span data-stu-id="bc03d-110">duckOthers</span></span>             | <span data-ttu-id="bc03d-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc03d-111">Boolean</span></span> | <span data-ttu-id="bc03d-112">Permite que essa fonte para o pato de outras fontes enquanto ativa.</span><span class="sxs-lookup"><span data-stu-id="bc03d-112">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="bc03d-113">Se for definido como true, o nível de pato precisará ser definido.</span><span class="sxs-lookup"><span data-stu-id="bc03d-113">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="bc03d-114">antes</span><span class="sxs-lookup"><span data-stu-id="bc03d-114">level</span></span>                  | <span data-ttu-id="bc03d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="bc03d-115">Int64</span></span>   | <span data-ttu-id="bc03d-116">O nível de pato da origem se `duckOthers` estiver definido como `true`.</span><span class="sxs-lookup"><span data-stu-id="bc03d-116">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="bc03d-117">participante</span><span class="sxs-lookup"><span data-stu-id="bc03d-117">participant</span></span>            | <span data-ttu-id="bc03d-118">String</span><span class="sxs-lookup"><span data-stu-id="bc03d-118">String</span></span>  | <span data-ttu-id="bc03d-119">O fluxo de áudio do participante de origem.</span><span class="sxs-lookup"><span data-stu-id="bc03d-119">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="bc03d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc03d-120">JSON representation</span></span>

<span data-ttu-id="bc03d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc03d-121">The following is a JSON representation of the resource.</span></span>

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
