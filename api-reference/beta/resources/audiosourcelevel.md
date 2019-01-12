---
title: tipo de recurso de audioSourceLevel
description: Configuração de nível de outras fontes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 79ad56c11e8b277a1354ffc3a6292a0434466c8a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947649"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="3c111-103">tipo de recurso de audioSourceLevel</span><span class="sxs-lookup"><span data-stu-id="3c111-103">audioSourceLevel resource type</span></span>

> <span data-ttu-id="3c111-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3c111-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c111-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3c111-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c111-106">Configuração de nível de outras fontes.</span><span class="sxs-lookup"><span data-stu-id="3c111-106">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="3c111-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c111-107">Properties</span></span>

| <span data-ttu-id="3c111-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c111-108">Property</span></span>               | <span data-ttu-id="3c111-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c111-109">Type</span></span>    | <span data-ttu-id="3c111-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c111-110">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3c111-111">duckOthers</span><span class="sxs-lookup"><span data-stu-id="3c111-111">duckOthers</span></span>             | <span data-ttu-id="3c111-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="3c111-112">Boolean</span></span> | <span data-ttu-id="3c111-113">Habilita a essa fonte para jantar de outras fontes enquanto estão ativos.</span><span class="sxs-lookup"><span data-stu-id="3c111-113">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="3c111-114">Se definido como true, desviando nível deve ser definido.</span><span class="sxs-lookup"><span data-stu-id="3c111-114">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="3c111-115">nível</span><span class="sxs-lookup"><span data-stu-id="3c111-115">level</span></span>                  | <span data-ttu-id="3c111-116">Int64</span><span class="sxs-lookup"><span data-stu-id="3c111-116">Int64</span></span>   | <span data-ttu-id="3c111-117">Desviando nível da fonte se `duckOthers` estiver definida como `true`.</span><span class="sxs-lookup"><span data-stu-id="3c111-117">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="3c111-118">participante</span><span class="sxs-lookup"><span data-stu-id="3c111-118">participant</span></span>            | <span data-ttu-id="3c111-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c111-119">String</span></span>  | <span data-ttu-id="3c111-120">O fluxo de áudio participante do código-fonte.</span><span class="sxs-lookup"><span data-stu-id="3c111-120">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="3c111-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c111-121">JSON representation</span></span>

<span data-ttu-id="3c111-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c111-122">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
