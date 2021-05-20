---
title: Tipo de recurso assignedLicense
description: Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade user é uma coleção de **assignedLicense**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 9d957f2bfa5c7c9e4390e5c4df06d084a3e49e6f
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547246"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="10b72-104">Tipo de recurso assignedLicense</span><span class="sxs-lookup"><span data-stu-id="10b72-104">assignedLicense resource type</span></span>

<span data-ttu-id="10b72-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10b72-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10b72-p102">Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade [user](user.md) é uma coleção de **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="10b72-p102">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="10b72-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10b72-108">Properties</span></span>
| <span data-ttu-id="10b72-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10b72-109">Property</span></span>     | <span data-ttu-id="10b72-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="10b72-110">Type</span></span>   |<span data-ttu-id="10b72-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="10b72-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10b72-112">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="10b72-112">disabledPlans</span></span>|<span data-ttu-id="10b72-113">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="10b72-113">Guid collection</span></span>|<span data-ttu-id="10b72-114">Uma coleção dos identificadores exclusivos de planos que foram desabilitados.</span><span class="sxs-lookup"><span data-stu-id="10b72-114">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="10b72-115">skuId</span><span class="sxs-lookup"><span data-stu-id="10b72-115">skuId</span></span>|<span data-ttu-id="10b72-116">Guid</span><span class="sxs-lookup"><span data-stu-id="10b72-116">Guid</span></span>|<span data-ttu-id="10b72-117">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="10b72-117">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10b72-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10b72-118">JSON representation</span></span>

<span data-ttu-id="10b72-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="10b72-119">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


