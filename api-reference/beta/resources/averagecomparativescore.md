---
title: " tipo de recurso averageComparativeScore"
description: Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3e2256e7edefd0670bb697ec6d89c9fb80a5beeb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013147"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="91202-103">tipo de recurso averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="91202-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="91202-104">Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="91202-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="91202-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91202-105">Property</span></span> |<span data-ttu-id="91202-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="91202-106">Type</span></span> |<span data-ttu-id="91202-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="91202-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="91202-108">base</span><span class="sxs-lookup"><span data-stu-id="91202-108">basis</span></span>   |   <span data-ttu-id="91202-109">String</span><span class="sxs-lookup"><span data-stu-id="91202-109">String</span></span>  |   <span data-ttu-id="91202-110">Tipo de escopo (por islocatários, TotalSeats, IndustryTypes).</span><span class="sxs-lookup"><span data-stu-id="91202-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="91202-111">averageScore</span><span class="sxs-lookup"><span data-stu-id="91202-111">averageScore</span></span>    |   <span data-ttu-id="91202-112">Duplo</span><span class="sxs-lookup"><span data-stu-id="91202-112">Double</span></span>  | <span data-ttu-id="91202-113">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="91202-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="91202-114">deviceScore</span><span class="sxs-lookup"><span data-stu-id="91202-114">deviceScore</span></span> |   <span data-ttu-id="91202-115">Duplo</span><span class="sxs-lookup"><span data-stu-id="91202-115">Double</span></span>  | <span data-ttu-id="91202-116">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="91202-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="91202-117">datascore</span><span class="sxs-lookup"><span data-stu-id="91202-117">dataScore</span></span>   |   <span data-ttu-id="91202-118">Duplo</span><span class="sxs-lookup"><span data-stu-id="91202-118">Double</span></span>  | <span data-ttu-id="91202-119">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="91202-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="91202-120">identityScore</span><span class="sxs-lookup"><span data-stu-id="91202-120">identityScore</span></span>   |   <span data-ttu-id="91202-121">Duplo</span><span class="sxs-lookup"><span data-stu-id="91202-121">Double</span></span>  | <span data-ttu-id="91202-122">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="91202-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="91202-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91202-123">JSON representation</span></span>

<span data-ttu-id="91202-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91202-124">The following is a JSON representation of the resource.</span></span>

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
