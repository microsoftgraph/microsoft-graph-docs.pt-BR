---
title: Tipo de recurso provisionedPlan
description: A propriedade **provisionedPlans** das entidades user e organization é uma coleção de **provisionedPlan**.
localization_priority: Normal
ms.openlocfilehash: 5f9d9c5b2dfffb86643c5e355799f46382bc38cd
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643367"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="0c394-103">Tipo de recurso provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="0c394-103">provisionedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c394-104">A propriedade **provisionedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="0c394-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="0c394-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c394-105">Properties</span></span>
| <span data-ttu-id="0c394-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c394-106">Property</span></span>     | <span data-ttu-id="0c394-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c394-107">Type</span></span>   |<span data-ttu-id="0c394-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c394-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c394-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="0c394-109">capabilityStatus</span></span>|<span data-ttu-id="0c394-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c394-110">String</span></span>|<span data-ttu-id="0c394-111">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="0c394-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="0c394-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="0c394-112">provisioningStatus</span></span>|<span data-ttu-id="0c394-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c394-113">String</span></span>|<span data-ttu-id="0c394-114">Por exemplo, "Success".</span><span class="sxs-lookup"><span data-stu-id="0c394-114">For example, “Success”.</span></span>|
|<span data-ttu-id="0c394-115">service</span><span class="sxs-lookup"><span data-stu-id="0c394-115">service</span></span>|<span data-ttu-id="0c394-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c394-116">String</span></span>|<span data-ttu-id="0c394-117">O nome do serviço; por exemplo, "AccessControlS2S".</span><span class="sxs-lookup"><span data-stu-id="0c394-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c394-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c394-118">JSON representation</span></span>

<span data-ttu-id="0c394-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0c394-119">Here is a JSON representation of the resource</span></span>

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
