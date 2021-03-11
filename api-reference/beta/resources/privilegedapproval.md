---
title: Tipo de recurso privilegedApproval
description: Representa uma aprovação solicitada no Privileged Identity Management para entrar em uma função.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 7d7842b89bce06d582aa827b853e4170b0693ff8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721604"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="2f9cc-103">Tipo de recurso privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="2f9cc-103">privilegedApproval resource type</span></span>

<span data-ttu-id="2f9cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f9cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f9cc-105">Representa uma aprovação solicitada no Privileged Identity Management para entrar em uma função.</span><span class="sxs-lookup"><span data-stu-id="2f9cc-105">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="2f9cc-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2f9cc-106">Methods</span></span>

| <span data-ttu-id="2f9cc-107">Método</span><span class="sxs-lookup"><span data-stu-id="2f9cc-107">Method</span></span>           | <span data-ttu-id="2f9cc-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2f9cc-108">Return Type</span></span>    |<span data-ttu-id="2f9cc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f9cc-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f9cc-110">Get privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="2f9cc-110">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="2f9cc-111">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="2f9cc-111">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="2f9cc-112">Ler propriedades e relações do objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="2f9cc-112">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="2f9cc-113">Listar objetos privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="2f9cc-113">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="2f9cc-114">[privilegedApproval](privilegedapproval.md) collection</span><span class="sxs-lookup"><span data-stu-id="2f9cc-114">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="2f9cc-115">Obter a coleção privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="2f9cc-115">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="2f9cc-116">Create privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="2f9cc-116">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="2f9cc-117">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="2f9cc-117">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="2f9cc-118">Crie um objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="2f9cc-118">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="2f9cc-119">Update privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="2f9cc-119">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="2f9cc-120">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="2f9cc-120">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="2f9cc-121">Atualize um objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="2f9cc-121">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="2f9cc-122">Myrequests</span><span class="sxs-lookup"><span data-stu-id="2f9cc-122">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="2f9cc-123">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="2f9cc-123">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="2f9cc-124">Receba solicitações de aprovação do solicitante.</span><span class="sxs-lookup"><span data-stu-id="2f9cc-124">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="2f9cc-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f9cc-125">Properties</span></span>
| <span data-ttu-id="2f9cc-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f9cc-126">Property</span></span>     | <span data-ttu-id="2f9cc-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f9cc-127">Type</span></span>   |<span data-ttu-id="2f9cc-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f9cc-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f9cc-129">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="2f9cc-129">approvalDuration</span></span>|<span data-ttu-id="2f9cc-130">Duration</span><span class="sxs-lookup"><span data-stu-id="2f9cc-130">Duration</span></span>||
|<span data-ttu-id="2f9cc-131">approvalState</span><span class="sxs-lookup"><span data-stu-id="2f9cc-131">approvalState</span></span>|<span data-ttu-id="2f9cc-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f9cc-132">string</span></span>| <span data-ttu-id="2f9cc-133">Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="2f9cc-133">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="2f9cc-134">approvalType</span><span class="sxs-lookup"><span data-stu-id="2f9cc-134">approvalType</span></span>|<span data-ttu-id="2f9cc-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f9cc-135">String</span></span>||
|<span data-ttu-id="2f9cc-136">approverReason</span><span class="sxs-lookup"><span data-stu-id="2f9cc-136">approverReason</span></span>|<span data-ttu-id="2f9cc-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f9cc-137">String</span></span>||
|<span data-ttu-id="2f9cc-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2f9cc-138">endDateTime</span></span>|<span data-ttu-id="2f9cc-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f9cc-139">DateTimeOffset</span></span>|<span data-ttu-id="2f9cc-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2f9cc-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2f9cc-141">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="2f9cc-141">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="2f9cc-142">id</span><span class="sxs-lookup"><span data-stu-id="2f9cc-142">id</span></span>|<span data-ttu-id="2f9cc-143">String</span><span class="sxs-lookup"><span data-stu-id="2f9cc-143">String</span></span>| <span data-ttu-id="2f9cc-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f9cc-144">Read-only.</span></span>|
|<span data-ttu-id="2f9cc-145">requestorReason</span><span class="sxs-lookup"><span data-stu-id="2f9cc-145">requestorReason</span></span>|<span data-ttu-id="2f9cc-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f9cc-146">String</span></span>||
|<span data-ttu-id="2f9cc-147">roleId</span><span class="sxs-lookup"><span data-stu-id="2f9cc-147">roleId</span></span>|<span data-ttu-id="2f9cc-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f9cc-148">String</span></span>||
|<span data-ttu-id="2f9cc-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2f9cc-149">startDateTime</span></span>|<span data-ttu-id="2f9cc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f9cc-150">DateTimeOffset</span></span>|<span data-ttu-id="2f9cc-151">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2f9cc-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2f9cc-152">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="2f9cc-152">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="2f9cc-153">userId</span><span class="sxs-lookup"><span data-stu-id="2f9cc-153">userId</span></span>|<span data-ttu-id="2f9cc-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f9cc-154">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="2f9cc-155">Relações</span><span class="sxs-lookup"><span data-stu-id="2f9cc-155">Relationships</span></span>
| <span data-ttu-id="2f9cc-156">Relação</span><span class="sxs-lookup"><span data-stu-id="2f9cc-156">Relationship</span></span> | <span data-ttu-id="2f9cc-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f9cc-157">Type</span></span>   |<span data-ttu-id="2f9cc-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f9cc-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f9cc-159">roleInfo</span><span class="sxs-lookup"><span data-stu-id="2f9cc-159">roleInfo</span></span>|[<span data-ttu-id="2f9cc-160">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="2f9cc-160">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="2f9cc-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f9cc-161">Read-only.</span></span> <span data-ttu-id="2f9cc-162">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f9cc-162">Nullable.</span></span>|
|<span data-ttu-id="2f9cc-163">request</span><span class="sxs-lookup"><span data-stu-id="2f9cc-163">request</span></span>|[<span data-ttu-id="2f9cc-164">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2f9cc-164">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="2f9cc-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f9cc-165">Read-only.</span></span> <span data-ttu-id="2f9cc-166">A solicitação de atribuição de função para este objeto de aprovação</span><span class="sxs-lookup"><span data-stu-id="2f9cc-166">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f9cc-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f9cc-167">JSON representation</span></span>
<span data-ttu-id="2f9cc-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2f9cc-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedApproval"
}-->

```json
{
  "approvalDuration": "string (timestamp)",
  "approvalState": "string",
  "approvalType": "string",
  "approverReason": "String",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "requestorReason": "String",
  "roleId": "String",
  "startDateTime": "String (timestamp)",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


