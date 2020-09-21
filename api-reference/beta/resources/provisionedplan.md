---
title: Tipo de recurso provisionedPlan
description: A propriedade **provisionedPlans** das entidades user e organization é uma coleção de **provisionedPlan**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: davidmu1
ms.openlocfilehash: da1ecc796c3978195ee974eda4290c7cf9b37f2e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026499"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="509c6-103">Tipo de recurso provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="509c6-103">provisionedPlan resource type</span></span>

<span data-ttu-id="509c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="509c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="509c6-105">A propriedade **provisionedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="509c6-105">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="509c6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="509c6-106">Properties</span></span>
| <span data-ttu-id="509c6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="509c6-107">Property</span></span>     | <span data-ttu-id="509c6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="509c6-108">Type</span></span>   |<span data-ttu-id="509c6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="509c6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="509c6-110">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="509c6-110">capabilityStatus</span></span>|<span data-ttu-id="509c6-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="509c6-111">String</span></span>|<span data-ttu-id="509c6-112">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="509c6-112">For example, “Enabled”.</span></span>|
|<span data-ttu-id="509c6-113">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="509c6-113">provisioningStatus</span></span>|<span data-ttu-id="509c6-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="509c6-114">String</span></span>|<span data-ttu-id="509c6-115">Por exemplo, "Success".</span><span class="sxs-lookup"><span data-stu-id="509c6-115">For example, “Success”.</span></span>|
|<span data-ttu-id="509c6-116">service</span><span class="sxs-lookup"><span data-stu-id="509c6-116">service</span></span>|<span data-ttu-id="509c6-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="509c6-117">String</span></span>|<span data-ttu-id="509c6-118">O nome do serviço; por exemplo, "AccessControlS2S".</span><span class="sxs-lookup"><span data-stu-id="509c6-118">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="509c6-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="509c6-119">JSON representation</span></span>

<span data-ttu-id="509c6-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="509c6-120">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


