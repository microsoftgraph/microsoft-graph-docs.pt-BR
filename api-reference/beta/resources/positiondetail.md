---
title: tipo de recurso positionDetail
description: tipo de recurso positionDetail
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6c77c116f013000ec4d419ec20c1e45c07187a22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521590"
---
# <a name="positiondetail-resource-type"></a><span data-ttu-id="ef3c9-103">tipo de recurso positionDetail</span><span class="sxs-lookup"><span data-stu-id="ef3c9-103">positionDetail resource type</span></span>

<span data-ttu-id="ef3c9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ef3c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef3c9-105">Representa informações sobre posições relacionadas a entidades dentro de um [perfil](profile.md)de usuário.</span><span class="sxs-lookup"><span data-stu-id="ef3c9-105">Represents information about positions related to entities within a user's [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ef3c9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef3c9-106">Properties</span></span>

| <span data-ttu-id="ef3c9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef3c9-107">Property</span></span>       | <span data-ttu-id="ef3c9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef3c9-108">Type</span></span>                             | <span data-ttu-id="ef3c9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef3c9-109">Description</span></span>                                            |
|:---------------|:---------------------------------|:-------------------------------------------------------|
|<span data-ttu-id="ef3c9-110">empresarial</span><span class="sxs-lookup"><span data-stu-id="ef3c9-110">company</span></span>         |[<span data-ttu-id="ef3c9-111">companyDetail</span><span class="sxs-lookup"><span data-stu-id="ef3c9-111">companyDetail</span></span>](companydetail.md) | <span data-ttu-id="ef3c9-112">Detalhes sobre a empresa ou o empregador.</span><span class="sxs-lookup"><span data-stu-id="ef3c9-112">Detail about the company or employer.</span></span>                  |
|<span data-ttu-id="ef3c9-113">description</span><span class="sxs-lookup"><span data-stu-id="ef3c9-113">description</span></span>     |<span data-ttu-id="ef3c9-114">String</span><span class="sxs-lookup"><span data-stu-id="ef3c9-114">String</span></span>                            | <span data-ttu-id="ef3c9-115">Descrição da posição em questão.</span><span class="sxs-lookup"><span data-stu-id="ef3c9-115">Description of the position in question.</span></span>               |
|<span data-ttu-id="ef3c9-116">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="ef3c9-116">endMonthYear</span></span>    |<span data-ttu-id="ef3c9-117">Data</span><span class="sxs-lookup"><span data-stu-id="ef3c9-117">Date</span></span>                              | <span data-ttu-id="ef3c9-118">Quando a posição terminou.</span><span class="sxs-lookup"><span data-stu-id="ef3c9-118">When the position ended.</span></span>                               |
|<span data-ttu-id="ef3c9-119">jobTitle</span><span class="sxs-lookup"><span data-stu-id="ef3c9-119">jobTitle</span></span>        |<span data-ttu-id="ef3c9-120">String</span><span class="sxs-lookup"><span data-stu-id="ef3c9-120">String</span></span>                            | <span data-ttu-id="ef3c9-121">O título mantido na posição.</span><span class="sxs-lookup"><span data-stu-id="ef3c9-121">The title held when in that position.</span></span>                  |
|<span data-ttu-id="ef3c9-122">role</span><span class="sxs-lookup"><span data-stu-id="ef3c9-122">role</span></span>            |<span data-ttu-id="ef3c9-123">String</span><span class="sxs-lookup"><span data-stu-id="ef3c9-123">String</span></span>                            | <span data-ttu-id="ef3c9-124">A função em que a posição é encaudada.</span><span class="sxs-lookup"><span data-stu-id="ef3c9-124">The role the position entailed.</span></span>                        |
|<span data-ttu-id="ef3c9-125">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="ef3c9-125">startMonthYear</span></span>  |<span data-ttu-id="ef3c9-126">Data</span><span class="sxs-lookup"><span data-stu-id="ef3c9-126">Date</span></span>                              | <span data-ttu-id="ef3c9-127">O mês e o ano de início da posição.</span><span class="sxs-lookup"><span data-stu-id="ef3c9-127">The start month and year of the position.</span></span>              |
|<span data-ttu-id="ef3c9-128">summary</span><span class="sxs-lookup"><span data-stu-id="ef3c9-128">summary</span></span>         |<span data-ttu-id="ef3c9-129">String</span><span class="sxs-lookup"><span data-stu-id="ef3c9-129">String</span></span>                            |<span data-ttu-id="ef3c9-130">Breve resumo da posição.</span><span class="sxs-lookup"><span data-stu-id="ef3c9-130">Short summary of the position.</span></span>                          |

## <a name="json-representation"></a><span data-ttu-id="ef3c9-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef3c9-131">JSON representation</span></span>

<span data-ttu-id="ef3c9-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef3c9-132">The following is a JSON representation of the resource.</span></span>

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