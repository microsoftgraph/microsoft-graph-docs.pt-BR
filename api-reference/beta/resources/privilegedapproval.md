---
title: tipo de recurso privilegedApproval
description: Representa uma aprovação solicitada no gerenciamento de identidade privilegiado para obter uma função.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: c4148e5740c9b31368be336a615524ced426a560
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219225"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="135a0-103">tipo de recurso privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="135a0-103">privilegedApproval resource type</span></span>

<span data-ttu-id="135a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="135a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="135a0-105">Representa uma aprovação solicitada no gerenciamento de identidade privilegiado para obter uma função.</span><span class="sxs-lookup"><span data-stu-id="135a0-105">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="135a0-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="135a0-106">Methods</span></span>

| <span data-ttu-id="135a0-107">Método</span><span class="sxs-lookup"><span data-stu-id="135a0-107">Method</span></span>           | <span data-ttu-id="135a0-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="135a0-108">Return Type</span></span>    |<span data-ttu-id="135a0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="135a0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="135a0-110">Get privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="135a0-110">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="135a0-111">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="135a0-111">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="135a0-112">Leia as propriedades e os relacionamentos do objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="135a0-112">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="135a0-113">Listar objetos privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="135a0-113">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="135a0-114">[privilegedApproval](privilegedapproval.md) collection</span><span class="sxs-lookup"><span data-stu-id="135a0-114">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="135a0-115">Obtenha a coleção de privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="135a0-115">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="135a0-116">Create privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="135a0-116">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="135a0-117">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="135a0-117">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="135a0-118">Crie um objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="135a0-118">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="135a0-119">Update privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="135a0-119">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="135a0-120">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="135a0-120">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="135a0-121">Atualize um objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="135a0-121">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="135a0-122">Myrequests</span><span class="sxs-lookup"><span data-stu-id="135a0-122">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="135a0-123">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="135a0-123">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="135a0-124">Receba solicitações de aprovação do solicitante.</span><span class="sxs-lookup"><span data-stu-id="135a0-124">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="135a0-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="135a0-125">Properties</span></span>
| <span data-ttu-id="135a0-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="135a0-126">Property</span></span>     | <span data-ttu-id="135a0-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="135a0-127">Type</span></span>   |<span data-ttu-id="135a0-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="135a0-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="135a0-129">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="135a0-129">approvalDuration</span></span>|<span data-ttu-id="135a0-130">Duração</span><span class="sxs-lookup"><span data-stu-id="135a0-130">Duration</span></span>||
|<span data-ttu-id="135a0-131">approvalstate</span><span class="sxs-lookup"><span data-stu-id="135a0-131">approvalState</span></span>|<span data-ttu-id="135a0-132">string</span><span class="sxs-lookup"><span data-stu-id="135a0-132">string</span></span>| <span data-ttu-id="135a0-133">Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="135a0-133">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="135a0-134">approvaltype</span><span class="sxs-lookup"><span data-stu-id="135a0-134">approvalType</span></span>|<span data-ttu-id="135a0-135">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="135a0-135">String</span></span>||
|<span data-ttu-id="135a0-136">approverReason</span><span class="sxs-lookup"><span data-stu-id="135a0-136">approverReason</span></span>|<span data-ttu-id="135a0-137">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="135a0-137">String</span></span>||
|<span data-ttu-id="135a0-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="135a0-138">endDateTime</span></span>|<span data-ttu-id="135a0-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="135a0-139">DateTimeOffset</span></span>|<span data-ttu-id="135a0-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="135a0-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="135a0-142">id</span><span class="sxs-lookup"><span data-stu-id="135a0-142">id</span></span>|<span data-ttu-id="135a0-143">String</span><span class="sxs-lookup"><span data-stu-id="135a0-143">String</span></span>| <span data-ttu-id="135a0-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="135a0-144">Read-only.</span></span>|
|<span data-ttu-id="135a0-145">requestorReason</span><span class="sxs-lookup"><span data-stu-id="135a0-145">requestorReason</span></span>|<span data-ttu-id="135a0-146">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="135a0-146">String</span></span>||
|<span data-ttu-id="135a0-147">roleId</span><span class="sxs-lookup"><span data-stu-id="135a0-147">roleId</span></span>|<span data-ttu-id="135a0-148">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="135a0-148">String</span></span>||
|<span data-ttu-id="135a0-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="135a0-149">startDateTime</span></span>|<span data-ttu-id="135a0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="135a0-150">DateTimeOffset</span></span>|<span data-ttu-id="135a0-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="135a0-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="135a0-153">userId</span><span class="sxs-lookup"><span data-stu-id="135a0-153">userId</span></span>|<span data-ttu-id="135a0-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="135a0-154">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="135a0-155">Relações</span><span class="sxs-lookup"><span data-stu-id="135a0-155">Relationships</span></span>
| <span data-ttu-id="135a0-156">Relação</span><span class="sxs-lookup"><span data-stu-id="135a0-156">Relationship</span></span> | <span data-ttu-id="135a0-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="135a0-157">Type</span></span>   |<span data-ttu-id="135a0-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="135a0-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="135a0-159">roleInfo</span><span class="sxs-lookup"><span data-stu-id="135a0-159">roleInfo</span></span>|[<span data-ttu-id="135a0-160">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="135a0-160">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="135a0-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="135a0-161">Read-only.</span></span> <span data-ttu-id="135a0-162">Anulável.</span><span class="sxs-lookup"><span data-stu-id="135a0-162">Nullable.</span></span>|
|<span data-ttu-id="135a0-163">pedir</span><span class="sxs-lookup"><span data-stu-id="135a0-163">request</span></span>|[<span data-ttu-id="135a0-164">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="135a0-164">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="135a0-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="135a0-165">Read-only.</span></span> <span data-ttu-id="135a0-166">A solicitação de atribuição de função para este objeto de aprovação</span><span class="sxs-lookup"><span data-stu-id="135a0-166">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="135a0-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="135a0-167">JSON representation</span></span>
<span data-ttu-id="135a0-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="135a0-168">Here is a JSON representation of the resource.</span></span>

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
