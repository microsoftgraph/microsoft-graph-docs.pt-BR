---
title: " tipo de recurso averageComparativeScore"
description: Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f2ac965d4dae0b038f3aad9fe13ed57a283a42bc
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812552"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="e4414-103">tipo de recurso averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="e4414-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="e4414-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4414-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4414-105">Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="e4414-105">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="e4414-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4414-106">Property</span></span> |<span data-ttu-id="e4414-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4414-107">Type</span></span> |<span data-ttu-id="e4414-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4414-108">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="e4414-109">base</span><span class="sxs-lookup"><span data-stu-id="e4414-109">basis</span></span>   |   <span data-ttu-id="e4414-110">String</span><span class="sxs-lookup"><span data-stu-id="e4414-110">String</span></span>  |   <span data-ttu-id="e4414-111">Tipo de escopo (por islocatários, TotalSeats, IndustryTypes).</span><span class="sxs-lookup"><span data-stu-id="e4414-111">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="e4414-112">averageScore</span><span class="sxs-lookup"><span data-stu-id="e4414-112">averageScore</span></span>    |   <span data-ttu-id="e4414-113">Duplo</span><span class="sxs-lookup"><span data-stu-id="e4414-113">Double</span></span>  | <span data-ttu-id="e4414-114">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="e4414-114">Average score within specified basis.</span></span> |
|   <span data-ttu-id="e4414-115">deviceScore</span><span class="sxs-lookup"><span data-stu-id="e4414-115">deviceScore</span></span> |   <span data-ttu-id="e4414-116">Duplo</span><span class="sxs-lookup"><span data-stu-id="e4414-116">Double</span></span>  | <span data-ttu-id="e4414-117">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="e4414-117">Average score within specified basis.</span></span> |
|   <span data-ttu-id="e4414-118">datascore</span><span class="sxs-lookup"><span data-stu-id="e4414-118">dataScore</span></span>   |   <span data-ttu-id="e4414-119">Duplo</span><span class="sxs-lookup"><span data-stu-id="e4414-119">Double</span></span>  | <span data-ttu-id="e4414-120">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="e4414-120">Average score within specified basis.</span></span> |
|   <span data-ttu-id="e4414-121">identityScore</span><span class="sxs-lookup"><span data-stu-id="e4414-121">identityScore</span></span>   |   <span data-ttu-id="e4414-122">Duplo</span><span class="sxs-lookup"><span data-stu-id="e4414-122">Double</span></span>  | <span data-ttu-id="e4414-123">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="e4414-123">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e4414-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4414-124">JSON representation</span></span>

<span data-ttu-id="e4414-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e4414-125">The following is a JSON representation of the resource.</span></span>

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
