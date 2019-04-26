---
title: tipo de recurso audioDuckingConfiguration
description: Parâmetros para o pato de outras fontes (phasing dentro e fora de outras fontes).
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c19a8d364c681fd199bf998a6951123a1cb5da86
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339030"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="04296-103">tipo de recurso audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="04296-103">audioDuckingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04296-104">Parâmetros para o pato de outras fontes (phasing dentro e fora de outras fontes).</span><span class="sxs-lookup"><span data-stu-id="04296-104">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="04296-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04296-105">Properties</span></span>

| <span data-ttu-id="04296-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04296-106">Property</span></span>      | <span data-ttu-id="04296-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="04296-107">Type</span></span>     | <span data-ttu-id="04296-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="04296-108">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="04296-109">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="04296-109">lowerLevel</span></span>    | <span data-ttu-id="04296-110">Int64</span><span class="sxs-lookup"><span data-stu-id="04296-110">Int64</span></span>    | <span data-ttu-id="04296-111">O volume de fontes em porcentagem quando as fontes estão sendo disparadas.</span><span class="sxs-lookup"><span data-stu-id="04296-111">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="04296-112">rampActive</span><span class="sxs-lookup"><span data-stu-id="04296-112">rampActive</span></span>    | <span data-ttu-id="04296-113">Int64</span><span class="sxs-lookup"><span data-stu-id="04296-113">Int64</span></span>    | <span data-ttu-id="04296-114">A quantidade de tempo (em milissegundos) que demora para que as fontes em intervalo sejam "Fade out".</span><span class="sxs-lookup"><span data-stu-id="04296-114">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="04296-115">rampInactive</span><span class="sxs-lookup"><span data-stu-id="04296-115">rampInactive</span></span>  | <span data-ttu-id="04296-116">Int64</span><span class="sxs-lookup"><span data-stu-id="04296-116">Int64</span></span>    | <span data-ttu-id="04296-117">A quantidade de tempo (em milissegundos) que demora para as fontes em um intervalo para "Fade in".</span><span class="sxs-lookup"><span data-stu-id="04296-117">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="04296-118">upperLevel</span><span class="sxs-lookup"><span data-stu-id="04296-118">upperLevel</span></span>    | <span data-ttu-id="04296-119">Int64</span><span class="sxs-lookup"><span data-stu-id="04296-119">Int64</span></span>    | <span data-ttu-id="04296-120">O volume de fontes em porcentagem quando as fontes não estão sendo disparadas.</span><span class="sxs-lookup"><span data-stu-id="04296-120">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="04296-121">**Observação:** A duração da rampa não pode ser maior que 5.000 milissegundos.</span><span class="sxs-lookup"><span data-stu-id="04296-121">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04296-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04296-122">JSON representation</span></span>

<span data-ttu-id="04296-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04296-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
