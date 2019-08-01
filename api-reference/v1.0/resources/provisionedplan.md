---
title: Tipo de recurso provisionedPlan
description: A propriedade **provisionedPlans** das entidades user e organization é uma coleção de **provisionedPlan**.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3560aab132448a0d13c4b4abe2590d4802cdf9f3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034990"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="6cb75-103">Tipo de recurso provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="6cb75-103">provisionedPlan resource type</span></span>

<span data-ttu-id="6cb75-104">A propriedade **provisionedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="6cb75-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="6cb75-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6cb75-105">Properties</span></span>
| <span data-ttu-id="6cb75-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cb75-106">Property</span></span>     | <span data-ttu-id="6cb75-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cb75-107">Type</span></span>   |<span data-ttu-id="6cb75-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cb75-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cb75-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="6cb75-109">capabilityStatus</span></span>|<span data-ttu-id="6cb75-110">String</span><span class="sxs-lookup"><span data-stu-id="6cb75-110">String</span></span>|<span data-ttu-id="6cb75-111">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="6cb75-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="6cb75-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="6cb75-112">provisioningStatus</span></span>|<span data-ttu-id="6cb75-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cb75-113">String</span></span>|<span data-ttu-id="6cb75-114">Por exemplo, "Success".</span><span class="sxs-lookup"><span data-stu-id="6cb75-114">For example, “Success”.</span></span>|
|<span data-ttu-id="6cb75-115">service</span><span class="sxs-lookup"><span data-stu-id="6cb75-115">service</span></span>|<span data-ttu-id="6cb75-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cb75-116">String</span></span>|<span data-ttu-id="6cb75-117">O nome do serviço; por exemplo, "AccessControlS2S".</span><span class="sxs-lookup"><span data-stu-id="6cb75-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6cb75-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6cb75-118">JSON representation</span></span>

<span data-ttu-id="6cb75-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6cb75-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedPlan"
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
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
