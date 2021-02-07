---
title: Tipo de recurso assignedPlan
description: A propriedade **assignedPlans** das entidades user e organization é uma coleção de **assignedPlan**.
localization_priority: Normal
author: krbain
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 44af60c7d74f0a0d21a2312a19853a23cdcbe0ec
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135300"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="9df65-103">Tipo de recurso assignedPlan</span><span class="sxs-lookup"><span data-stu-id="9df65-103">assignedPlan resource type</span></span>

<span data-ttu-id="9df65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9df65-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9df65-105">A propriedade **assignedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="9df65-105">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="9df65-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9df65-106">Properties</span></span>

| <span data-ttu-id="9df65-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9df65-107">Property</span></span>     | <span data-ttu-id="9df65-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9df65-108">Type</span></span>   |<span data-ttu-id="9df65-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9df65-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9df65-110">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="9df65-110">assignedDateTime</span></span>|<span data-ttu-id="9df65-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9df65-111">DateTimeOffset</span></span>|<span data-ttu-id="9df65-p101">A data e hora em que o plano foi atribuído; por exemplo: 2013-01-02T19:32:30Z. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9df65-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9df65-115">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="9df65-115">capabilityStatus</span></span>|[<span data-ttu-id="9df65-116">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="9df65-116">capabilityStatus</span></span>](#capabilitystatus-values)|<span data-ttu-id="9df65-117">Condição da atribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="9df65-117">Condition of the capability assignment.</span></span> <span data-ttu-id="9df65-118">Os valores possíveis `Enabled` são , , , `Warning` `Suspended` `Deleted` `LockedOut` .</span><span class="sxs-lookup"><span data-stu-id="9df65-118">The possible values are `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span>|
|<span data-ttu-id="9df65-119">service</span><span class="sxs-lookup"><span data-stu-id="9df65-119">service</span></span>|<span data-ttu-id="9df65-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9df65-120">String</span></span>|<span data-ttu-id="9df65-121">O nome do serviço; por exemplo, "Exchange".</span><span class="sxs-lookup"><span data-stu-id="9df65-121">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="9df65-122">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="9df65-122">servicePlanId</span></span>|<span data-ttu-id="9df65-123">Guid</span><span class="sxs-lookup"><span data-stu-id="9df65-123">Guid</span></span>|<span data-ttu-id="9df65-124">Um GUID que identifica o plano de serviço.</span><span class="sxs-lookup"><span data-stu-id="9df65-124">A GUID that identifies the service plan.</span></span>|


### <a name="capabilitystatus-values"></a><span data-ttu-id="9df65-125">Valores de capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="9df65-125">capabilityStatus values</span></span>

| <span data-ttu-id="9df65-126">Member</span><span class="sxs-lookup"><span data-stu-id="9df65-126">Member</span></span> | <span data-ttu-id="9df65-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="9df65-127">Description</span></span>  |
|:---------------|:--------|
| <span data-ttu-id="9df65-128">Habilitado</span><span class="sxs-lookup"><span data-stu-id="9df65-128">Enabled</span></span> | <span data-ttu-id="9df65-129">Disponível para uso normal.</span><span class="sxs-lookup"><span data-stu-id="9df65-129">Available for normal use.</span></span> |
| <span data-ttu-id="9df65-130">Aviso</span><span class="sxs-lookup"><span data-stu-id="9df65-130">Warning</span></span> | <span data-ttu-id="9df65-131">Disponível para uso normal, mas está em um período de carência.</span><span class="sxs-lookup"><span data-stu-id="9df65-131">Available for normal use but is in a grace period.</span></span> |
| <span data-ttu-id="9df65-132">Suspenso</span><span class="sxs-lookup"><span data-stu-id="9df65-132">Suspended</span></span> | <span data-ttu-id="9df65-133">Indisponível, mas todos os dados associados à funcionalidade devem ser preservados.</span><span class="sxs-lookup"><span data-stu-id="9df65-133">Unavailable but any data associated with the capability must be preserved.</span></span> |
| <span data-ttu-id="9df65-134">Deleted</span><span class="sxs-lookup"><span data-stu-id="9df65-134">Deleted</span></span> | <span data-ttu-id="9df65-135">Indisponível e quaisquer dados associados à funcionalidade podem ser excluídos.</span><span class="sxs-lookup"><span data-stu-id="9df65-135">Unavailable and any data associated with the capability may be deleted.</span></span> |
| <span data-ttu-id="9df65-136">LockedOut</span><span class="sxs-lookup"><span data-stu-id="9df65-136">LockedOut</span></span> | <span data-ttu-id="9df65-137">Indisponível para todos os administradores e usuários, mas todos os dados associados à funcionalidade devem ser preservados.</span><span class="sxs-lookup"><span data-stu-id="9df65-137">Unavailable for all administrators and users but any data associated with the capability must be preserved.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9df65-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9df65-138">JSON representation</span></span>

<span data-ttu-id="9df65-139">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9df65-139">Here is a JSON representation of the resource</span></span>

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

