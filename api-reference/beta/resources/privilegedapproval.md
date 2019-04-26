---
title: tipo de recurso privilegedApproval
description: Representa uma aprovação solicitada no gerenciamento de identidade privilegiado para obter uma função.
localization_priority: Normal
ms.openlocfilehash: 754fcd9b61321db1675408172c945557e38dc0e0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344212"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="64cab-103">tipo de recurso privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="64cab-103">privilegedApproval resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64cab-104">Representa uma aprovação solicitada no gerenciamento de identidade privilegiado para obter uma função.</span><span class="sxs-lookup"><span data-stu-id="64cab-104">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="64cab-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="64cab-105">Methods</span></span>

| <span data-ttu-id="64cab-106">Método</span><span class="sxs-lookup"><span data-stu-id="64cab-106">Method</span></span>           | <span data-ttu-id="64cab-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="64cab-107">Return Type</span></span>    |<span data-ttu-id="64cab-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="64cab-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="64cab-109">Get privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="64cab-109">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="64cab-110">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="64cab-110">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="64cab-111">Leia as propriedades e os relacionamentos do objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="64cab-111">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="64cab-112">Listar objetos privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="64cab-112">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="64cab-113">[privilegedApproval](privilegedapproval.md) collection</span><span class="sxs-lookup"><span data-stu-id="64cab-113">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="64cab-114">Obtenha a coleção de privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="64cab-114">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="64cab-115">Create privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="64cab-115">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="64cab-116">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="64cab-116">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="64cab-117">Crie um objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="64cab-117">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="64cab-118">Update privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="64cab-118">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="64cab-119">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="64cab-119">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="64cab-120">Atualize um objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="64cab-120">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="64cab-121">Myrequests</span><span class="sxs-lookup"><span data-stu-id="64cab-121">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="64cab-122">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="64cab-122">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="64cab-123">Receba solicitações de aprovação do solicitante.</span><span class="sxs-lookup"><span data-stu-id="64cab-123">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="64cab-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64cab-124">Properties</span></span>
| <span data-ttu-id="64cab-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64cab-125">Property</span></span>     | <span data-ttu-id="64cab-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="64cab-126">Type</span></span>   |<span data-ttu-id="64cab-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="64cab-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64cab-128">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="64cab-128">approvalDuration</span></span>|<span data-ttu-id="64cab-129">Duração</span><span class="sxs-lookup"><span data-stu-id="64cab-129">Duration</span></span>||
|<span data-ttu-id="64cab-130">approvalstate</span><span class="sxs-lookup"><span data-stu-id="64cab-130">approvalState</span></span>|<span data-ttu-id="64cab-131">string</span><span class="sxs-lookup"><span data-stu-id="64cab-131">string</span></span>| <span data-ttu-id="64cab-132">Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="64cab-132">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="64cab-133">approvaltype</span><span class="sxs-lookup"><span data-stu-id="64cab-133">approvalType</span></span>|<span data-ttu-id="64cab-134">String</span><span class="sxs-lookup"><span data-stu-id="64cab-134">String</span></span>||
|<span data-ttu-id="64cab-135">approverReason</span><span class="sxs-lookup"><span data-stu-id="64cab-135">approverReason</span></span>|<span data-ttu-id="64cab-136">String</span><span class="sxs-lookup"><span data-stu-id="64cab-136">String</span></span>||
|<span data-ttu-id="64cab-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="64cab-137">endDateTime</span></span>|<span data-ttu-id="64cab-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64cab-138">DateTimeOffset</span></span>|<span data-ttu-id="64cab-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="64cab-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="64cab-141">id</span><span class="sxs-lookup"><span data-stu-id="64cab-141">id</span></span>|<span data-ttu-id="64cab-142">String</span><span class="sxs-lookup"><span data-stu-id="64cab-142">String</span></span>| <span data-ttu-id="64cab-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64cab-143">Read-only.</span></span>|
|<span data-ttu-id="64cab-144">requestorReason</span><span class="sxs-lookup"><span data-stu-id="64cab-144">requestorReason</span></span>|<span data-ttu-id="64cab-145">String</span><span class="sxs-lookup"><span data-stu-id="64cab-145">String</span></span>||
|<span data-ttu-id="64cab-146">roleId</span><span class="sxs-lookup"><span data-stu-id="64cab-146">roleId</span></span>|<span data-ttu-id="64cab-147">String</span><span class="sxs-lookup"><span data-stu-id="64cab-147">String</span></span>||
|<span data-ttu-id="64cab-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="64cab-148">startDateTime</span></span>|<span data-ttu-id="64cab-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64cab-149">DateTimeOffset</span></span>|<span data-ttu-id="64cab-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="64cab-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="64cab-152">userId</span><span class="sxs-lookup"><span data-stu-id="64cab-152">userId</span></span>|<span data-ttu-id="64cab-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64cab-153">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="64cab-154">Relações</span><span class="sxs-lookup"><span data-stu-id="64cab-154">Relationships</span></span>
| <span data-ttu-id="64cab-155">Relação</span><span class="sxs-lookup"><span data-stu-id="64cab-155">Relationship</span></span> | <span data-ttu-id="64cab-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="64cab-156">Type</span></span>   |<span data-ttu-id="64cab-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="64cab-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64cab-158">roleInfo</span><span class="sxs-lookup"><span data-stu-id="64cab-158">roleInfo</span></span>|[<span data-ttu-id="64cab-159">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="64cab-159">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="64cab-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64cab-160">Read-only.</span></span> <span data-ttu-id="64cab-161">Anulável.</span><span class="sxs-lookup"><span data-stu-id="64cab-161">Nullable.</span></span>|
|<span data-ttu-id="64cab-162">pedir</span><span class="sxs-lookup"><span data-stu-id="64cab-162">request</span></span>|[<span data-ttu-id="64cab-163">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="64cab-163">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="64cab-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64cab-164">Read-only.</span></span> <span data-ttu-id="64cab-165">A solicitação de atribuição de função para este objeto de aprovação</span><span class="sxs-lookup"><span data-stu-id="64cab-165">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64cab-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64cab-166">JSON representation</span></span>
<span data-ttu-id="64cab-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64cab-167">Here is a JSON representation of the resource.</span></span>

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
