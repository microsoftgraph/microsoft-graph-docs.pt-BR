---
title: Tipo de recurso provisionedPlan
description: A propriedade **provisionedPlans** das entidades user e organization é uma coleção de **provisionedPlan**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 76c29a74d54ca6e02febe8c83c80072bf158aa6b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965543"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="52ca7-103">Tipo de recurso provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="52ca7-103">provisionedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52ca7-104">A propriedade **provisionedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="52ca7-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="52ca7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52ca7-105">Properties</span></span>
| <span data-ttu-id="52ca7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52ca7-106">Property</span></span>     | <span data-ttu-id="52ca7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="52ca7-107">Type</span></span>   |<span data-ttu-id="52ca7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="52ca7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52ca7-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="52ca7-109">capabilityStatus</span></span>|<span data-ttu-id="52ca7-110">String</span><span class="sxs-lookup"><span data-stu-id="52ca7-110">String</span></span>|<span data-ttu-id="52ca7-111">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="52ca7-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="52ca7-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="52ca7-112">provisioningStatus</span></span>|<span data-ttu-id="52ca7-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52ca7-113">String</span></span>|<span data-ttu-id="52ca7-114">Por exemplo, "Success".</span><span class="sxs-lookup"><span data-stu-id="52ca7-114">For example, “Success”.</span></span>|
|<span data-ttu-id="52ca7-115">service</span><span class="sxs-lookup"><span data-stu-id="52ca7-115">service</span></span>|<span data-ttu-id="52ca7-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52ca7-116">String</span></span>|<span data-ttu-id="52ca7-117">O nome do serviço; por exemplo, "AccessControlS2S".</span><span class="sxs-lookup"><span data-stu-id="52ca7-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52ca7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52ca7-118">JSON representation</span></span>

<span data-ttu-id="52ca7-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="52ca7-119">Here is a JSON representation of the resource</span></span>

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
