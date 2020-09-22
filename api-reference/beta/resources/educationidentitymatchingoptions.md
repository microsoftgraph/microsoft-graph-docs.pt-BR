---
title: tipo de recurso educationIdentityMatchingOptions
description: Fornece um mapeamento entre uma propriedade de origem e uma propriedade de destino para as contas de usuário correspondentes. A propriedade Source deve existir nos dados de origem. A propriedade target deve ser uma propriedade válida no Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 73c97b0e9c23c455b3e15ed656060eca7f8a3e4e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095370"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="4adc3-105">tipo de recurso educationIdentityMatchingOptions</span><span class="sxs-lookup"><span data-stu-id="4adc3-105">educationIdentityMatchingOptions resource type</span></span>

<span data-ttu-id="4adc3-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4adc3-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4adc3-107">Fornece um mapeamento entre uma propriedade de origem e uma propriedade de destino para as contas de usuário correspondentes.</span><span class="sxs-lookup"><span data-stu-id="4adc3-107">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="4adc3-108">A propriedade Source deve existir nos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="4adc3-108">The source property should exist in the source data.</span></span> <span data-ttu-id="4adc3-109">A propriedade target deve ser uma propriedade válida no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="4adc3-109">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="4adc3-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4adc3-110">Properties</span></span>

| <span data-ttu-id="4adc3-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4adc3-111">Property</span></span>           | <span data-ttu-id="4adc3-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="4adc3-112">Type</span></span>   | <span data-ttu-id="4adc3-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="4adc3-113">Description</span></span>                                                                                                                                                    |
| :----------------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="4adc3-114">appliesTo</span><span class="sxs-lookup"><span data-stu-id="4adc3-114">appliesTo</span></span>          | <span data-ttu-id="4adc3-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4adc3-115">String</span></span> | <span data-ttu-id="4adc3-116">O tipo de função de usuário a ser atribuído à licença.</span><span class="sxs-lookup"><span data-stu-id="4adc3-116">The user role type to assign to the license.</span></span> <span data-ttu-id="4adc3-117">Os valores possíveis são: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="4adc3-117">Possible values are: `student`, `teacher`, `faculty`.</span></span>                                                             |
| <span data-ttu-id="4adc3-118">sourcePropertyName</span><span class="sxs-lookup"><span data-stu-id="4adc3-118">sourcePropertyName</span></span> | <span data-ttu-id="4adc3-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4adc3-119">String</span></span> | <span data-ttu-id="4adc3-120">O nome da propriedade Source, que deve ser um nome de campo nos dados de origem.</span><span class="sxs-lookup"><span data-stu-id="4adc3-120">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="4adc3-121">Essa propriedade diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="4adc3-121">This property is case-sensitive.</span></span>                                             |
| <span data-ttu-id="4adc3-122">TargetName</span><span class="sxs-lookup"><span data-stu-id="4adc3-122">targetPropertyName</span></span> | <span data-ttu-id="4adc3-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4adc3-123">String</span></span> | <span data-ttu-id="4adc3-124">O nome da propriedade de destino, que deve ser uma propriedade válida no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4adc3-124">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="4adc3-125">Essa propriedade diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="4adc3-125">This property is case-sensitive.</span></span>                                                |
| <span data-ttu-id="4adc3-126">targetDomain</span><span class="sxs-lookup"><span data-stu-id="4adc3-126">targetDomain</span></span>       | <span data-ttu-id="4adc3-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4adc3-127">String</span></span> | <span data-ttu-id="4adc3-128">O domínio a ser sufixo com a propriedade Source para corresponder ao destino.</span><span class="sxs-lookup"><span data-stu-id="4adc3-128">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="4adc3-129">Se fornecido como nulo, a propriedade Source será usada para corresponder à Propriedade Target.</span><span class="sxs-lookup"><span data-stu-id="4adc3-129">If provided as null, the source property will be used to match with the target property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4adc3-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4adc3-130">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "sourcePropertyName": "String",
  "targetPropertyName": "String",
  "targetDomain": "String"
}
```


