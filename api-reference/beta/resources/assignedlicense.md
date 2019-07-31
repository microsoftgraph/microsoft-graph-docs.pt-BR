---
title: Tipo de recurso assignedLicense
description: Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade user é uma coleção de **assignedLicense**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8e23ed2430dcf20b49e8c792311f91507d3192ce
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974308"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="40b62-104">Tipo de recurso assignedLicense</span><span class="sxs-lookup"><span data-stu-id="40b62-104">assignedLicense resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40b62-105">Representa uma licença atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="40b62-105">Represents a license assigned to a user.</span></span> <span data-ttu-id="40b62-106">A propriedade **assignedLicenses** da entidade [user](user.md) é uma coleção de **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="40b62-106">The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="40b62-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40b62-107">Properties</span></span>
| <span data-ttu-id="40b62-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40b62-108">Property</span></span>     | <span data-ttu-id="40b62-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="40b62-109">Type</span></span>   |<span data-ttu-id="40b62-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="40b62-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40b62-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="40b62-111">disabledPlans</span></span>|<span data-ttu-id="40b62-112">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="40b62-112">Guid collection</span></span>|<span data-ttu-id="40b62-113">Uma coleção dos identificadores exclusivos de planos que foram desabilitados.</span><span class="sxs-lookup"><span data-stu-id="40b62-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="40b62-114">skuId</span><span class="sxs-lookup"><span data-stu-id="40b62-114">skuId</span></span>|<span data-ttu-id="40b62-115">Guid</span><span class="sxs-lookup"><span data-stu-id="40b62-115">Guid</span></span>|<span data-ttu-id="40b62-116">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="40b62-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40b62-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40b62-117">JSON representation</span></span>

<span data-ttu-id="40b62-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="40b62-118">Here is a JSON representation of the resource</span></span>

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
