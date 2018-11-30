---
title: " tipo de recurso de averageComparativeScore"
description: Este recurso contém vários pontuações diferentes com base em por categoria de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura) e escopos diferentes (por exemplo, média pelo setor vertical, média pelo tamanho da estação de empresa e assim por diante).
ms.openlocfilehash: 08e4ec60788b21476d8f1491ab5548c7a4ca2e01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034440"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="5a92a-103">tipo de recurso de averageComparativeScore</span><span class="sxs-lookup"><span data-stu-id="5a92a-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="5a92a-104">Este recurso contém vários pontuações diferentes com base em por categoria de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura) e escopos diferentes (por exemplo, média pelo setor vertical, média pelo tamanho da estação de empresa e assim por diante).</span><span class="sxs-lookup"><span data-stu-id="5a92a-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="5a92a-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a92a-105">Property</span></span> |<span data-ttu-id="5a92a-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a92a-106">Type</span></span> |<span data-ttu-id="5a92a-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a92a-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="5a92a-108">base</span><span class="sxs-lookup"><span data-stu-id="5a92a-108">basis</span></span>   |   <span data-ttu-id="5a92a-109">String</span><span class="sxs-lookup"><span data-stu-id="5a92a-109">String</span></span>  |   <span data-ttu-id="5a92a-110">Tipo de escopo (por AllTenants, TotalSeats, IndustryTypes).</span><span class="sxs-lookup"><span data-stu-id="5a92a-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="5a92a-111">Média</span><span class="sxs-lookup"><span data-stu-id="5a92a-111">averageScore</span></span>    |   <span data-ttu-id="5a92a-112">Duplo</span><span class="sxs-lookup"><span data-stu-id="5a92a-112">Double</span></span>  | <span data-ttu-id="5a92a-113">Pontuação média dentro de base especificada.</span><span class="sxs-lookup"><span data-stu-id="5a92a-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="5a92a-114">deviceScore</span><span class="sxs-lookup"><span data-stu-id="5a92a-114">deviceScore</span></span> |   <span data-ttu-id="5a92a-115">Duplo</span><span class="sxs-lookup"><span data-stu-id="5a92a-115">Double</span></span>  | <span data-ttu-id="5a92a-116">Pontuação média dentro de base especificada.</span><span class="sxs-lookup"><span data-stu-id="5a92a-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="5a92a-117">dataScore</span><span class="sxs-lookup"><span data-stu-id="5a92a-117">dataScore</span></span>   |   <span data-ttu-id="5a92a-118">Duplo</span><span class="sxs-lookup"><span data-stu-id="5a92a-118">Double</span></span>  | <span data-ttu-id="5a92a-119">Pontuação média dentro de base especificada.</span><span class="sxs-lookup"><span data-stu-id="5a92a-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="5a92a-120">identityScore</span><span class="sxs-lookup"><span data-stu-id="5a92a-120">identityScore</span></span>   |   <span data-ttu-id="5a92a-121">Duplo</span><span class="sxs-lookup"><span data-stu-id="5a92a-121">Double</span></span>  | <span data-ttu-id="5a92a-122">Pontuação média dentro de base especificada.</span><span class="sxs-lookup"><span data-stu-id="5a92a-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5a92a-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a92a-123">JSON representation</span></span>

<span data-ttu-id="5a92a-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a92a-124">The following is a JSON representation of the resource.</span></span>

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
