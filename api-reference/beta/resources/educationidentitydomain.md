---
title: tipo de recurso educationIdentityDomain
description: 'Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence. O recurso de domínio faz parte da configuração de criação de identidade. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a21d4d3005be8a776ae8bb9f9e3c1027be48de72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501924"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="c3e59-104">tipo de recurso educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="c3e59-104">educationIdentityDomain resource type</span></span>

<span data-ttu-id="c3e59-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c3e59-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3e59-106">Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence.</span><span class="sxs-lookup"><span data-stu-id="c3e59-106">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="c3e59-107">O recurso de domínio faz parte da [configuração de criação de identidade](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3e59-107">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="c3e59-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3e59-108">Properties</span></span>

| <span data-ttu-id="c3e59-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3e59-109">Property</span></span> | <span data-ttu-id="c3e59-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3e59-110">Type</span></span> | <span data-ttu-id="c3e59-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3e59-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c3e59-112">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="c3e59-112">**appliesTo**</span></span> | <span data-ttu-id="c3e59-113">string</span><span class="sxs-lookup"><span data-stu-id="c3e59-113">string</span></span> |  <span data-ttu-id="c3e59-114">O tipo de função de usuário a ser atribuído à licença.</span><span class="sxs-lookup"><span data-stu-id="c3e59-114">The user role type to assign to the license.</span></span> <span data-ttu-id="c3e59-115">Os valores possíveis são: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="c3e59-115">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="c3e59-116">**name**</span><span class="sxs-lookup"><span data-stu-id="c3e59-116">**name**</span></span> | <span data-ttu-id="c3e59-117">string</span><span class="sxs-lookup"><span data-stu-id="c3e59-117">string</span></span> |  <span data-ttu-id="c3e59-118">Representa o domínio da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="c3e59-118">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="c3e59-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3e59-119">JSON representation</span></span>
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
