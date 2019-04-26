---
title: tipo de recurso educationIdentityMatchingOptions
description: Fornece um mapeamento entre uma propriedade de origem e uma propriedade de destino para as contas de usuário correspondentes. A propriedade Source deve existir nos dados de origem. A propriedade target deve ser uma propriedade válida no Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7ce68460e8dfd0ff3e58b51d0007278aa6c9426e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334237"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="202a9-105">tipo de recurso educationIdentityMatchingOptions</span><span class="sxs-lookup"><span data-stu-id="202a9-105">educationIdentityMatchingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="202a9-106">Fornece um mapeamento entre uma propriedade de origem e uma propriedade de destino para as contas de usuário correspondentes.</span><span class="sxs-lookup"><span data-stu-id="202a9-106">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="202a9-107">A propriedade Source deve existir nos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="202a9-107">The source property should exist in the source data.</span></span> <span data-ttu-id="202a9-108">A propriedade target deve ser uma propriedade válida no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="202a9-108">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="202a9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="202a9-109">Properties</span></span>

| <span data-ttu-id="202a9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="202a9-110">Property</span></span> | <span data-ttu-id="202a9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="202a9-111">Type</span></span> | <span data-ttu-id="202a9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="202a9-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="202a9-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="202a9-113">**appliesTo**</span></span> | <span data-ttu-id="202a9-114">string</span><span class="sxs-lookup"><span data-stu-id="202a9-114">string</span></span> |  <span data-ttu-id="202a9-115">O tipo de função de usuário a ser atribuído à licença.</span><span class="sxs-lookup"><span data-stu-id="202a9-115">The user role type to assign to the license.</span></span> <span data-ttu-id="202a9-116">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="202a9-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="202a9-117">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="202a9-117">**sourcePropertyName**</span></span> | <span data-ttu-id="202a9-118">string</span><span class="sxs-lookup"><span data-stu-id="202a9-118">string</span></span> |  <span data-ttu-id="202a9-119">O nome da propriedade Source, que deve ser um nome de campo nos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="202a9-119">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="202a9-120">Essa propriedade diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="202a9-120">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="202a9-121">**TargetName**</span><span class="sxs-lookup"><span data-stu-id="202a9-121">**targetPropertyName**</span></span> | <span data-ttu-id="202a9-122">string</span><span class="sxs-lookup"><span data-stu-id="202a9-122">string</span></span> |  <span data-ttu-id="202a9-123">O nome da propriedade de destino, que deve ser uma propriedade válida no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="202a9-123">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="202a9-124">Essa propriedade diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="202a9-124">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="202a9-125">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="202a9-125">**targetDomain**</span></span> | <span data-ttu-id="202a9-126">string</span><span class="sxs-lookup"><span data-stu-id="202a9-126">string</span></span> |  <span data-ttu-id="202a9-127">O domínio a ser sufixo com a propriedade Source para corresponder ao destino.</span><span class="sxs-lookup"><span data-stu-id="202a9-127">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="202a9-128">Se fornecido como nulo, a propriedade Source será usada para corresponder à Propriedade Target.</span><span class="sxs-lookup"><span data-stu-id="202a9-128">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="202a9-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="202a9-129">JSON representation</span></span>
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
