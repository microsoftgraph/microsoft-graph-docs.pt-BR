---
title: tipo de recurso de audioDuckingConfiguration
description: Parâmetros para desviando de outras fontes (Introdução gradual e sair de outras fontes.)
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4132946573342976bb1f20c593454a8e18030d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916870"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="93bce-103">tipo de recurso de audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="93bce-103">audioDuckingConfiguration resource type</span></span>

> <span data-ttu-id="93bce-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="93bce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93bce-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="93bce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93bce-106">Parâmetros para desviando de outras fontes (Introdução gradual e sair de outras fontes.)</span><span class="sxs-lookup"><span data-stu-id="93bce-106">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="93bce-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93bce-107">Properties</span></span>

| <span data-ttu-id="93bce-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93bce-108">Property</span></span>      | <span data-ttu-id="93bce-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="93bce-109">Type</span></span>     | <span data-ttu-id="93bce-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="93bce-110">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="93bce-111">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="93bce-111">lowerLevel</span></span>    | <span data-ttu-id="93bce-112">Int64</span><span class="sxs-lookup"><span data-stu-id="93bce-112">Int64</span></span>    | <span data-ttu-id="93bce-113">O volume das fontes em % quando as fontes estão sendo ducked.</span><span class="sxs-lookup"><span data-stu-id="93bce-113">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="93bce-114">rampActive</span><span class="sxs-lookup"><span data-stu-id="93bce-114">rampActive</span></span>    | <span data-ttu-id="93bce-115">Int64</span><span class="sxs-lookup"><span data-stu-id="93bce-115">Int64</span></span>    | <span data-ttu-id="93bce-116">A quantidade de tempo (em milissegundos) que leva para fontes ducked "desaparecer".</span><span class="sxs-lookup"><span data-stu-id="93bce-116">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="93bce-117">rampInactive</span><span class="sxs-lookup"><span data-stu-id="93bce-117">rampInactive</span></span>  | <span data-ttu-id="93bce-118">Int64</span><span class="sxs-lookup"><span data-stu-id="93bce-118">Int64</span></span>    | <span data-ttu-id="93bce-119">A quantidade de tempo (em milissegundos) que leva para ducked fontes para "desaparecer".</span><span class="sxs-lookup"><span data-stu-id="93bce-119">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="93bce-120">upperLevel</span><span class="sxs-lookup"><span data-stu-id="93bce-120">upperLevel</span></span>    | <span data-ttu-id="93bce-121">Int64</span><span class="sxs-lookup"><span data-stu-id="93bce-121">Int64</span></span>    | <span data-ttu-id="93bce-122">O volume das fontes em % quando as fontes não estão sendo ducked.</span><span class="sxs-lookup"><span data-stu-id="93bce-122">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="93bce-123">**Observação:** Duração conheça não pode ser mais de 5.000 milissegundos.</span><span class="sxs-lookup"><span data-stu-id="93bce-123">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="93bce-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93bce-124">JSON representation</span></span>

<span data-ttu-id="93bce-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93bce-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
