---
title: tipo de recurso de audioSourceLevel
description: Configuração de nível de outras fontes.
author: VinodRavichandran
ms.openlocfilehash: 5d5abe7eba03891427b30ba1c8f63b15b3707e46
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380237"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="1750a-103">tipo de recurso de audioSourceLevel</span><span class="sxs-lookup"><span data-stu-id="1750a-103">audioSourceLevel resource type</span></span>

> <span data-ttu-id="1750a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1750a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1750a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1750a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1750a-106">Configuração de nível de outras fontes.</span><span class="sxs-lookup"><span data-stu-id="1750a-106">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="1750a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1750a-107">Properties</span></span>

| <span data-ttu-id="1750a-108">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="1750a-108">Property</span></span>               | <span data-ttu-id="1750a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1750a-109">Type</span></span>    | <span data-ttu-id="1750a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1750a-110">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1750a-111">duckOthers</span><span class="sxs-lookup"><span data-stu-id="1750a-111">duckOthers</span></span>             | <span data-ttu-id="1750a-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="1750a-112">Boolean</span></span> | <span data-ttu-id="1750a-113">Habilita a essa fonte para jantar de outras fontes enquanto estão ativos.</span><span class="sxs-lookup"><span data-stu-id="1750a-113">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="1750a-114">Se definido como true, desviando nível deve ser definido.</span><span class="sxs-lookup"><span data-stu-id="1750a-114">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="1750a-115">nível</span><span class="sxs-lookup"><span data-stu-id="1750a-115">level</span></span>                  | <span data-ttu-id="1750a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1750a-116">Int64</span></span>   | <span data-ttu-id="1750a-117">Desviando nível da fonte se `duckOthers` estiver definida como `true`.</span><span class="sxs-lookup"><span data-stu-id="1750a-117">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="1750a-118">participante</span><span class="sxs-lookup"><span data-stu-id="1750a-118">participant</span></span>            | <span data-ttu-id="1750a-119">String</span><span class="sxs-lookup"><span data-stu-id="1750a-119">String</span></span>  | <span data-ttu-id="1750a-120">O fluxo de áudio participante do código-fonte.</span><span class="sxs-lookup"><span data-stu-id="1750a-120">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="1750a-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1750a-121">JSON representation</span></span>

<span data-ttu-id="1750a-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1750a-122">The following is a JSON representation of the resource.</span></span>

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
