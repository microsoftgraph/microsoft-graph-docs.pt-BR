---
title: Tipo de recurso assignedLicense
description: Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade user é uma coleção de **assignedLicense**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jpettere
ms.openlocfilehash: 4014198d211c2955866b1a56d80377e19ba4a38f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721849"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="55136-104">Tipo de recurso assignedLicense</span><span class="sxs-lookup"><span data-stu-id="55136-104">assignedLicense resource type</span></span>

<span data-ttu-id="55136-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55136-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55136-106">Representa uma licença atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="55136-106">Represents a license assigned to a user.</span></span> <span data-ttu-id="55136-107">A propriedade **assignedLicenses** da entidade [user](user.md) é uma coleção de **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="55136-107">The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="55136-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55136-108">Properties</span></span>
| <span data-ttu-id="55136-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55136-109">Property</span></span>     | <span data-ttu-id="55136-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="55136-110">Type</span></span>   |<span data-ttu-id="55136-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="55136-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55136-112">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="55136-112">disabledPlans</span></span>|<span data-ttu-id="55136-113">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="55136-113">Guid collection</span></span>|<span data-ttu-id="55136-114">Uma coleção dos identificadores exclusivos de planos que foram desabilitados.</span><span class="sxs-lookup"><span data-stu-id="55136-114">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="55136-115">skuId</span><span class="sxs-lookup"><span data-stu-id="55136-115">skuId</span></span>|<span data-ttu-id="55136-116">Guid</span><span class="sxs-lookup"><span data-stu-id="55136-116">Guid</span></span>|<span data-ttu-id="55136-117">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="55136-117">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55136-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55136-118">JSON representation</span></span>

<span data-ttu-id="55136-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="55136-119">Here is a JSON representation of the resource</span></span>

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


