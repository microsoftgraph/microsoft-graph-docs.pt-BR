---
title: Tipo de recurso assignedPlan
description: A propriedade **assignedPlans** das entidades user e organization é uma coleção de **assignedPlan**.
localization_priority: Normal
ms.openlocfilehash: d1f3df6a88ab688206d26db6fc0afe1e1d4a4f60
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852994"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="74649-103">Tipo de recurso assignedPlan</span><span class="sxs-lookup"><span data-stu-id="74649-103">assignedPlan resource type</span></span>

<span data-ttu-id="74649-104">A propriedade **assignedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="74649-104">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="74649-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74649-105">Properties</span></span>
| <span data-ttu-id="74649-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74649-106">Property</span></span>     | <span data-ttu-id="74649-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="74649-107">Type</span></span>   |<span data-ttu-id="74649-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="74649-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74649-109">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="74649-109">assignedDateTime</span></span>|<span data-ttu-id="74649-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74649-110">DateTimeOffset</span></span>|<span data-ttu-id="74649-p101">A data e hora em que o plano foi atribuído; por exemplo: 2013-01-02T19:32:30Z. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="74649-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="74649-114">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="74649-114">capabilityStatus</span></span>|<span data-ttu-id="74649-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74649-115">String</span></span>|<span data-ttu-id="74649-116">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="74649-116">For example, “Enabled”.</span></span>|
|<span data-ttu-id="74649-117">service</span><span class="sxs-lookup"><span data-stu-id="74649-117">service</span></span>|<span data-ttu-id="74649-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74649-118">String</span></span>|<span data-ttu-id="74649-119">O nome do serviço; por exemplo, "Exchange".</span><span class="sxs-lookup"><span data-stu-id="74649-119">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="74649-120">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="74649-120">servicePlanId</span></span>|<span data-ttu-id="74649-121">Guid</span><span class="sxs-lookup"><span data-stu-id="74649-121">Guid</span></span>|<span data-ttu-id="74649-122">Um GUID que identifica o plano de serviço.</span><span class="sxs-lookup"><span data-stu-id="74649-122">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74649-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74649-123">JSON representation</span></span>

<span data-ttu-id="74649-124">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="74649-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
