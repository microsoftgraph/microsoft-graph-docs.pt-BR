---
title: Tipo de recurso provisionedPlan
description: A propriedade **provisionedPlans** das entidades user e organization é uma coleção de **provisionedPlan**.
localization_priority: Normal
ms.openlocfilehash: 1d6bec5cdcd4caaf8990caac6614f2fa589d4c4c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344014"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="f6dd4-103">Tipo de recurso provisionedPlan</span><span class="sxs-lookup"><span data-stu-id="f6dd4-103">provisionedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6dd4-104">A propriedade **provisionedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="f6dd4-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="f6dd4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6dd4-105">Properties</span></span>
| <span data-ttu-id="f6dd4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6dd4-106">Property</span></span>     | <span data-ttu-id="f6dd4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6dd4-107">Type</span></span>   |<span data-ttu-id="f6dd4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6dd4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6dd4-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="f6dd4-109">capabilityStatus</span></span>|<span data-ttu-id="f6dd4-110">String</span><span class="sxs-lookup"><span data-stu-id="f6dd4-110">String</span></span>|<span data-ttu-id="f6dd4-111">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="f6dd4-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="f6dd4-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="f6dd4-112">provisioningStatus</span></span>|<span data-ttu-id="f6dd4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6dd4-113">String</span></span>|<span data-ttu-id="f6dd4-114">Por exemplo, "Success".</span><span class="sxs-lookup"><span data-stu-id="f6dd4-114">For example, “Success”.</span></span>|
|<span data-ttu-id="f6dd4-115">service</span><span class="sxs-lookup"><span data-stu-id="f6dd4-115">service</span></span>|<span data-ttu-id="f6dd4-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6dd4-116">String</span></span>|<span data-ttu-id="f6dd4-117">O nome do serviço; por exemplo, "AccessControlS2S".</span><span class="sxs-lookup"><span data-stu-id="f6dd4-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6dd4-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6dd4-118">JSON representation</span></span>

<span data-ttu-id="f6dd4-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f6dd4-119">Here is a JSON representation of the resource</span></span>

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
