---
title: tipo de recurso educationIdentityDomain
description: 'Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence. O recurso de domínio faz parte da configuração de criação de identidade. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5cf7444c51b34ae4a8eacf9c99fdfd085dbec896
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334252"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="8e066-104">tipo de recurso educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="8e066-104">educationIdentityDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e066-105">Representa o mapeamento entre um tipo de usuário educacional e o domínio ao qual a conta do usuário pertence.</span><span class="sxs-lookup"><span data-stu-id="8e066-105">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="8e066-106">O recurso de domínio faz parte da [configuração de criação de identidade](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e066-106">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="8e066-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e066-107">Properties</span></span>

| <span data-ttu-id="8e066-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e066-108">Property</span></span> | <span data-ttu-id="8e066-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e066-109">Type</span></span> | <span data-ttu-id="8e066-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e066-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8e066-111">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="8e066-111">**appliesTo**</span></span> | <span data-ttu-id="8e066-112">string</span><span class="sxs-lookup"><span data-stu-id="8e066-112">string</span></span> |  <span data-ttu-id="8e066-113">O tipo de função de usuário a ser atribuído à licença.</span><span class="sxs-lookup"><span data-stu-id="8e066-113">The user role type to assign to license.</span></span> <span data-ttu-id="8e066-114">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="8e066-114">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="8e066-115">**name**</span><span class="sxs-lookup"><span data-stu-id="8e066-115">**name**</span></span> | <span data-ttu-id="8e066-116">string</span><span class="sxs-lookup"><span data-stu-id="8e066-116">string</span></span> |  <span data-ttu-id="8e066-117">Representa o domínio da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="8e066-117">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="8e066-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e066-118">JSON representation</span></span>
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
