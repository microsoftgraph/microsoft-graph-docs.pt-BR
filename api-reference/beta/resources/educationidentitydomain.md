---
title: tipo de recurso educationIdentityDomain
description: 'Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence. O recurso de domínio faz parte da configuração de criação de identidade. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5f4e23a9111d2515234d1aa665f4847d732dc563
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435037"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="f4aa1-104">tipo de recurso educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="f4aa1-104">educationIdentityDomain resource type</span></span>

<span data-ttu-id="f4aa1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4aa1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4aa1-106">Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence.</span><span class="sxs-lookup"><span data-stu-id="f4aa1-106">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="f4aa1-107">O recurso de domínio faz parte da [configuração de criação de identidade](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4aa1-107">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f4aa1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4aa1-108">Properties</span></span>

| <span data-ttu-id="f4aa1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4aa1-109">Property</span></span>  | <span data-ttu-id="f4aa1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4aa1-110">Type</span></span>   | <span data-ttu-id="f4aa1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4aa1-111">Description</span></span>                                                                                        |
| :-------- | :----- | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f4aa1-112">appliesTo</span><span class="sxs-lookup"><span data-stu-id="f4aa1-112">appliesTo</span></span> | <span data-ttu-id="f4aa1-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4aa1-113">String</span></span> | <span data-ttu-id="f4aa1-114">O tipo de função de usuário a ser atribuído à licença.</span><span class="sxs-lookup"><span data-stu-id="f4aa1-114">The user role type to assign to the license.</span></span> <span data-ttu-id="f4aa1-115">Os valores possíveis são: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="f4aa1-115">Possible values are: `student`, `teacher`, `faculty`.</span></span> |
| <span data-ttu-id="f4aa1-116">nome</span><span class="sxs-lookup"><span data-stu-id="f4aa1-116">name</span></span>      | <span data-ttu-id="f4aa1-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4aa1-117">String</span></span> | <span data-ttu-id="f4aa1-118">Representa o domínio da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="f4aa1-118">Represents the domain for the user account.</span></span>                                                        |

## <a name="json-representation"></a><span data-ttu-id="f4aa1-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4aa1-119">JSON representation</span></span>

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
