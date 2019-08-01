---
title: tipo de recurso averageComparativeScore
description: Contém várias pontuações diferentes com base em escopos diferentes.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f128fd22562889a5a537f3815a4003aec9bfc8a9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030013"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="968e8-103">tipo de recurso averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="968e8-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="968e8-104">Contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho da indústria vertical, média por tamanho de estação da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="968e8-104">Contains various different scores based on different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

## <a name="properties"></a><span data-ttu-id="968e8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="968e8-105">Properties</span></span>

|<span data-ttu-id="968e8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="968e8-106">Property</span></span> |<span data-ttu-id="968e8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="968e8-107">Type</span></span> |<span data-ttu-id="968e8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="968e8-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="968e8-109">base</span><span class="sxs-lookup"><span data-stu-id="968e8-109">basis</span></span>|<span data-ttu-id="968e8-110">String</span><span class="sxs-lookup"><span data-stu-id="968e8-110">String</span></span>|<span data-ttu-id="968e8-111">Tipo de escopo.</span><span class="sxs-lookup"><span data-stu-id="968e8-111">Scope type.</span></span> <span data-ttu-id="968e8-112">Os valores possíveis são: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span><span class="sxs-lookup"><span data-stu-id="968e8-112">The possible values are: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span></span>|
|<span data-ttu-id="968e8-113">averageScore</span><span class="sxs-lookup"><span data-stu-id="968e8-113">averageScore</span></span>|<span data-ttu-id="968e8-114">Duplo</span><span class="sxs-lookup"><span data-stu-id="968e8-114">Double</span></span>|<span data-ttu-id="968e8-115">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="968e8-115">Average score within specified basis.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="968e8-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="968e8-116">JSON representation</span></span>

<span data-ttu-id="968e8-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="968e8-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
