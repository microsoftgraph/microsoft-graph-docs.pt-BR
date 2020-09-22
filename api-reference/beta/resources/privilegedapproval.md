---
title: tipo de recurso privilegedApproval
description: Representa uma aprovação solicitada no gerenciamento de identidade privilegiado para obter uma função.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: cd6f352ad114307933682f4d6df22408b54ebc73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070580"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="f2e05-103">tipo de recurso privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f2e05-103">privilegedApproval resource type</span></span>

<span data-ttu-id="f2e05-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2e05-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2e05-105">Representa uma aprovação solicitada no gerenciamento de identidade privilegiado para obter uma função.</span><span class="sxs-lookup"><span data-stu-id="f2e05-105">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="f2e05-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f2e05-106">Methods</span></span>

| <span data-ttu-id="f2e05-107">Método</span><span class="sxs-lookup"><span data-stu-id="f2e05-107">Method</span></span>           | <span data-ttu-id="f2e05-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f2e05-108">Return Type</span></span>    |<span data-ttu-id="f2e05-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2e05-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2e05-110">Get privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f2e05-110">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="f2e05-111">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f2e05-111">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="f2e05-112">Leia as propriedades e os relacionamentos do objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="f2e05-112">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="f2e05-113">Listar objetos privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f2e05-113">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="f2e05-114">[privilegedApproval](privilegedapproval.md) collection</span><span class="sxs-lookup"><span data-stu-id="f2e05-114">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="f2e05-115">Obtenha a coleção de privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="f2e05-115">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="f2e05-116">Create privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f2e05-116">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="f2e05-117">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f2e05-117">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="f2e05-118">Crie um objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="f2e05-118">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="f2e05-119">Update privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f2e05-119">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="f2e05-120">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f2e05-120">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="f2e05-121">Atualize um objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="f2e05-121">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="f2e05-122">Myrequests</span><span class="sxs-lookup"><span data-stu-id="f2e05-122">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="f2e05-123">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f2e05-123">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="f2e05-124">Receba solicitações de aprovação do solicitante.</span><span class="sxs-lookup"><span data-stu-id="f2e05-124">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2e05-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2e05-125">Properties</span></span>
| <span data-ttu-id="f2e05-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2e05-126">Property</span></span>     | <span data-ttu-id="f2e05-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2e05-127">Type</span></span>   |<span data-ttu-id="f2e05-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2e05-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2e05-129">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="f2e05-129">approvalDuration</span></span>|<span data-ttu-id="f2e05-130">Duração</span><span class="sxs-lookup"><span data-stu-id="f2e05-130">Duration</span></span>||
|<span data-ttu-id="f2e05-131">approvalstate</span><span class="sxs-lookup"><span data-stu-id="f2e05-131">approvalState</span></span>|<span data-ttu-id="f2e05-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2e05-132">string</span></span>| <span data-ttu-id="f2e05-133">Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="f2e05-133">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="f2e05-134">approvaltype</span><span class="sxs-lookup"><span data-stu-id="f2e05-134">approvalType</span></span>|<span data-ttu-id="f2e05-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2e05-135">String</span></span>||
|<span data-ttu-id="f2e05-136">approverReason</span><span class="sxs-lookup"><span data-stu-id="f2e05-136">approverReason</span></span>|<span data-ttu-id="f2e05-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2e05-137">String</span></span>||
|<span data-ttu-id="f2e05-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f2e05-138">endDateTime</span></span>|<span data-ttu-id="f2e05-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2e05-139">DateTimeOffset</span></span>|<span data-ttu-id="f2e05-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f2e05-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f2e05-142">id</span><span class="sxs-lookup"><span data-stu-id="f2e05-142">id</span></span>|<span data-ttu-id="f2e05-143">String</span><span class="sxs-lookup"><span data-stu-id="f2e05-143">String</span></span>| <span data-ttu-id="f2e05-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2e05-144">Read-only.</span></span>|
|<span data-ttu-id="f2e05-145">requestorReason</span><span class="sxs-lookup"><span data-stu-id="f2e05-145">requestorReason</span></span>|<span data-ttu-id="f2e05-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2e05-146">String</span></span>||
|<span data-ttu-id="f2e05-147">roleId</span><span class="sxs-lookup"><span data-stu-id="f2e05-147">roleId</span></span>|<span data-ttu-id="f2e05-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2e05-148">String</span></span>||
|<span data-ttu-id="f2e05-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f2e05-149">startDateTime</span></span>|<span data-ttu-id="f2e05-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2e05-150">DateTimeOffset</span></span>|<span data-ttu-id="f2e05-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f2e05-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f2e05-153">userId</span><span class="sxs-lookup"><span data-stu-id="f2e05-153">userId</span></span>|<span data-ttu-id="f2e05-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2e05-154">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="f2e05-155">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="f2e05-155">Relationships</span></span>
| <span data-ttu-id="f2e05-156">Relação</span><span class="sxs-lookup"><span data-stu-id="f2e05-156">Relationship</span></span> | <span data-ttu-id="f2e05-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2e05-157">Type</span></span>   |<span data-ttu-id="f2e05-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2e05-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2e05-159">roleInfo</span><span class="sxs-lookup"><span data-stu-id="f2e05-159">roleInfo</span></span>|[<span data-ttu-id="f2e05-160">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="f2e05-160">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="f2e05-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2e05-161">Read-only.</span></span> <span data-ttu-id="f2e05-162">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f2e05-162">Nullable.</span></span>|
|<span data-ttu-id="f2e05-163">pedir</span><span class="sxs-lookup"><span data-stu-id="f2e05-163">request</span></span>|[<span data-ttu-id="f2e05-164">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f2e05-164">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="f2e05-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2e05-165">Read-only.</span></span> <span data-ttu-id="f2e05-166">A solicitação de atribuição de função para este objeto de aprovação</span><span class="sxs-lookup"><span data-stu-id="f2e05-166">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2e05-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2e05-167">JSON representation</span></span>
<span data-ttu-id="f2e05-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2e05-168">Here is a JSON representation of the resource.</span></span>

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


