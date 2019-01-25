---
title: Tipo de recurso assignedLicense
description: Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade **user** é uma coleção de assignedLicense.
localization_priority: Normal
ms.openlocfilehash: 2d9620ec33a296c09ced9bc9d8af8d6d032bb7d9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524916"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="e6225-104">Tipo de recurso assignedLicense</span><span class="sxs-lookup"><span data-stu-id="e6225-104">assignedLicense resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6225-p102">Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade [user](user.md) é uma coleção de **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="e6225-p102">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="e6225-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6225-107">Properties</span></span>
| <span data-ttu-id="e6225-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6225-108">Property</span></span>     | <span data-ttu-id="e6225-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6225-109">Type</span></span>   |<span data-ttu-id="e6225-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6225-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6225-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="e6225-111">disabledPlans</span></span>|<span data-ttu-id="e6225-112">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="e6225-112">Guid collection</span></span>|<span data-ttu-id="e6225-113">Uma coleção dos identificadores exclusivos de planos que foram desabilitados.</span><span class="sxs-lookup"><span data-stu-id="e6225-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="e6225-114">skuId</span><span class="sxs-lookup"><span data-stu-id="e6225-114">skuId</span></span>|<span data-ttu-id="e6225-115">Guid</span><span class="sxs-lookup"><span data-stu-id="e6225-115">Guid</span></span>|<span data-ttu-id="e6225-116">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="e6225-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6225-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6225-117">JSON representation</span></span>

<span data-ttu-id="e6225-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e6225-118">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/assignedlicense.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
