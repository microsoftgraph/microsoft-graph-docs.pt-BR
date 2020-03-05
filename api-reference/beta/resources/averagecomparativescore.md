---
title: " tipo de recurso averageComparativeScore"
description: Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e051ee3d1265c1dc65a5ab0cb9352d9cd536b21c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508049"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="4ae2d-103">tipo de recurso averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="4ae2d-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="4ae2d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4ae2d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ae2d-105">Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="4ae2d-105">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="4ae2d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ae2d-106">Property</span></span> |<span data-ttu-id="4ae2d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ae2d-107">Type</span></span> |<span data-ttu-id="4ae2d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ae2d-108">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="4ae2d-109">base</span><span class="sxs-lookup"><span data-stu-id="4ae2d-109">basis</span></span>   |   <span data-ttu-id="4ae2d-110">String</span><span class="sxs-lookup"><span data-stu-id="4ae2d-110">String</span></span>  |   <span data-ttu-id="4ae2d-111">Tipo de escopo (por islocatários, TotalSeats, IndustryTypes).</span><span class="sxs-lookup"><span data-stu-id="4ae2d-111">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="4ae2d-112">averageScore</span><span class="sxs-lookup"><span data-stu-id="4ae2d-112">averageScore</span></span>    |   <span data-ttu-id="4ae2d-113">Duplo</span><span class="sxs-lookup"><span data-stu-id="4ae2d-113">Double</span></span>  | <span data-ttu-id="4ae2d-114">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-114">Average score within specified basis.</span></span> |
|   <span data-ttu-id="4ae2d-115">deviceScore</span><span class="sxs-lookup"><span data-stu-id="4ae2d-115">deviceScore</span></span> |   <span data-ttu-id="4ae2d-116">Duplo</span><span class="sxs-lookup"><span data-stu-id="4ae2d-116">Double</span></span>  | <span data-ttu-id="4ae2d-117">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-117">Average score within specified basis.</span></span> |
|   <span data-ttu-id="4ae2d-118">datascore</span><span class="sxs-lookup"><span data-stu-id="4ae2d-118">dataScore</span></span>   |   <span data-ttu-id="4ae2d-119">Duplo</span><span class="sxs-lookup"><span data-stu-id="4ae2d-119">Double</span></span>  | <span data-ttu-id="4ae2d-120">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-120">Average score within specified basis.</span></span> |
|   <span data-ttu-id="4ae2d-121">identityScore</span><span class="sxs-lookup"><span data-stu-id="4ae2d-121">identityScore</span></span>   |   <span data-ttu-id="4ae2d-122">Duplo</span><span class="sxs-lookup"><span data-stu-id="4ae2d-122">Double</span></span>  | <span data-ttu-id="4ae2d-123">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-123">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4ae2d-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ae2d-124">JSON representation</span></span>

<span data-ttu-id="4ae2d-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ae2d-125">The following is a JSON representation of the resource.</span></span>

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
