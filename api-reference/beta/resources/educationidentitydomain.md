---
title: tipo de recurso de educationIdentityDomain
description: 'Representa o mapeamento entre um tipo de usuário de educação e o domínio em que a conta do usuário pertence. O recurso de domínio é parte da configuração de criação de identidade. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0c6004d18897b8f8284c06a3b09830072148df87
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528176"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="8eeb5-104">tipo de recurso de educationIdentityDomain</span><span class="sxs-lookup"><span data-stu-id="8eeb5-104">educationIdentityDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8eeb5-105">Representa o mapeamento entre um tipo de usuário de educação e o domínio em que a conta do usuário pertence.</span><span class="sxs-lookup"><span data-stu-id="8eeb5-105">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="8eeb5-106">O recurso de domínio é parte da [configuração de criação de identidade](educationidentitycreationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eeb5-106">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="8eeb5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8eeb5-107">Properties</span></span>

| <span data-ttu-id="8eeb5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8eeb5-108">Property</span></span> | <span data-ttu-id="8eeb5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8eeb5-109">Type</span></span> | <span data-ttu-id="8eeb5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8eeb5-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8eeb5-111">appliesTo</span><span class="sxs-lookup"><span data-stu-id="8eeb5-111">**appliesTo**</span></span> | <span data-ttu-id="8eeb5-112">string</span><span class="sxs-lookup"><span data-stu-id="8eeb5-112">string</span></span> |  <span data-ttu-id="8eeb5-113">O tipo de função de usuário para atribuir a licença.</span><span class="sxs-lookup"><span data-stu-id="8eeb5-113">The user role type to assign to license.</span></span> <span data-ttu-id="8eeb5-114">Os valores possíveis são: `student` e `teacher`.</span><span class="sxs-lookup"><span data-stu-id="8eeb5-114">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="8eeb5-115">**name**</span><span class="sxs-lookup"><span data-stu-id="8eeb5-115">**name**</span></span> | <span data-ttu-id="8eeb5-116">string</span><span class="sxs-lookup"><span data-stu-id="8eeb5-116">string</span></span> |  <span data-ttu-id="8eeb5-117">Representa o domínio da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="8eeb5-117">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="8eeb5-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8eeb5-118">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitydomain.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
