---
title: tipo de recurso employeeOrgData
description: Representa os dados da organização associados a um usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: cmmdesai
ms.openlocfilehash: 841d3c7965309721d662475f2cba553c378c49ee
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635604"
---
# <a name="employeeorgdata-resource-type"></a><span data-ttu-id="7fde2-103">tipo de recurso employeeOrgData</span><span class="sxs-lookup"><span data-stu-id="7fde2-103">employeeOrgData resource type</span></span>

<span data-ttu-id="7fde2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fde2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7fde2-105">Representa os dados da organização associados a um usuário.</span><span class="sxs-lookup"><span data-stu-id="7fde2-105">Represents organization data associated with a user.</span></span> <span data-ttu-id="7fde2-106">A propriedade **employeeOrgData** da entidade [User](user.md) é uma coleção de atributos de organização.</span><span class="sxs-lookup"><span data-stu-id="7fde2-106">The **employeeOrgData** property of the [user](user.md) entity is a collection of organization attributes.</span></span>

## <a name="properties"></a><span data-ttu-id="7fde2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7fde2-107">Properties</span></span>
| <span data-ttu-id="7fde2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7fde2-108">Property</span></span>       | <span data-ttu-id="7fde2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fde2-109">Type</span></span>    |<span data-ttu-id="7fde2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fde2-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7fde2-111">Division</span><span class="sxs-lookup"><span data-stu-id="7fde2-111">division</span></span> | <span data-ttu-id="7fde2-112">String</span><span class="sxs-lookup"><span data-stu-id="7fde2-112">String</span></span> | <span data-ttu-id="7fde2-113">O nome da divisão na qual o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="7fde2-113">The name of the division in which the user works.</span></span> <br><br><span data-ttu-id="7fde2-114">Retornado apenas em `$select`.</span><span class="sxs-lookup"><span data-stu-id="7fde2-114">Returned only on `$select`.</span></span> <span data-ttu-id="7fde2-115">Oferece suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7fde2-115">Supports `$filter`.</span></span> |
| <span data-ttu-id="7fde2-116">costCenter</span><span class="sxs-lookup"><span data-stu-id="7fde2-116">costCenter</span></span> | <span data-ttu-id="7fde2-117">String</span><span class="sxs-lookup"><span data-stu-id="7fde2-117">String</span></span> | <span data-ttu-id="7fde2-118">O centro de custos associado ao usuário.</span><span class="sxs-lookup"><span data-stu-id="7fde2-118">The cost center associated with the user.</span></span> <br><br><span data-ttu-id="7fde2-119">Retornado apenas em `$select`.</span><span class="sxs-lookup"><span data-stu-id="7fde2-119">Returned only on `$select`.</span></span> <span data-ttu-id="7fde2-120">Oferece suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7fde2-120">Supports `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7fde2-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7fde2-121">JSON representation</span></span>

<span data-ttu-id="7fde2-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7fde2-122">The following is a JSON representation of the resource.</span></span>

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
