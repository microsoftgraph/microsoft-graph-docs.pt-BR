---
title: tipo de recurso positionDetail
description: tipo de recurso positionDetail
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: f4094da9c3ffc6a000fc0f7954ca8838a2d659af
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939786"
---
# <a name="positiondetail-resource-type"></a><span data-ttu-id="41764-103">tipo de recurso positionDetail</span><span class="sxs-lookup"><span data-stu-id="41764-103">positionDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41764-104">Representa informações sobre posições relacionadas a entidades dentro de um [perfil](profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="41764-104">Represents information about positions related to entities within a user's [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="41764-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41764-105">Properties</span></span>

| <span data-ttu-id="41764-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41764-106">Property</span></span>       | <span data-ttu-id="41764-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="41764-107">Type</span></span>                             | <span data-ttu-id="41764-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="41764-108">Description</span></span>                                            |
|:---------------|:---------------------------------|:-------------------------------------------------------|
|<span data-ttu-id="41764-109">empresarial</span><span class="sxs-lookup"><span data-stu-id="41764-109">company</span></span>         |[<span data-ttu-id="41764-110">companyDetail</span><span class="sxs-lookup"><span data-stu-id="41764-110">companyDetail</span></span>](companydetail.md) | <span data-ttu-id="41764-111">Detalhes sobre a empresa ou o empregador.</span><span class="sxs-lookup"><span data-stu-id="41764-111">Detail about the company or employer.</span></span>                  |
|<span data-ttu-id="41764-112">description</span><span class="sxs-lookup"><span data-stu-id="41764-112">description</span></span>     |<span data-ttu-id="41764-113">String</span><span class="sxs-lookup"><span data-stu-id="41764-113">String</span></span>                            | <span data-ttu-id="41764-114">Descrição da posição em questão.</span><span class="sxs-lookup"><span data-stu-id="41764-114">Description of the position in question.</span></span>               |
|<span data-ttu-id="41764-115">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="41764-115">endMonthYear</span></span>    |<span data-ttu-id="41764-116">Data</span><span class="sxs-lookup"><span data-stu-id="41764-116">Date</span></span>                              | <span data-ttu-id="41764-117">Quando a posição terminou.</span><span class="sxs-lookup"><span data-stu-id="41764-117">When the position ended.</span></span>                               |
|<span data-ttu-id="41764-118">jobTitle</span><span class="sxs-lookup"><span data-stu-id="41764-118">jobTitle</span></span>        |<span data-ttu-id="41764-119">String</span><span class="sxs-lookup"><span data-stu-id="41764-119">String</span></span>                            | <span data-ttu-id="41764-120">O título mantido na posição.</span><span class="sxs-lookup"><span data-stu-id="41764-120">The title held when in that position.</span></span>                  |
|<span data-ttu-id="41764-121">role</span><span class="sxs-lookup"><span data-stu-id="41764-121">role</span></span>            |<span data-ttu-id="41764-122">String</span><span class="sxs-lookup"><span data-stu-id="41764-122">String</span></span>                            | <span data-ttu-id="41764-123">A função em que a posição é encaudada.</span><span class="sxs-lookup"><span data-stu-id="41764-123">The role the position entailed.</span></span>                        |
|<span data-ttu-id="41764-124">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="41764-124">startMonthYear</span></span>  |<span data-ttu-id="41764-125">Data</span><span class="sxs-lookup"><span data-stu-id="41764-125">Date</span></span>                              | <span data-ttu-id="41764-126">O mês e o ano de início da posição.</span><span class="sxs-lookup"><span data-stu-id="41764-126">The start month and year of the position.</span></span>              |
|<span data-ttu-id="41764-127">summary</span><span class="sxs-lookup"><span data-stu-id="41764-127">summary</span></span>         |<span data-ttu-id="41764-128">String</span><span class="sxs-lookup"><span data-stu-id="41764-128">String</span></span>                            |<span data-ttu-id="41764-129">Breve resumo da posição.</span><span class="sxs-lookup"><span data-stu-id="41764-129">Short summary of the position.</span></span>                          |

## <a name="json-representation"></a><span data-ttu-id="41764-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41764-130">JSON representation</span></span>

<span data-ttu-id="41764-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41764-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.positionDetail",
  "baseType": null
}-->

```json
{
  "company": {"@odata.type": "microsoft.graph.companyDetail"},
  "description": "String",
  "endMonthYear": "String (timestamp)",
  "jobTitle": "String",
  "role": "String",
  "startMonthYear": "String (timestamp)",
  "summary": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "positionDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->