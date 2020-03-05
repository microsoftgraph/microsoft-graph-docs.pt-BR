---
title: tipo de recurso audioDuckingConfiguration
description: Parâmetros para o pato de outras fontes (phasing dentro e fora de outras fontes).
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99aa202e0048b328d97453f57d249df749f7bce5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508112"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="6eac7-103">tipo de recurso audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="6eac7-103">audioDuckingConfiguration resource type</span></span>

<span data-ttu-id="6eac7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6eac7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6eac7-105">Parâmetros para o pato de outras fontes (phasing dentro e fora de outras fontes).</span><span class="sxs-lookup"><span data-stu-id="6eac7-105">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="6eac7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6eac7-106">Properties</span></span>

| <span data-ttu-id="6eac7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6eac7-107">Property</span></span>      | <span data-ttu-id="6eac7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6eac7-108">Type</span></span>     | <span data-ttu-id="6eac7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6eac7-109">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="6eac7-110">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="6eac7-110">lowerLevel</span></span>    | <span data-ttu-id="6eac7-111">Int64</span><span class="sxs-lookup"><span data-stu-id="6eac7-111">Int64</span></span>    | <span data-ttu-id="6eac7-112">O volume de fontes em porcentagem quando as fontes estão sendo disparadas.</span><span class="sxs-lookup"><span data-stu-id="6eac7-112">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="6eac7-113">rampActive</span><span class="sxs-lookup"><span data-stu-id="6eac7-113">rampActive</span></span>    | <span data-ttu-id="6eac7-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6eac7-114">Int64</span></span>    | <span data-ttu-id="6eac7-115">A quantidade de tempo (em milissegundos) que demora para que as fontes em intervalo sejam "Fade out".</span><span class="sxs-lookup"><span data-stu-id="6eac7-115">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="6eac7-116">rampInactive</span><span class="sxs-lookup"><span data-stu-id="6eac7-116">rampInactive</span></span>  | <span data-ttu-id="6eac7-117">Int64</span><span class="sxs-lookup"><span data-stu-id="6eac7-117">Int64</span></span>    | <span data-ttu-id="6eac7-118">A quantidade de tempo (em milissegundos) que demora para as fontes em um intervalo para "Fade in".</span><span class="sxs-lookup"><span data-stu-id="6eac7-118">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="6eac7-119">upperLevel</span><span class="sxs-lookup"><span data-stu-id="6eac7-119">upperLevel</span></span>    | <span data-ttu-id="6eac7-120">Int64</span><span class="sxs-lookup"><span data-stu-id="6eac7-120">Int64</span></span>    | <span data-ttu-id="6eac7-121">O volume de fontes em porcentagem quando as fontes não estão sendo disparadas.</span><span class="sxs-lookup"><span data-stu-id="6eac7-121">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="6eac7-122">**Observação:** A duração da rampa não pode ser maior que 5.000 milissegundos.</span><span class="sxs-lookup"><span data-stu-id="6eac7-122">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6eac7-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6eac7-123">JSON representation</span></span>

<span data-ttu-id="6eac7-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6eac7-124">The following is a JSON representation of the resource.</span></span>

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
