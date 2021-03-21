---
title: Tipo de recurso employeeOrgData
description: Representa os dados da organização associados a um usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: cmmdesai
ms.openlocfilehash: 5e3ea0401730ffc8b15cae8c371d9352995c6f28
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961990"
---
# <a name="employeeorgdata-resource-type"></a><span data-ttu-id="a3287-103">Tipo de recurso employeeOrgData</span><span class="sxs-lookup"><span data-stu-id="a3287-103">employeeOrgData resource type</span></span>

<span data-ttu-id="a3287-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3287-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a3287-105">Representa os dados da organização associados a um usuário.</span><span class="sxs-lookup"><span data-stu-id="a3287-105">Represents organization data associated with a user.</span></span> <span data-ttu-id="a3287-106">A **propriedade employeeOrgData** da entidade [user](user.md) é uma coleção de atributos da organização.</span><span class="sxs-lookup"><span data-stu-id="a3287-106">The **employeeOrgData** property of the [user](user.md) entity is a collection of organization attributes.</span></span>

## <a name="properties"></a><span data-ttu-id="a3287-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3287-107">Properties</span></span>
| <span data-ttu-id="a3287-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3287-108">Property</span></span>       | <span data-ttu-id="a3287-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3287-109">Type</span></span>    |<span data-ttu-id="a3287-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3287-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a3287-111">division</span><span class="sxs-lookup"><span data-stu-id="a3287-111">division</span></span> | <span data-ttu-id="a3287-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3287-112">String</span></span> | <span data-ttu-id="a3287-113">O nome da divisão na qual o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="a3287-113">The name of the division in which the user works.</span></span> <br><br><span data-ttu-id="a3287-114">Retornado apenas em `$select`.</span><span class="sxs-lookup"><span data-stu-id="a3287-114">Returned only on `$select`.</span></span> <span data-ttu-id="a3287-115">Oferece suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="a3287-115">Supports `$filter`.</span></span> |
| <span data-ttu-id="a3287-116">costCenter</span><span class="sxs-lookup"><span data-stu-id="a3287-116">costCenter</span></span> | <span data-ttu-id="a3287-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3287-117">String</span></span> | <span data-ttu-id="a3287-118">O centro de custos associado ao usuário.</span><span class="sxs-lookup"><span data-stu-id="a3287-118">The cost center associated with the user.</span></span> <br><br><span data-ttu-id="a3287-119">Retornado apenas em `$select`.</span><span class="sxs-lookup"><span data-stu-id="a3287-119">Returned only on `$select`.</span></span> <span data-ttu-id="a3287-120">Oferece suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="a3287-120">Supports `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a3287-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3287-121">JSON representation</span></span>

<span data-ttu-id="a3287-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3287-122">The following is a JSON representation of the resource.</span></span>

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
