---
title: Tipo de recurso assignedPlan
description: A propriedade **assignedPlans** das entidades user e organization é uma coleção de **assignedPlan**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: krbain
ms.openlocfilehash: fe546f2dd25ca7f65e1ce8299bfad9b9ce5be56d
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563419"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="dbd86-103">Tipo de recurso assignedPlan</span><span class="sxs-lookup"><span data-stu-id="dbd86-103">assignedPlan resource type</span></span>

<span data-ttu-id="dbd86-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbd86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbd86-105">A propriedade **assignedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="dbd86-105">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="dbd86-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbd86-106">Properties</span></span>

| <span data-ttu-id="dbd86-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbd86-107">Property</span></span>     | <span data-ttu-id="dbd86-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbd86-108">Type</span></span>   |<span data-ttu-id="dbd86-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbd86-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbd86-110">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbd86-110">assignedDateTime</span></span>|<span data-ttu-id="dbd86-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbd86-111">DateTimeOffset</span></span>|<span data-ttu-id="dbd86-p101">A data e hora em que o plano foi atribuído; por exemplo: 2013-01-02T19:32:30Z. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="dbd86-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="dbd86-115">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="dbd86-115">capabilityStatus</span></span>|[<span data-ttu-id="dbd86-116">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="dbd86-116">capabilityStatus</span></span>](#capabilitystatus-values)|<span data-ttu-id="dbd86-117">Condição da atribuição de recurso.</span><span class="sxs-lookup"><span data-stu-id="dbd86-117">Condition of the capability assignment.</span></span> <span data-ttu-id="dbd86-118">Os valores possíveis são:,,, `Enabled` `Warning` `Suspended` `Deleted` , `LockedOut` .</span><span class="sxs-lookup"><span data-stu-id="dbd86-118">The possible values are `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span>|
|<span data-ttu-id="dbd86-119">service</span><span class="sxs-lookup"><span data-stu-id="dbd86-119">service</span></span>|<span data-ttu-id="dbd86-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbd86-120">String</span></span>|<span data-ttu-id="dbd86-121">O nome do serviço; por exemplo, "Exchange".</span><span class="sxs-lookup"><span data-stu-id="dbd86-121">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="dbd86-122">onplanid</span><span class="sxs-lookup"><span data-stu-id="dbd86-122">servicePlanId</span></span>|<span data-ttu-id="dbd86-123">Guid</span><span class="sxs-lookup"><span data-stu-id="dbd86-123">Guid</span></span>|<span data-ttu-id="dbd86-124">Um GUID que identifica o plano de serviço.</span><span class="sxs-lookup"><span data-stu-id="dbd86-124">A GUID that identifies the service plan.</span></span>|


### <a name="capabilitystatus-values"></a><span data-ttu-id="dbd86-125">valores de capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="dbd86-125">capabilityStatus values</span></span>

| <span data-ttu-id="dbd86-126">Member</span><span class="sxs-lookup"><span data-stu-id="dbd86-126">Member</span></span> | <span data-ttu-id="dbd86-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbd86-127">Description</span></span>  |
|:---------------|:--------|
| <span data-ttu-id="dbd86-128">Habilitado</span><span class="sxs-lookup"><span data-stu-id="dbd86-128">Enabled</span></span> | <span data-ttu-id="dbd86-129">Disponível para uso normal.</span><span class="sxs-lookup"><span data-stu-id="dbd86-129">Available for normal use.</span></span> |
| <span data-ttu-id="dbd86-130">Aviso</span><span class="sxs-lookup"><span data-stu-id="dbd86-130">Warning</span></span> | <span data-ttu-id="dbd86-131">Disponível para uso normal, mas está em um período de cortesia.</span><span class="sxs-lookup"><span data-stu-id="dbd86-131">Available for normal use but is in a grace period.</span></span> |
| <span data-ttu-id="dbd86-132">Suspensão</span><span class="sxs-lookup"><span data-stu-id="dbd86-132">Suspended</span></span> | <span data-ttu-id="dbd86-133">Indisponível, mas os dados associados ao recurso devem ser preservados.</span><span class="sxs-lookup"><span data-stu-id="dbd86-133">Unavailable but any data associated with the capability must be preserved.</span></span> |
| <span data-ttu-id="dbd86-134">Deleted</span><span class="sxs-lookup"><span data-stu-id="dbd86-134">Deleted</span></span> | <span data-ttu-id="dbd86-135">Indisponível e todos os dados associados ao recurso podem ser excluídos.</span><span class="sxs-lookup"><span data-stu-id="dbd86-135">Unavailable and any data associated with the capability may be deleted.</span></span> |
| <span data-ttu-id="dbd86-136">Bloqueado</span><span class="sxs-lookup"><span data-stu-id="dbd86-136">LockedOut</span></span> | <span data-ttu-id="dbd86-137">Indisponível para todos os administradores e usuários, mas os dados associados ao recurso devem ser preservados.</span><span class="sxs-lookup"><span data-stu-id="dbd86-137">Unavailable for all administrators and users but any data associated with the capability must be preserved.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dbd86-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbd86-138">JSON representation</span></span>

<span data-ttu-id="dbd86-139">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="dbd86-139">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


