---
title: Tipo de recurso provisionedPlan
description: A propriedade **provisionedPlans** das entidades user e organization é uma coleção de **provisionedPlan**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: 1fed61db1de92ba330d233725774e4978abe72ff
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469434"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="75e00-103">Tipo de recurso provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="75e00-103">provisionedPlan resource type</span></span>

<span data-ttu-id="75e00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75e00-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75e00-105">A propriedade **provisionedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="75e00-105">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="75e00-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75e00-106">Properties</span></span>
| <span data-ttu-id="75e00-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75e00-107">Property</span></span>     | <span data-ttu-id="75e00-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="75e00-108">Type</span></span>   |<span data-ttu-id="75e00-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="75e00-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75e00-110">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="75e00-110">capabilityStatus</span></span>|<span data-ttu-id="75e00-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75e00-111">String</span></span>|<span data-ttu-id="75e00-112">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="75e00-112">For example, “Enabled”.</span></span>|
|<span data-ttu-id="75e00-113">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="75e00-113">provisioningStatus</span></span>|<span data-ttu-id="75e00-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75e00-114">String</span></span>|<span data-ttu-id="75e00-115">Por exemplo, "Success".</span><span class="sxs-lookup"><span data-stu-id="75e00-115">For example, “Success”.</span></span>|
|<span data-ttu-id="75e00-116">service</span><span class="sxs-lookup"><span data-stu-id="75e00-116">service</span></span>|<span data-ttu-id="75e00-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75e00-117">String</span></span>|<span data-ttu-id="75e00-118">O nome do serviço; por exemplo, "AccessControlS2S".</span><span class="sxs-lookup"><span data-stu-id="75e00-118">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75e00-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75e00-119">JSON representation</span></span>

<span data-ttu-id="75e00-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="75e00-120">Here is a JSON representation of the resource</span></span>

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


