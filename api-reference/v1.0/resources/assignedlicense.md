---
title: Tipo de recurso assignedLicense
description: Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade user é uma coleção de **assignedLicense**.
ms.openlocfilehash: 48863a9acdcfa173a3f0c1a2a008516360ffdf9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004574"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="5f978-104">Tipo de recurso assignedLicense</span><span class="sxs-lookup"><span data-stu-id="5f978-104">assignedLicense resource type</span></span>

<span data-ttu-id="5f978-p102">Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade [user](user.md) é uma coleção de **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="5f978-p102">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="5f978-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f978-107">Properties</span></span>
| <span data-ttu-id="5f978-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f978-108">Property</span></span>     | <span data-ttu-id="5f978-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f978-109">Type</span></span>   |<span data-ttu-id="5f978-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f978-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f978-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="5f978-111">disabledPlans</span></span>|<span data-ttu-id="5f978-112">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="5f978-112">Guid collection</span></span>|<span data-ttu-id="5f978-113">Uma coleção dos identificadores exclusivos de planos que foram desabilitados.</span><span class="sxs-lookup"><span data-stu-id="5f978-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="5f978-114">skuId</span><span class="sxs-lookup"><span data-stu-id="5f978-114">skuId</span></span>|<span data-ttu-id="5f978-115">Guid</span><span class="sxs-lookup"><span data-stu-id="5f978-115">Guid</span></span>|<span data-ttu-id="5f978-116">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="5f978-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f978-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f978-117">JSON representation</span></span>

<span data-ttu-id="5f978-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5f978-118">Here is a JSON representation of the resource</span></span>

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
