---
title: Tipo de recurso assignedPlan
description: A propriedade **assignedPlans** das entidades user e organization é uma coleção de **assignedPlan**.
ms.openlocfilehash: 0df1540819b569b62607bf0e56c1c8f53d2749da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033428"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="354d7-103">Tipo de recurso assignedPlan</span><span class="sxs-lookup"><span data-stu-id="354d7-103">assignedPlan resource type</span></span>

> <span data-ttu-id="354d7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="354d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="354d7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="354d7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="354d7-106">A propriedade **assignedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="354d7-106">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="354d7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="354d7-107">Properties</span></span>
| <span data-ttu-id="354d7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="354d7-108">Property</span></span>     | <span data-ttu-id="354d7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="354d7-109">Type</span></span>   |<span data-ttu-id="354d7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="354d7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="354d7-111">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="354d7-111">assignedDateTime</span></span>|<span data-ttu-id="354d7-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="354d7-112">DateTimeOffset</span></span>|<span data-ttu-id="354d7-p102">A data e hora em que o plano foi atribuído; por exemplo: 2013-01-02T19:32:30Z. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="354d7-p102">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="354d7-116">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="354d7-116">capabilityStatus</span></span>|<span data-ttu-id="354d7-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="354d7-117">String</span></span>|<span data-ttu-id="354d7-118">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="354d7-118">For example, “Enabled”.</span></span>|
|<span data-ttu-id="354d7-119">service</span><span class="sxs-lookup"><span data-stu-id="354d7-119">service</span></span>|<span data-ttu-id="354d7-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="354d7-120">String</span></span>|<span data-ttu-id="354d7-121">O nome do serviço; por exemplo, "Exchange".</span><span class="sxs-lookup"><span data-stu-id="354d7-121">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="354d7-122">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="354d7-122">servicePlanId</span></span>|<span data-ttu-id="354d7-123">Guid</span><span class="sxs-lookup"><span data-stu-id="354d7-123">Guid</span></span>|<span data-ttu-id="354d7-124">Um GUID que identifica o plano de serviço.</span><span class="sxs-lookup"><span data-stu-id="354d7-124">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="354d7-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="354d7-125">JSON representation</span></span>

<span data-ttu-id="354d7-126">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="354d7-126">Here is a JSON representation of the resource</span></span>

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
