---
title: tipo de recurso companyDetail
description: tipo de recurso companyDetail
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 04e33c9fdae1eae811ee88e7cdef95b4b97b2c3f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936836"
---
# <a name="companydetail-resource-type"></a><span data-ttu-id="472a6-103">tipo de recurso companyDetail</span><span class="sxs-lookup"><span data-stu-id="472a6-103">companyDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="472a6-104">Representa informações sobre as empresas relacionadas às entidades em seu [perfil](profile.md).</span><span class="sxs-lookup"><span data-stu-id="472a6-104">Represents information about companies related to entities within their [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="472a6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="472a6-105">Properties</span></span>

| <span data-ttu-id="472a6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="472a6-106">Property</span></span>       | <span data-ttu-id="472a6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="472a6-107">Type</span></span>                                | <span data-ttu-id="472a6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="472a6-108">Description</span></span>                                 |
|:---------------|:------------------------------------|:--------------------------------------------|
|<span data-ttu-id="472a6-109">address</span><span class="sxs-lookup"><span data-stu-id="472a6-109">address</span></span>         |[<span data-ttu-id="472a6-110">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="472a6-110">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="472a6-111">Endereço da empresa.</span><span class="sxs-lookup"><span data-stu-id="472a6-111">Address of the company.</span></span>                     |
|<span data-ttu-id="472a6-112">department</span><span class="sxs-lookup"><span data-stu-id="472a6-112">department</span></span>      |<span data-ttu-id="472a6-113">String</span><span class="sxs-lookup"><span data-stu-id="472a6-113">String</span></span>                               | <span data-ttu-id="472a6-114">Nome do departamento dentro de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="472a6-114">Department Name within a company.</span></span>           |
|<span data-ttu-id="472a6-115">displayName</span><span class="sxs-lookup"><span data-stu-id="472a6-115">displayName</span></span>     |<span data-ttu-id="472a6-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="472a6-116">String</span></span>                               | <span data-ttu-id="472a6-117">Nome da empresa.</span><span class="sxs-lookup"><span data-stu-id="472a6-117">Company name.</span></span>                               |
|<span data-ttu-id="472a6-118">officeLocation</span><span class="sxs-lookup"><span data-stu-id="472a6-118">officeLocation</span></span>  |<span data-ttu-id="472a6-119">String</span><span class="sxs-lookup"><span data-stu-id="472a6-119">String</span></span>                               | <span data-ttu-id="472a6-120">Local do escritório da pessoa que se refere.</span><span class="sxs-lookup"><span data-stu-id="472a6-120">Office Location of the person referred to.</span></span>  |
|<span data-ttu-id="472a6-121">pronúncia</span><span class="sxs-lookup"><span data-stu-id="472a6-121">pronunciation</span></span>   |<span data-ttu-id="472a6-122">String</span><span class="sxs-lookup"><span data-stu-id="472a6-122">String</span></span>                               | <span data-ttu-id="472a6-123">Guia de pronúncia para o nome da empresa.</span><span class="sxs-lookup"><span data-stu-id="472a6-123">Pronunciation guide for the company name.</span></span>   |
|<span data-ttu-id="472a6-124">webUrl</span><span class="sxs-lookup"><span data-stu-id="472a6-124">webUrl</span></span>          |<span data-ttu-id="472a6-125">String</span><span class="sxs-lookup"><span data-stu-id="472a6-125">String</span></span>                               | <span data-ttu-id="472a6-126">Link para a Home Page da empresa.</span><span class="sxs-lookup"><span data-stu-id="472a6-126">Link to the company home page.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="472a6-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="472a6-127">JSON representation</span></span>

<span data-ttu-id="472a6-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="472a6-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.companyDetail",
  "baseType": null
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "department": "String",
  "displayName": "String",
  "officeLocation": "String",
  "pronunciation": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "companyDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->