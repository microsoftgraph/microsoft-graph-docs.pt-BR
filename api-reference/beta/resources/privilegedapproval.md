---
title: tipo de recurso privilegedApproval
description: Representa uma aprovação solicitada no gerenciamento de identidade privilegiado para obter uma função.
localization_priority: Normal
ms.openlocfilehash: 283236d945e9a71a4ae0461bbefe66260efa88a4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563623"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="9d15e-103">tipo de recurso privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="9d15e-103">privilegedApproval resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d15e-104">Representa uma aprovação solicitada no gerenciamento de identidade privilegiado para obter uma função.</span><span class="sxs-lookup"><span data-stu-id="9d15e-104">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="9d15e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="9d15e-105">Methods</span></span>

| <span data-ttu-id="9d15e-106">Método</span><span class="sxs-lookup"><span data-stu-id="9d15e-106">Method</span></span>           | <span data-ttu-id="9d15e-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9d15e-107">Return Type</span></span>    |<span data-ttu-id="9d15e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d15e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9d15e-109">Get privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="9d15e-109">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="9d15e-110">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="9d15e-110">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="9d15e-111">Leia as propriedades e os relacionamentos do objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="9d15e-111">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="9d15e-112">Listar objetos privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="9d15e-112">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="9d15e-113">[privilegedApproval](privilegedapproval.md) collection</span><span class="sxs-lookup"><span data-stu-id="9d15e-113">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="9d15e-114">Obtenha a coleção de privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="9d15e-114">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="9d15e-115">Create privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="9d15e-115">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="9d15e-116">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="9d15e-116">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="9d15e-117">Crie um objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="9d15e-117">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="9d15e-118">Update privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="9d15e-118">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="9d15e-119">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="9d15e-119">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="9d15e-120">Atualize um objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="9d15e-120">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="9d15e-121">Myrequests</span><span class="sxs-lookup"><span data-stu-id="9d15e-121">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="9d15e-122">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="9d15e-122">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="9d15e-123">Receba solicitações de aprovação do solicitante.</span><span class="sxs-lookup"><span data-stu-id="9d15e-123">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="9d15e-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d15e-124">Properties</span></span>
| <span data-ttu-id="9d15e-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d15e-125">Property</span></span>     | <span data-ttu-id="9d15e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d15e-126">Type</span></span>   |<span data-ttu-id="9d15e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d15e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d15e-128">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="9d15e-128">approvalDuration</span></span>|<span data-ttu-id="9d15e-129">Duração</span><span class="sxs-lookup"><span data-stu-id="9d15e-129">Duration</span></span>||
|<span data-ttu-id="9d15e-130">approvalstate</span><span class="sxs-lookup"><span data-stu-id="9d15e-130">approvalState</span></span>|<span data-ttu-id="9d15e-131">string</span><span class="sxs-lookup"><span data-stu-id="9d15e-131">string</span></span>| <span data-ttu-id="9d15e-132">Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="9d15e-132">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="9d15e-133">approvaltype</span><span class="sxs-lookup"><span data-stu-id="9d15e-133">approvalType</span></span>|<span data-ttu-id="9d15e-134">String</span><span class="sxs-lookup"><span data-stu-id="9d15e-134">String</span></span>||
|<span data-ttu-id="9d15e-135">approverReason</span><span class="sxs-lookup"><span data-stu-id="9d15e-135">approverReason</span></span>|<span data-ttu-id="9d15e-136">String</span><span class="sxs-lookup"><span data-stu-id="9d15e-136">String</span></span>||
|<span data-ttu-id="9d15e-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9d15e-137">endDateTime</span></span>|<span data-ttu-id="9d15e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d15e-138">DateTimeOffset</span></span>|<span data-ttu-id="9d15e-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9d15e-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9d15e-141">id</span><span class="sxs-lookup"><span data-stu-id="9d15e-141">id</span></span>|<span data-ttu-id="9d15e-142">String</span><span class="sxs-lookup"><span data-stu-id="9d15e-142">String</span></span>| <span data-ttu-id="9d15e-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9d15e-143">Read-only.</span></span>|
|<span data-ttu-id="9d15e-144">requestorReason</span><span class="sxs-lookup"><span data-stu-id="9d15e-144">requestorReason</span></span>|<span data-ttu-id="9d15e-145">String</span><span class="sxs-lookup"><span data-stu-id="9d15e-145">String</span></span>||
|<span data-ttu-id="9d15e-146">roleId</span><span class="sxs-lookup"><span data-stu-id="9d15e-146">roleId</span></span>|<span data-ttu-id="9d15e-147">String</span><span class="sxs-lookup"><span data-stu-id="9d15e-147">String</span></span>||
|<span data-ttu-id="9d15e-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9d15e-148">startDateTime</span></span>|<span data-ttu-id="9d15e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d15e-149">DateTimeOffset</span></span>|<span data-ttu-id="9d15e-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9d15e-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9d15e-152">userId</span><span class="sxs-lookup"><span data-stu-id="9d15e-152">userId</span></span>|<span data-ttu-id="9d15e-153">String</span><span class="sxs-lookup"><span data-stu-id="9d15e-153">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="9d15e-154">Relações</span><span class="sxs-lookup"><span data-stu-id="9d15e-154">Relationships</span></span>
| <span data-ttu-id="9d15e-155">Relação</span><span class="sxs-lookup"><span data-stu-id="9d15e-155">Relationship</span></span> | <span data-ttu-id="9d15e-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d15e-156">Type</span></span>   |<span data-ttu-id="9d15e-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d15e-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d15e-158">roleInfo</span><span class="sxs-lookup"><span data-stu-id="9d15e-158">roleInfo</span></span>|[<span data-ttu-id="9d15e-159">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="9d15e-159">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="9d15e-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9d15e-160">Read-only.</span></span> <span data-ttu-id="9d15e-161">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9d15e-161">Nullable.</span></span>|
|<span data-ttu-id="9d15e-162">pedir</span><span class="sxs-lookup"><span data-stu-id="9d15e-162">request</span></span>|[<span data-ttu-id="9d15e-163">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9d15e-163">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="9d15e-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9d15e-164">Read-only.</span></span> <span data-ttu-id="9d15e-165">A solicitação de atribuição de função para este objeto de aprovação</span><span class="sxs-lookup"><span data-stu-id="9d15e-165">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d15e-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d15e-166">JSON representation</span></span>
<span data-ttu-id="9d15e-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d15e-167">Here is a JSON representation of the resource.</span></span>

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
