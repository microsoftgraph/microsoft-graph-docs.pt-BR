---
title: tipo de recurso averageComparativeScore
description: Contém várias pontuações diferentes com base em escopos diferentes.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bc104f3a9c19c38ef569d08d24da83d0e07d75f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091898"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="9d877-103">tipo de recurso averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="9d877-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="9d877-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d877-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d877-105">Contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho da indústria vertical, média por tamanho de estação da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="9d877-105">Contains various different scores based on different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

## <a name="properties"></a><span data-ttu-id="9d877-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d877-106">Properties</span></span>

|<span data-ttu-id="9d877-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d877-107">Property</span></span> |<span data-ttu-id="9d877-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d877-108">Type</span></span> |<span data-ttu-id="9d877-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d877-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="9d877-110">base</span><span class="sxs-lookup"><span data-stu-id="9d877-110">basis</span></span>|<span data-ttu-id="9d877-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d877-111">String</span></span>|<span data-ttu-id="9d877-112">Tipo de escopo.</span><span class="sxs-lookup"><span data-stu-id="9d877-112">Scope type.</span></span> <span data-ttu-id="9d877-113">Os valores possíveis são: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span><span class="sxs-lookup"><span data-stu-id="9d877-113">The possible values are: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span></span>|
|<span data-ttu-id="9d877-114">averageScore</span><span class="sxs-lookup"><span data-stu-id="9d877-114">averageScore</span></span>|<span data-ttu-id="9d877-115">Duplo</span><span class="sxs-lookup"><span data-stu-id="9d877-115">Double</span></span>|<span data-ttu-id="9d877-116">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="9d877-116">Average score within specified basis.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d877-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d877-117">JSON representation</span></span>

<span data-ttu-id="9d877-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d877-118">The following is a JSON representation of the resource.</span></span>

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

