---
title: " tipo de recurso averageComparativeScore"
description: Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535435"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="48699-103">tipo de recurso averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="48699-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="48699-104">Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).</span><span class="sxs-lookup"><span data-stu-id="48699-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="48699-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48699-105">Property</span></span> |<span data-ttu-id="48699-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="48699-106">Type</span></span> |<span data-ttu-id="48699-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="48699-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="48699-108">base</span><span class="sxs-lookup"><span data-stu-id="48699-108">basis</span></span>   |   <span data-ttu-id="48699-109">String</span><span class="sxs-lookup"><span data-stu-id="48699-109">String</span></span>  |   <span data-ttu-id="48699-110">Tipo de escopo (por isLocatários, TotalSeats, IndustryTypes).</span><span class="sxs-lookup"><span data-stu-id="48699-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="48699-111">averageScore</span><span class="sxs-lookup"><span data-stu-id="48699-111">averageScore</span></span>    |   <span data-ttu-id="48699-112">Duplo</span><span class="sxs-lookup"><span data-stu-id="48699-112">Double</span></span>  | <span data-ttu-id="48699-113">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="48699-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="48699-114">deviceScore</span><span class="sxs-lookup"><span data-stu-id="48699-114">deviceScore</span></span> |   <span data-ttu-id="48699-115">Duplo</span><span class="sxs-lookup"><span data-stu-id="48699-115">Double</span></span>  | <span data-ttu-id="48699-116">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="48699-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="48699-117">dataScore</span><span class="sxs-lookup"><span data-stu-id="48699-117">dataScore</span></span>   |   <span data-ttu-id="48699-118">Duplo</span><span class="sxs-lookup"><span data-stu-id="48699-118">Double</span></span>  | <span data-ttu-id="48699-119">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="48699-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="48699-120">identityScore</span><span class="sxs-lookup"><span data-stu-id="48699-120">identityScore</span></span>   |   <span data-ttu-id="48699-121">Duplo</span><span class="sxs-lookup"><span data-stu-id="48699-121">Double</span></span>  | <span data-ttu-id="48699-122">Pontuação média dentro da base especificada.</span><span class="sxs-lookup"><span data-stu-id="48699-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="48699-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48699-123">JSON representation</span></span>

<span data-ttu-id="48699-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48699-124">The following is a JSON representation of the resource.</span></span>

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
