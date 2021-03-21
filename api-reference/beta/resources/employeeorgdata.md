---
title: Tipo de recurso employeeOrgData
description: Representa os dados da organização associados a um usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: cmmdesai
ms.openlocfilehash: 841422920ccfe625bd03d8167c13f2a1eba83088
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960429"
---
# <a name="employeeorgdata-resource-type"></a><span data-ttu-id="a2a74-103">Tipo de recurso employeeOrgData</span><span class="sxs-lookup"><span data-stu-id="a2a74-103">employeeOrgData resource type</span></span>

<span data-ttu-id="a2a74-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2a74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2a74-105">Representa os dados da organização associados a um usuário.</span><span class="sxs-lookup"><span data-stu-id="a2a74-105">Represents organization data associated with a user.</span></span> <span data-ttu-id="a2a74-106">A **propriedade employeeOrgData** da entidade [user](user.md) é uma coleção de atributos da organização.</span><span class="sxs-lookup"><span data-stu-id="a2a74-106">The **employeeOrgData** property of the [user](user.md) entity is a collection of organization attributes.</span></span>

## <a name="properties"></a><span data-ttu-id="a2a74-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2a74-107">Properties</span></span>
| <span data-ttu-id="a2a74-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2a74-108">Property</span></span>       | <span data-ttu-id="a2a74-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2a74-109">Type</span></span>    |<span data-ttu-id="a2a74-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2a74-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a2a74-111">division</span><span class="sxs-lookup"><span data-stu-id="a2a74-111">division</span></span> | <span data-ttu-id="a2a74-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2a74-112">String</span></span> | <span data-ttu-id="a2a74-113">O nome da divisão na qual o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="a2a74-113">The name of the division in which the user works.</span></span> <br><br><span data-ttu-id="a2a74-114">Retornado apenas em `$select`.</span><span class="sxs-lookup"><span data-stu-id="a2a74-114">Returned only on `$select`.</span></span> <span data-ttu-id="a2a74-115">Oferece suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="a2a74-115">Supports `$filter`.</span></span> |
| <span data-ttu-id="a2a74-116">costCenter</span><span class="sxs-lookup"><span data-stu-id="a2a74-116">costCenter</span></span> | <span data-ttu-id="a2a74-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2a74-117">String</span></span> | <span data-ttu-id="a2a74-118">O centro de custos associado ao usuário.</span><span class="sxs-lookup"><span data-stu-id="a2a74-118">The cost center associated with the user.</span></span> <br><br><span data-ttu-id="a2a74-119">Retornado apenas em `$select`.</span><span class="sxs-lookup"><span data-stu-id="a2a74-119">Returned only on `$select`.</span></span> <span data-ttu-id="a2a74-120">Oferece suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="a2a74-120">Supports `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a2a74-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2a74-121">JSON representation</span></span>

<span data-ttu-id="a2a74-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2a74-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.employeeOrgData"
}-->

```json
{
  "costCenter": "string",
  "division": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-10-24 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "employeeOrgData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
