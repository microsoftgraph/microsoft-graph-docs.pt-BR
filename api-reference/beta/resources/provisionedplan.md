---
title: Tipo de recurso provisionedPlan
description: A propriedade **provisionedPlans** das entidades **user** e organization é uma coleção de provisionedPlan.
localization_priority: Normal
ms.openlocfilehash: 5f9d9c5b2dfffb86643c5e355799f46382bc38cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527812"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="860fa-103">Tipo de recurso provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="860fa-103">provisionedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="860fa-104">A propriedade **provisionedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="860fa-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="860fa-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="860fa-105">Properties</span></span>
| <span data-ttu-id="860fa-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="860fa-106">Property</span></span>     | <span data-ttu-id="860fa-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="860fa-107">Type</span></span>   |<span data-ttu-id="860fa-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="860fa-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="860fa-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="860fa-109">capabilityStatus</span></span>|<span data-ttu-id="860fa-110">String</span><span class="sxs-lookup"><span data-stu-id="860fa-110">String</span></span>|<span data-ttu-id="860fa-111">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="860fa-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="860fa-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="860fa-112">provisioningStatus</span></span>|<span data-ttu-id="860fa-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="860fa-113">String</span></span>|<span data-ttu-id="860fa-114">Por exemplo, "Success".</span><span class="sxs-lookup"><span data-stu-id="860fa-114">For example, “Success”.</span></span>|
|<span data-ttu-id="860fa-115">service</span><span class="sxs-lookup"><span data-stu-id="860fa-115">service</span></span>|<span data-ttu-id="860fa-116">String</span><span class="sxs-lookup"><span data-stu-id="860fa-116">String</span></span>|<span data-ttu-id="860fa-117">O nome do serviço; por exemplo, "AccessControlS2S".</span><span class="sxs-lookup"><span data-stu-id="860fa-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="860fa-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="860fa-118">JSON representation</span></span>

<span data-ttu-id="860fa-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="860fa-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedplan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/provisionedplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
