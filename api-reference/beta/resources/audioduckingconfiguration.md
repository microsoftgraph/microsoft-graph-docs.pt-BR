---
title: tipo de recurso de audioDuckingConfiguration
description: Parâmetros para desviando de outras fontes (Introdução gradual e sair de outras fontes.)
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d61e4150250df25e020f45a65676d1c55c0e4c9d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522459"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="7c615-103">tipo de recurso de audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c615-103">audioDuckingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c615-104">Parâmetros para desviando de outras fontes (Introdução gradual e sair de outras fontes.)</span><span class="sxs-lookup"><span data-stu-id="7c615-104">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="7c615-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c615-105">Properties</span></span>

| <span data-ttu-id="7c615-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c615-106">Property</span></span>      | <span data-ttu-id="7c615-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c615-107">Type</span></span>     | <span data-ttu-id="7c615-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c615-108">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="7c615-109">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="7c615-109">lowerLevel</span></span>    | <span data-ttu-id="7c615-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7c615-110">Int64</span></span>    | <span data-ttu-id="7c615-111">O volume das fontes em % quando as fontes estão sendo ducked.</span><span class="sxs-lookup"><span data-stu-id="7c615-111">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="7c615-112">rampActive</span><span class="sxs-lookup"><span data-stu-id="7c615-112">rampActive</span></span>    | <span data-ttu-id="7c615-113">Int64</span><span class="sxs-lookup"><span data-stu-id="7c615-113">Int64</span></span>    | <span data-ttu-id="7c615-114">A quantidade de tempo (em milissegundos) que leva para fontes ducked "desaparecer".</span><span class="sxs-lookup"><span data-stu-id="7c615-114">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="7c615-115">rampInactive</span><span class="sxs-lookup"><span data-stu-id="7c615-115">rampInactive</span></span>  | <span data-ttu-id="7c615-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7c615-116">Int64</span></span>    | <span data-ttu-id="7c615-117">A quantidade de tempo (em milissegundos) que leva para ducked fontes para "desaparecer".</span><span class="sxs-lookup"><span data-stu-id="7c615-117">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="7c615-118">upperLevel</span><span class="sxs-lookup"><span data-stu-id="7c615-118">upperLevel</span></span>    | <span data-ttu-id="7c615-119">Int64</span><span class="sxs-lookup"><span data-stu-id="7c615-119">Int64</span></span>    | <span data-ttu-id="7c615-120">O volume das fontes em % quando as fontes não estão sendo ducked.</span><span class="sxs-lookup"><span data-stu-id="7c615-120">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="7c615-121">**Observação:** Duração conheça não pode ser mais de 5.000 milissegundos.</span><span class="sxs-lookup"><span data-stu-id="7c615-121">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c615-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c615-122">JSON representation</span></span>

<span data-ttu-id="7c615-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c615-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/audioduckingconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
