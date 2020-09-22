---
title: tipo de recurso educationIdentityDomain
description: 'Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence. O recurso de domínio faz parte da configuração de criação de identidade. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b25f935ae404a243826a14c310a17ad80c598380
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095384"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="7d7f9-104">tipo de recurso educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="7d7f9-104">educationIdentityDomain resource type</span></span>

<span data-ttu-id="7d7f9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d7f9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d7f9-106">Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence.</span><span class="sxs-lookup"><span data-stu-id="7d7f9-106">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="7d7f9-107">O recurso de domínio faz parte da [configuração de criação de identidade](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d7f9-107">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7d7f9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d7f9-108">Properties</span></span>

| <span data-ttu-id="7d7f9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d7f9-109">Property</span></span>  | <span data-ttu-id="7d7f9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d7f9-110">Type</span></span>   | <span data-ttu-id="7d7f9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d7f9-111">Description</span></span>                                                                                        |
| :-------- | :----- | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7d7f9-112">appliesTo</span><span class="sxs-lookup"><span data-stu-id="7d7f9-112">appliesTo</span></span> | <span data-ttu-id="7d7f9-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7f9-113">String</span></span> | <span data-ttu-id="7d7f9-114">O tipo de função de usuário a ser atribuído à licença.</span><span class="sxs-lookup"><span data-stu-id="7d7f9-114">The user role type to assign to the license.</span></span> <span data-ttu-id="7d7f9-115">Os valores possíveis são: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="7d7f9-115">Possible values are: `student`, `teacher`, `faculty`.</span></span> |
| <span data-ttu-id="7d7f9-116">name</span><span class="sxs-lookup"><span data-stu-id="7d7f9-116">name</span></span>      | <span data-ttu-id="7d7f9-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7f9-117">String</span></span> | <span data-ttu-id="7d7f9-118">Representa o domínio da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="7d7f9-118">Represents the domain for the user account.</span></span>                                                        |

## <a name="json-representation"></a><span data-ttu-id="7d7f9-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d7f9-119">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "name": "String"
}
```


