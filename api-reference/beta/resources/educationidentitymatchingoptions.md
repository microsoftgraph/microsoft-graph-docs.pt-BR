---
title: tipo de recurso educationIdentityMatchingOptions
description: Fornece um mapeamento entre uma propriedade de origem e uma propriedade de destino para as contas de usuário correspondentes. A propriedade Source deve existir nos dados de origem. A propriedade target deve ser uma propriedade válida no Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d722beaac54cbd57c227457a0883b856f6eca4bc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501826"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="7f3fd-105">tipo de recurso educationIdentityMatchingOptions</span><span class="sxs-lookup"><span data-stu-id="7f3fd-105">educationIdentityMatchingOptions resource type</span></span>

<span data-ttu-id="7f3fd-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7f3fd-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f3fd-107">Fornece um mapeamento entre uma propriedade de origem e uma propriedade de destino para as contas de usuário correspondentes.</span><span class="sxs-lookup"><span data-stu-id="7f3fd-107">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="7f3fd-108">A propriedade Source deve existir nos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="7f3fd-108">The source property should exist in the source data.</span></span> <span data-ttu-id="7f3fd-109">A propriedade target deve ser uma propriedade válida no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="7f3fd-109">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="7f3fd-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f3fd-110">Properties</span></span>

| <span data-ttu-id="7f3fd-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f3fd-111">Property</span></span> | <span data-ttu-id="7f3fd-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f3fd-112">Type</span></span> | <span data-ttu-id="7f3fd-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f3fd-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="7f3fd-114">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="7f3fd-114">**appliesTo**</span></span> | <span data-ttu-id="7f3fd-115">string</span><span class="sxs-lookup"><span data-stu-id="7f3fd-115">string</span></span> |  <span data-ttu-id="7f3fd-116">O tipo de função de usuário a ser atribuído à licença.</span><span class="sxs-lookup"><span data-stu-id="7f3fd-116">The user role type to assign to the license.</span></span> <span data-ttu-id="7f3fd-117">Os valores possíveis são: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="7f3fd-117">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="7f3fd-118">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="7f3fd-118">**sourcePropertyName**</span></span> | <span data-ttu-id="7f3fd-119">string</span><span class="sxs-lookup"><span data-stu-id="7f3fd-119">string</span></span> |  <span data-ttu-id="7f3fd-120">O nome da propriedade Source, que deve ser um nome de campo nos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="7f3fd-120">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="7f3fd-121">Essa propriedade diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7f3fd-121">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="7f3fd-122">**TargetName**</span><span class="sxs-lookup"><span data-stu-id="7f3fd-122">**targetPropertyName**</span></span> | <span data-ttu-id="7f3fd-123">string</span><span class="sxs-lookup"><span data-stu-id="7f3fd-123">string</span></span> |  <span data-ttu-id="7f3fd-124">O nome da propriedade de destino, que deve ser uma propriedade válida no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7f3fd-124">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="7f3fd-125">Essa propriedade diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7f3fd-125">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="7f3fd-126">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="7f3fd-126">**targetDomain**</span></span> | <span data-ttu-id="7f3fd-127">string</span><span class="sxs-lookup"><span data-stu-id="7f3fd-127">string</span></span> |  <span data-ttu-id="7f3fd-128">O domínio a ser sufixo com a propriedade Source para corresponder ao destino.</span><span class="sxs-lookup"><span data-stu-id="7f3fd-128">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="7f3fd-129">Se fornecido como nulo, a propriedade Source será usada para corresponder à Propriedade Target.</span><span class="sxs-lookup"><span data-stu-id="7f3fd-129">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="7f3fd-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f3fd-130">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
