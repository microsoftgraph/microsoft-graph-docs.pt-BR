---
title: " tipo de recurso averageComparativeScore"
description: Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 69a9e63960499fb50b34cd38986b1312a4313090
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076481"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="8e713-103">tipo de recurso averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="8e713-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="8e713-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e713-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e713-105">Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="8e713-105">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="8e713-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e713-106">Property</span></span> |<span data-ttu-id="8e713-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e713-107">Type</span></span> |<span data-ttu-id="8e713-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e713-108">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="8e713-109">base</span><span class="sxs-lookup"><span data-stu-id="8e713-109">basis</span></span>   |   <span data-ttu-id="8e713-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e713-110">String</span></span>  |   <span data-ttu-id="8e713-111">Tipo de escopo (por islocatários, TotalSeats, IndustryTypes).</span><span class="sxs-lookup"><span data-stu-id="8e713-111">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="8e713-112">averageScore</span><span class="sxs-lookup"><span data-stu-id="8e713-112">averageScore</span></span>    |   <span data-ttu-id="8e713-113">Duplo</span><span class="sxs-lookup"><span data-stu-id="8e713-113">Double</span></span>  | <span data-ttu-id="8e713-114">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="8e713-114">Average score within specified basis.</span></span> |
|   <span data-ttu-id="8e713-115">deviceScore</span><span class="sxs-lookup"><span data-stu-id="8e713-115">deviceScore</span></span> |   <span data-ttu-id="8e713-116">Duplo</span><span class="sxs-lookup"><span data-stu-id="8e713-116">Double</span></span>  | <span data-ttu-id="8e713-117">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="8e713-117">Average score within specified basis.</span></span> |
|   <span data-ttu-id="8e713-118">datascore</span><span class="sxs-lookup"><span data-stu-id="8e713-118">dataScore</span></span>   |   <span data-ttu-id="8e713-119">Duplo</span><span class="sxs-lookup"><span data-stu-id="8e713-119">Double</span></span>  | <span data-ttu-id="8e713-120">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="8e713-120">Average score within specified basis.</span></span> |
|   <span data-ttu-id="8e713-121">identityScore</span><span class="sxs-lookup"><span data-stu-id="8e713-121">identityScore</span></span>   |   <span data-ttu-id="8e713-122">Duplo</span><span class="sxs-lookup"><span data-stu-id="8e713-122">Double</span></span>  | <span data-ttu-id="8e713-123">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="8e713-123">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8e713-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e713-124">JSON representation</span></span>

<span data-ttu-id="8e713-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e713-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double",
  "deviceScore": "Double",
  "dataScore": "Double",
  "identityScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


