---
title: Tipo de recurso assignedLicense
description: Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade user é uma coleção de **assignedLicense**.
localization_priority: Normal
ms.openlocfilehash: 2d9620ec33a296c09ced9bc9d8af8d6d032bb7d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535652"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="e8e73-104">Tipo de recurso assignedLicense</span><span class="sxs-lookup"><span data-stu-id="e8e73-104">assignedLicense resource type</span></span>

<span data-ttu-id="e8e73-105">Representa uma licença atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="e8e73-105">Represents a license assigned to a user.</span></span> <span data-ttu-id="e8e73-106">A propriedade **assignedLicenses** da entidade [user](user.md) é uma coleção de **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="e8e73-106">The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="e8e73-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8e73-107">Properties</span></span>
| <span data-ttu-id="e8e73-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8e73-108">Property</span></span>     | <span data-ttu-id="e8e73-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8e73-109">Type</span></span>   |<span data-ttu-id="e8e73-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8e73-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8e73-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="e8e73-111">disabledPlans</span></span>|<span data-ttu-id="e8e73-112">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="e8e73-112">Guid collection</span></span>|<span data-ttu-id="e8e73-113">Uma coleção dos identificadores exclusivos de planos que foram desabilitados.</span><span class="sxs-lookup"><span data-stu-id="e8e73-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="e8e73-114">skuId</span><span class="sxs-lookup"><span data-stu-id="e8e73-114">skuId</span></span>|<span data-ttu-id="e8e73-115">Guid</span><span class="sxs-lookup"><span data-stu-id="e8e73-115">Guid</span></span>|<span data-ttu-id="e8e73-116">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="e8e73-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8e73-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8e73-117">JSON representation</span></span>

<span data-ttu-id="e8e73-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e8e73-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
