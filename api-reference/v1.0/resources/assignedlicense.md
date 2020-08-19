---
title: Tipo de recurso assignedLicense
description: Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade user é uma coleção de **assignedLicense**.
localization_priority: Normal
author: krbain
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b7d03a4f6fd9703a3a24900f12b2e522c6535452
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808393"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="721a5-104">Tipo de recurso assignedLicense</span><span class="sxs-lookup"><span data-stu-id="721a5-104">assignedLicense resource type</span></span>

<span data-ttu-id="721a5-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="721a5-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="721a5-106">Representa uma licença atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="721a5-106">Represents a license assigned to a user.</span></span> <span data-ttu-id="721a5-107">A propriedade **assignedLicenses** da entidade [user](user.md) é uma coleção de **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="721a5-107">The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="721a5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="721a5-108">Properties</span></span>
| <span data-ttu-id="721a5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="721a5-109">Property</span></span>     | <span data-ttu-id="721a5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="721a5-110">Type</span></span>   |<span data-ttu-id="721a5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="721a5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="721a5-112">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="721a5-112">disabledPlans</span></span>|<span data-ttu-id="721a5-113">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="721a5-113">Guid collection</span></span>|<span data-ttu-id="721a5-114">Uma coleção dos identificadores exclusivos de planos que foram desabilitados.</span><span class="sxs-lookup"><span data-stu-id="721a5-114">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="721a5-115">skuId</span><span class="sxs-lookup"><span data-stu-id="721a5-115">skuId</span></span>|<span data-ttu-id="721a5-116">Guid</span><span class="sxs-lookup"><span data-stu-id="721a5-116">Guid</span></span>|<span data-ttu-id="721a5-117">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="721a5-117">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="721a5-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="721a5-118">JSON representation</span></span>

<span data-ttu-id="721a5-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="721a5-119">Here is a JSON representation of the resource</span></span>

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
