---
title: tipo de recurso educationIdentityDomain
description: 'Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence. O recurso de domínio faz parte da configuração de criação de identidade. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 86e65d46c8037ebcbb2c98f9f9e93f94f34bbdef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972702"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="9d8a3-104">tipo de recurso educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="9d8a3-104">educationIdentityDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d8a3-105">Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-105">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="9d8a3-106">O recurso de domínio faz parte da [configuração de criação de identidade](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9d8a3-106">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="9d8a3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d8a3-107">Properties</span></span>

| <span data-ttu-id="9d8a3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d8a3-108">Property</span></span> | <span data-ttu-id="9d8a3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d8a3-109">Type</span></span> | <span data-ttu-id="9d8a3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d8a3-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="9d8a3-111">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="9d8a3-111">**appliesTo**</span></span> | <span data-ttu-id="9d8a3-112">string</span><span class="sxs-lookup"><span data-stu-id="9d8a3-112">string</span></span> |  <span data-ttu-id="9d8a3-113">O tipo de função de usuário a ser atribuído à licença.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-113">The user role type to assign to the license.</span></span> <span data-ttu-id="9d8a3-114">Os valores possíveis são: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-114">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="9d8a3-115">**name**</span><span class="sxs-lookup"><span data-stu-id="9d8a3-115">**name**</span></span> | <span data-ttu-id="9d8a3-116">string</span><span class="sxs-lookup"><span data-stu-id="9d8a3-116">string</span></span> |  <span data-ttu-id="9d8a3-117">Representa o domínio da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-117">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="9d8a3-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d8a3-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "name": "String"
}
```
