---
title: Tipo de recurso assignedPlan
description: A propriedade **assignedPlans** das entidades user e organization é uma coleção de **assignedPlan**.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cff3987994b33be39dd274bfdd303db908a1eb7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533137"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="348fe-103">Tipo de recurso assignedPlan</span><span class="sxs-lookup"><span data-stu-id="348fe-103">assignedPlan resource type</span></span>

<span data-ttu-id="348fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="348fe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="348fe-105">A propriedade **assignedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="348fe-105">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="348fe-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="348fe-106">Properties</span></span>
| <span data-ttu-id="348fe-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="348fe-107">Property</span></span>     | <span data-ttu-id="348fe-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="348fe-108">Type</span></span>   |<span data-ttu-id="348fe-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="348fe-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="348fe-110">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="348fe-110">assignedDateTime</span></span>|<span data-ttu-id="348fe-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="348fe-111">DateTimeOffset</span></span>|<span data-ttu-id="348fe-p101">A data e hora em que o plano foi atribuído; por exemplo: 2013-01-02T19:32:30Z. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="348fe-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="348fe-115">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="348fe-115">capabilityStatus</span></span>|<span data-ttu-id="348fe-116">String</span><span class="sxs-lookup"><span data-stu-id="348fe-116">String</span></span>|<span data-ttu-id="348fe-117">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="348fe-117">For example, “Enabled”.</span></span>|
|<span data-ttu-id="348fe-118">service</span><span class="sxs-lookup"><span data-stu-id="348fe-118">service</span></span>|<span data-ttu-id="348fe-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="348fe-119">String</span></span>|<span data-ttu-id="348fe-120">O nome do serviço; por exemplo, "Exchange".</span><span class="sxs-lookup"><span data-stu-id="348fe-120">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="348fe-121">onplanid</span><span class="sxs-lookup"><span data-stu-id="348fe-121">servicePlanId</span></span>|<span data-ttu-id="348fe-122">Guid</span><span class="sxs-lookup"><span data-stu-id="348fe-122">Guid</span></span>|<span data-ttu-id="348fe-123">Um GUID que identifica o plano de serviço.</span><span class="sxs-lookup"><span data-stu-id="348fe-123">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="348fe-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="348fe-124">JSON representation</span></span>

<span data-ttu-id="348fe-125">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="348fe-125">Here is a JSON representation of the resource</span></span>

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
