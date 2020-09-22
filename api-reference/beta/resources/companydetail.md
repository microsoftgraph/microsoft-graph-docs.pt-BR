---
title: tipo de recurso companyDetail
description: tipo de recurso companyDetail
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 93b5490048c149ca526a9c3d0024175c1c20d7e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033927"
---
# <a name="companydetail-resource-type"></a><span data-ttu-id="f0a4e-103">tipo de recurso companyDetail</span><span class="sxs-lookup"><span data-stu-id="f0a4e-103">companyDetail resource type</span></span>

<span data-ttu-id="f0a4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0a4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0a4e-105">Representa informações sobre as empresas relacionadas às entidades em seu [perfil](profile.md).</span><span class="sxs-lookup"><span data-stu-id="f0a4e-105">Represents information about companies related to entities within their [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f0a4e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0a4e-106">Properties</span></span>

| <span data-ttu-id="f0a4e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0a4e-107">Property</span></span>       | <span data-ttu-id="f0a4e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0a4e-108">Type</span></span>                                | <span data-ttu-id="f0a4e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0a4e-109">Description</span></span>                                 |
|:---------------|:------------------------------------|:--------------------------------------------|
|<span data-ttu-id="f0a4e-110">address</span><span class="sxs-lookup"><span data-stu-id="f0a4e-110">address</span></span>         |[<span data-ttu-id="f0a4e-111">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="f0a4e-111">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="f0a4e-112">Endereço da empresa.</span><span class="sxs-lookup"><span data-stu-id="f0a4e-112">Address of the company.</span></span>                     |
|<span data-ttu-id="f0a4e-113">department</span><span class="sxs-lookup"><span data-stu-id="f0a4e-113">department</span></span>      |<span data-ttu-id="f0a4e-114">String</span><span class="sxs-lookup"><span data-stu-id="f0a4e-114">String</span></span>                               | <span data-ttu-id="f0a4e-115">Nome do departamento dentro de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="f0a4e-115">Department Name within a company.</span></span>           |
|<span data-ttu-id="f0a4e-116">displayName</span><span class="sxs-lookup"><span data-stu-id="f0a4e-116">displayName</span></span>     |<span data-ttu-id="f0a4e-117">String</span><span class="sxs-lookup"><span data-stu-id="f0a4e-117">String</span></span>                               | <span data-ttu-id="f0a4e-118">Nome da empresa.</span><span class="sxs-lookup"><span data-stu-id="f0a4e-118">Company name.</span></span>                               |
|<span data-ttu-id="f0a4e-119">officeLocation</span><span class="sxs-lookup"><span data-stu-id="f0a4e-119">officeLocation</span></span>  |<span data-ttu-id="f0a4e-120">String</span><span class="sxs-lookup"><span data-stu-id="f0a4e-120">String</span></span>                               | <span data-ttu-id="f0a4e-121">Local do escritório da pessoa que se refere.</span><span class="sxs-lookup"><span data-stu-id="f0a4e-121">Office Location of the person referred to.</span></span>  |
|<span data-ttu-id="f0a4e-122">pronúncia</span><span class="sxs-lookup"><span data-stu-id="f0a4e-122">pronunciation</span></span>   |<span data-ttu-id="f0a4e-123">String</span><span class="sxs-lookup"><span data-stu-id="f0a4e-123">String</span></span>                               | <span data-ttu-id="f0a4e-124">Guia de pronúncia para o nome da empresa.</span><span class="sxs-lookup"><span data-stu-id="f0a4e-124">Pronunciation guide for the company name.</span></span>   |
|<span data-ttu-id="f0a4e-125">webUrl</span><span class="sxs-lookup"><span data-stu-id="f0a4e-125">webUrl</span></span>          |<span data-ttu-id="f0a4e-126">String</span><span class="sxs-lookup"><span data-stu-id="f0a4e-126">String</span></span>                               | <span data-ttu-id="f0a4e-127">Link para a Home Page da empresa.</span><span class="sxs-lookup"><span data-stu-id="f0a4e-127">Link to the company home page.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="f0a4e-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0a4e-128">JSON representation</span></span>

<span data-ttu-id="f0a4e-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0a4e-129">The following is a JSON representation of the resource.</span></span>

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

