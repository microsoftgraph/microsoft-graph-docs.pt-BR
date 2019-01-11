---
title: " tipo de recurso de averageComparativeScore"
description: Este recurso contém vários pontuações diferentes com base em por categoria de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura) e escopos diferentes (por exemplo, média pelo setor vertical, média pelo tamanho da estação de empresa e assim por diante).
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834591"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="9c2a6-103">tipo de recurso de averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="9c2a6-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="9c2a6-104">Este recurso contém vários pontuações diferentes com base em por categoria de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura) e escopos diferentes (por exemplo, média pelo setor vertical, média pelo tamanho da estação de empresa e assim por diante).</span><span class="sxs-lookup"><span data-stu-id="9c2a6-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="9c2a6-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c2a6-105">Property</span></span> |<span data-ttu-id="9c2a6-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c2a6-106">Type</span></span> |<span data-ttu-id="9c2a6-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c2a6-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="9c2a6-108">base</span><span class="sxs-lookup"><span data-stu-id="9c2a6-108">basis</span></span>   |   <span data-ttu-id="9c2a6-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c2a6-109">String</span></span>  |   <span data-ttu-id="9c2a6-110">Tipo de escopo (por AllTenants, TotalSeats, IndustryTypes).</span><span class="sxs-lookup"><span data-stu-id="9c2a6-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="9c2a6-111">Média</span><span class="sxs-lookup"><span data-stu-id="9c2a6-111">averageScore</span></span>    |   <span data-ttu-id="9c2a6-112">Duplo</span><span class="sxs-lookup"><span data-stu-id="9c2a6-112">Double</span></span>  | <span data-ttu-id="9c2a6-113">Pontuação média dentro de base especificada.</span><span class="sxs-lookup"><span data-stu-id="9c2a6-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="9c2a6-114">deviceScore</span><span class="sxs-lookup"><span data-stu-id="9c2a6-114">deviceScore</span></span> |   <span data-ttu-id="9c2a6-115">Duplo</span><span class="sxs-lookup"><span data-stu-id="9c2a6-115">Double</span></span>  | <span data-ttu-id="9c2a6-116">Pontuação média dentro de base especificada.</span><span class="sxs-lookup"><span data-stu-id="9c2a6-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="9c2a6-117">dataScore</span><span class="sxs-lookup"><span data-stu-id="9c2a6-117">dataScore</span></span>   |   <span data-ttu-id="9c2a6-118">Duplo</span><span class="sxs-lookup"><span data-stu-id="9c2a6-118">Double</span></span>  | <span data-ttu-id="9c2a6-119">Pontuação média dentro de base especificada.</span><span class="sxs-lookup"><span data-stu-id="9c2a6-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="9c2a6-120">identityScore</span><span class="sxs-lookup"><span data-stu-id="9c2a6-120">identityScore</span></span>   |   <span data-ttu-id="9c2a6-121">Duplo</span><span class="sxs-lookup"><span data-stu-id="9c2a6-121">Double</span></span>  | <span data-ttu-id="9c2a6-122">Pontuação média dentro de base especificada.</span><span class="sxs-lookup"><span data-stu-id="9c2a6-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9c2a6-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c2a6-123">JSON representation</span></span>

<span data-ttu-id="9c2a6-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c2a6-124">The following is a JSON representation of the resource.</span></span>

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
