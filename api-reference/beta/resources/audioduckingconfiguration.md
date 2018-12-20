---
title: tipo de recurso de audioDuckingConfiguration
description: Parâmetros para desviando de outras fontes (Introdução gradual e sair de outras fontes.)
author: VinodRavichandran
ms.openlocfilehash: e595e2a46f3e8bcbee2bb7ad0e3421216244db71
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380172"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="3c910-103">tipo de recurso de audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="3c910-103">audioDuckingConfiguration resource type</span></span>

> <span data-ttu-id="3c910-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3c910-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c910-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3c910-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c910-106">Parâmetros para desviando de outras fontes (Introdução gradual e sair de outras fontes.)</span><span class="sxs-lookup"><span data-stu-id="3c910-106">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="3c910-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c910-107">Properties</span></span>

| <span data-ttu-id="3c910-108">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="3c910-108">Property</span></span>      | <span data-ttu-id="3c910-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c910-109">Type</span></span>     | <span data-ttu-id="3c910-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c910-110">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="3c910-111">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="3c910-111">lowerLevel</span></span>    | <span data-ttu-id="3c910-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3c910-112">Int64</span></span>    | <span data-ttu-id="3c910-113">O volume das fontes em % quando as fontes estão sendo ducked.</span><span class="sxs-lookup"><span data-stu-id="3c910-113">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="3c910-114">rampActive</span><span class="sxs-lookup"><span data-stu-id="3c910-114">rampActive</span></span>    | <span data-ttu-id="3c910-115">Int64</span><span class="sxs-lookup"><span data-stu-id="3c910-115">Int64</span></span>    | <span data-ttu-id="3c910-116">A quantidade de tempo (em milissegundos) que leva para fontes ducked "desaparecer".</span><span class="sxs-lookup"><span data-stu-id="3c910-116">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="3c910-117">rampInactive</span><span class="sxs-lookup"><span data-stu-id="3c910-117">rampInactive</span></span>  | <span data-ttu-id="3c910-118">Int64</span><span class="sxs-lookup"><span data-stu-id="3c910-118">Int64</span></span>    | <span data-ttu-id="3c910-119">A quantidade de tempo (em milissegundos) que leva para ducked fontes para "desaparecer".</span><span class="sxs-lookup"><span data-stu-id="3c910-119">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="3c910-120">upperLevel</span><span class="sxs-lookup"><span data-stu-id="3c910-120">upperLevel</span></span>    | <span data-ttu-id="3c910-121">Int64</span><span class="sxs-lookup"><span data-stu-id="3c910-121">Int64</span></span>    | <span data-ttu-id="3c910-122">O volume das fontes em % quando as fontes não estão sendo ducked.</span><span class="sxs-lookup"><span data-stu-id="3c910-122">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="3c910-123">**Observação:** Duração conheça não pode ser mais de 5.000 milissegundos.</span><span class="sxs-lookup"><span data-stu-id="3c910-123">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c910-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c910-124">JSON representation</span></span>

<span data-ttu-id="3c910-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c910-125">The following is a JSON representation of the resource.</span></span>

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
