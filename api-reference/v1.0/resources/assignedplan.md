---
title: Tipo de recurso assignedPlan
description: A propriedade **assignedPlans** das entidades user e organization é uma coleção de **assignedPlan**.
localization_priority: Normal
author: jpettere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 182ef3239437234c74945fa37483924429f2200b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958091"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="44959-103">Tipo de recurso assignedPlan</span><span class="sxs-lookup"><span data-stu-id="44959-103">assignedPlan resource type</span></span>

<span data-ttu-id="44959-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44959-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44959-105">A propriedade **assignedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="44959-105">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="44959-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44959-106">Properties</span></span>

| <span data-ttu-id="44959-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44959-107">Property</span></span>     | <span data-ttu-id="44959-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="44959-108">Type</span></span>   |<span data-ttu-id="44959-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="44959-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44959-110">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="44959-110">assignedDateTime</span></span>|<span data-ttu-id="44959-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44959-111">DateTimeOffset</span></span>|<span data-ttu-id="44959-112">A data e a hora em que o plano foi atribuído.</span><span class="sxs-lookup"><span data-stu-id="44959-112">The date and time at which the plan was assigned.</span></span> <span data-ttu-id="44959-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="44959-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="44959-114">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="44959-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="44959-115">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="44959-115">capabilityStatus</span></span>|<span data-ttu-id="44959-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44959-116">String</span></span>|<span data-ttu-id="44959-117">Condição da atribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="44959-117">Condition of the capability assignment.</span></span> <span data-ttu-id="44959-118">Os valores possíveis `Enabled` são , , , , `Warning` `Suspended` `Deleted` `LockedOut` .</span><span class="sxs-lookup"><span data-stu-id="44959-118">The possible values are `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> <span data-ttu-id="44959-119">Consulte [uma descrição detalhada](#capabilitystatus-values) de cada valor.</span><span class="sxs-lookup"><span data-stu-id="44959-119">See [a detailed description](#capabilitystatus-values) of each value.</span></span>|
|<span data-ttu-id="44959-120">service</span><span class="sxs-lookup"><span data-stu-id="44959-120">service</span></span>|<span data-ttu-id="44959-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44959-121">String</span></span>|<span data-ttu-id="44959-122">O nome do serviço; por exemplo, "Exchange".</span><span class="sxs-lookup"><span data-stu-id="44959-122">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="44959-123">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="44959-123">servicePlanId</span></span>|<span data-ttu-id="44959-124">Guid</span><span class="sxs-lookup"><span data-stu-id="44959-124">Guid</span></span>|<span data-ttu-id="44959-125">Um GUID que identifica o plano de serviço.</span><span class="sxs-lookup"><span data-stu-id="44959-125">A GUID that identifies the service plan.</span></span>|


### <a name="capabilitystatus-values"></a><span data-ttu-id="44959-126">valores de capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="44959-126">capabilityStatus values</span></span>

| <span data-ttu-id="44959-127">Member</span><span class="sxs-lookup"><span data-stu-id="44959-127">Member</span></span> | <span data-ttu-id="44959-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="44959-128">Description</span></span>  |
|:---------------|:--------|
| <span data-ttu-id="44959-129">Habilitado</span><span class="sxs-lookup"><span data-stu-id="44959-129">Enabled</span></span> | <span data-ttu-id="44959-130">Disponível para uso normal.</span><span class="sxs-lookup"><span data-stu-id="44959-130">Available for normal use.</span></span> |
| <span data-ttu-id="44959-131">Aviso</span><span class="sxs-lookup"><span data-stu-id="44959-131">Warning</span></span> | <span data-ttu-id="44959-132">Disponível para uso normal, mas está em um período de carência.</span><span class="sxs-lookup"><span data-stu-id="44959-132">Available for normal use but is in a grace period.</span></span> |
| <span data-ttu-id="44959-133">Suspenso</span><span class="sxs-lookup"><span data-stu-id="44959-133">Suspended</span></span> | <span data-ttu-id="44959-134">Indisponível, mas todos os dados associados à funcionalidade devem ser preservados.</span><span class="sxs-lookup"><span data-stu-id="44959-134">Unavailable but any data associated with the capability must be preserved.</span></span> |
| <span data-ttu-id="44959-135">Excluída</span><span class="sxs-lookup"><span data-stu-id="44959-135">Deleted</span></span> | <span data-ttu-id="44959-136">Indisponíveis e quaisquer dados associados à funcionalidade podem ser excluídos.</span><span class="sxs-lookup"><span data-stu-id="44959-136">Unavailable and any data associated with the capability may be deleted.</span></span> |
| <span data-ttu-id="44959-137">LockedOut</span><span class="sxs-lookup"><span data-stu-id="44959-137">LockedOut</span></span> | <span data-ttu-id="44959-138">Indisponível para todos os administradores e usuários, mas todos os dados associados à funcionalidade devem ser preservados.</span><span class="sxs-lookup"><span data-stu-id="44959-138">Unavailable for all administrators and users but any data associated with the capability must be preserved.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="44959-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44959-139">JSON representation</span></span>

<span data-ttu-id="44959-140">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="44959-140">Here is a JSON representation of the resource</span></span>

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

