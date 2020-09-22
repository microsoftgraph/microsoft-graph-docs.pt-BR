---
title: tipo de recurso positionDetail
description: tipo de recurso positionDetail
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: fbd013292754dea43dd69b645dcd2ab735559b69
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971479"
---
# <a name="positiondetail-resource-type"></a><span data-ttu-id="8386d-103">tipo de recurso positionDetail</span><span class="sxs-lookup"><span data-stu-id="8386d-103">positionDetail resource type</span></span>

<span data-ttu-id="8386d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8386d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8386d-105">Representa informações sobre posições relacionadas a entidades dentro de um [perfil](profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="8386d-105">Represents information about positions related to entities within a user's [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8386d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8386d-106">Properties</span></span>

| <span data-ttu-id="8386d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8386d-107">Property</span></span>       | <span data-ttu-id="8386d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8386d-108">Type</span></span>                             | <span data-ttu-id="8386d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8386d-109">Description</span></span>                                            |
|:---------------|:---------------------------------|:-------------------------------------------------------|
|<span data-ttu-id="8386d-110">empresarial</span><span class="sxs-lookup"><span data-stu-id="8386d-110">company</span></span>         |[<span data-ttu-id="8386d-111">companyDetail</span><span class="sxs-lookup"><span data-stu-id="8386d-111">companyDetail</span></span>](companydetail.md) | <span data-ttu-id="8386d-112">Detalhes sobre a empresa ou o empregador.</span><span class="sxs-lookup"><span data-stu-id="8386d-112">Detail about the company or employer.</span></span>                  |
|<span data-ttu-id="8386d-113">description</span><span class="sxs-lookup"><span data-stu-id="8386d-113">description</span></span>     |<span data-ttu-id="8386d-114">String</span><span class="sxs-lookup"><span data-stu-id="8386d-114">String</span></span>                            | <span data-ttu-id="8386d-115">Descrição da posição em questão.</span><span class="sxs-lookup"><span data-stu-id="8386d-115">Description of the position in question.</span></span>               |
|<span data-ttu-id="8386d-116">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="8386d-116">endMonthYear</span></span>    |<span data-ttu-id="8386d-117">Data</span><span class="sxs-lookup"><span data-stu-id="8386d-117">Date</span></span>                              | <span data-ttu-id="8386d-118">Quando a posição terminou.</span><span class="sxs-lookup"><span data-stu-id="8386d-118">When the position ended.</span></span>                               |
|<span data-ttu-id="8386d-119">jobTitle</span><span class="sxs-lookup"><span data-stu-id="8386d-119">jobTitle</span></span>        |<span data-ttu-id="8386d-120">String</span><span class="sxs-lookup"><span data-stu-id="8386d-120">String</span></span>                            | <span data-ttu-id="8386d-121">O título mantido na posição.</span><span class="sxs-lookup"><span data-stu-id="8386d-121">The title held when in that position.</span></span>                  |
|<span data-ttu-id="8386d-122">role</span><span class="sxs-lookup"><span data-stu-id="8386d-122">role</span></span>            |<span data-ttu-id="8386d-123">String</span><span class="sxs-lookup"><span data-stu-id="8386d-123">String</span></span>                            | <span data-ttu-id="8386d-124">A função em que a posição é encaudada.</span><span class="sxs-lookup"><span data-stu-id="8386d-124">The role the position entailed.</span></span>                        |
|<span data-ttu-id="8386d-125">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="8386d-125">startMonthYear</span></span>  |<span data-ttu-id="8386d-126">Data</span><span class="sxs-lookup"><span data-stu-id="8386d-126">Date</span></span>                              | <span data-ttu-id="8386d-127">O mês e o ano de início da posição.</span><span class="sxs-lookup"><span data-stu-id="8386d-127">The start month and year of the position.</span></span>              |
|<span data-ttu-id="8386d-128">summary</span><span class="sxs-lookup"><span data-stu-id="8386d-128">summary</span></span>         |<span data-ttu-id="8386d-129">String</span><span class="sxs-lookup"><span data-stu-id="8386d-129">String</span></span>                            |<span data-ttu-id="8386d-130">Breve resumo da posição.</span><span class="sxs-lookup"><span data-stu-id="8386d-130">Short summary of the position.</span></span>                          |

## <a name="json-representation"></a><span data-ttu-id="8386d-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8386d-131">JSON representation</span></span>

<span data-ttu-id="8386d-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8386d-132">The following is a JSON representation of the resource.</span></span>

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

