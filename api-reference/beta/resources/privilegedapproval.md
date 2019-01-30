---
title: tipo de recurso de privilegedApproval
description: Representa uma aprovação solicitada no gerenciamento de identidades privilegiado para entrar em uma função.
localization_priority: Normal
ms.openlocfilehash: 283236d945e9a71a4ae0461bbefe66260efa88a4
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643871"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="6c3d2-103">tipo de recurso de privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="6c3d2-103">privilegedApproval resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c3d2-104">Representa uma aprovação solicitada no gerenciamento de identidades privilegiado para entrar em uma função.</span><span class="sxs-lookup"><span data-stu-id="6c3d2-104">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="6c3d2-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="6c3d2-105">Methods</span></span>

| <span data-ttu-id="6c3d2-106">Método</span><span class="sxs-lookup"><span data-stu-id="6c3d2-106">Method</span></span>           | <span data-ttu-id="6c3d2-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6c3d2-107">Return Type</span></span>    |<span data-ttu-id="6c3d2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c3d2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c3d2-109">Get privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="6c3d2-109">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="6c3d2-110">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="6c3d2-110">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="6c3d2-111">Leia as propriedades e os relacionamentos do objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="6c3d2-111">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="6c3d2-112">Objetos de privilegedApproval List</span><span class="sxs-lookup"><span data-stu-id="6c3d2-112">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="6c3d2-113">[privilegedApproval](privilegedapproval.md) collection</span><span class="sxs-lookup"><span data-stu-id="6c3d2-113">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="6c3d2-114">Obtenha a coleção de privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="6c3d2-114">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="6c3d2-115">Create privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="6c3d2-115">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="6c3d2-116">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="6c3d2-116">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="6c3d2-117">Crie um objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="6c3d2-117">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="6c3d2-118">Update privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="6c3d2-118">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="6c3d2-119">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="6c3d2-119">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="6c3d2-120">Atualize um objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="6c3d2-120">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="6c3d2-121">Myrequests</span><span class="sxs-lookup"><span data-stu-id="6c3d2-121">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="6c3d2-122">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="6c3d2-122">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="6c3d2-123">Receba solicitações de aprovação do solicitante.</span><span class="sxs-lookup"><span data-stu-id="6c3d2-123">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c3d2-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c3d2-124">Properties</span></span>
| <span data-ttu-id="6c3d2-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c3d2-125">Property</span></span>     | <span data-ttu-id="6c3d2-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c3d2-126">Type</span></span>   |<span data-ttu-id="6c3d2-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c3d2-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c3d2-128">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="6c3d2-128">approvalDuration</span></span>|<span data-ttu-id="6c3d2-129">Duration</span><span class="sxs-lookup"><span data-stu-id="6c3d2-129">Duration</span></span>||
|<span data-ttu-id="6c3d2-130">approvalState</span><span class="sxs-lookup"><span data-stu-id="6c3d2-130">approvalState</span></span>|<span data-ttu-id="6c3d2-131">string</span><span class="sxs-lookup"><span data-stu-id="6c3d2-131">string</span></span>| <span data-ttu-id="6c3d2-132">Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="6c3d2-132">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="6c3d2-133">approvalType</span><span class="sxs-lookup"><span data-stu-id="6c3d2-133">approvalType</span></span>|<span data-ttu-id="6c3d2-134">String</span><span class="sxs-lookup"><span data-stu-id="6c3d2-134">String</span></span>||
|<span data-ttu-id="6c3d2-135">approverReason</span><span class="sxs-lookup"><span data-stu-id="6c3d2-135">approverReason</span></span>|<span data-ttu-id="6c3d2-136">String</span><span class="sxs-lookup"><span data-stu-id="6c3d2-136">String</span></span>||
|<span data-ttu-id="6c3d2-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6c3d2-137">endDateTime</span></span>|<span data-ttu-id="6c3d2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c3d2-138">DateTimeOffset</span></span>|<span data-ttu-id="6c3d2-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6c3d2-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6c3d2-141">id</span><span class="sxs-lookup"><span data-stu-id="6c3d2-141">id</span></span>|<span data-ttu-id="6c3d2-142">String</span><span class="sxs-lookup"><span data-stu-id="6c3d2-142">String</span></span>| <span data-ttu-id="6c3d2-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6c3d2-143">Read-only.</span></span>|
|<span data-ttu-id="6c3d2-144">requestorReason</span><span class="sxs-lookup"><span data-stu-id="6c3d2-144">requestorReason</span></span>|<span data-ttu-id="6c3d2-145">String</span><span class="sxs-lookup"><span data-stu-id="6c3d2-145">String</span></span>||
|<span data-ttu-id="6c3d2-146">roleId</span><span class="sxs-lookup"><span data-stu-id="6c3d2-146">roleId</span></span>|<span data-ttu-id="6c3d2-147">String</span><span class="sxs-lookup"><span data-stu-id="6c3d2-147">String</span></span>||
|<span data-ttu-id="6c3d2-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6c3d2-148">startDateTime</span></span>|<span data-ttu-id="6c3d2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c3d2-149">DateTimeOffset</span></span>|<span data-ttu-id="6c3d2-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6c3d2-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6c3d2-152">userId</span><span class="sxs-lookup"><span data-stu-id="6c3d2-152">userId</span></span>|<span data-ttu-id="6c3d2-153">String</span><span class="sxs-lookup"><span data-stu-id="6c3d2-153">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="6c3d2-154">Relações</span><span class="sxs-lookup"><span data-stu-id="6c3d2-154">Relationships</span></span>
| <span data-ttu-id="6c3d2-155">Relação</span><span class="sxs-lookup"><span data-stu-id="6c3d2-155">Relationship</span></span> | <span data-ttu-id="6c3d2-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c3d2-156">Type</span></span>   |<span data-ttu-id="6c3d2-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c3d2-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c3d2-158">roleInfo</span><span class="sxs-lookup"><span data-stu-id="6c3d2-158">roleInfo</span></span>|[<span data-ttu-id="6c3d2-159">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="6c3d2-159">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="6c3d2-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="6c3d2-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="6c3d2-162">solicitação</span><span class="sxs-lookup"><span data-stu-id="6c3d2-162">request</span></span>|[<span data-ttu-id="6c3d2-163">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="6c3d2-163">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="6c3d2-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6c3d2-164">Read-only.</span></span> <span data-ttu-id="6c3d2-165">A solicitação de atribuição de função para este objeto de aprovação</span><span class="sxs-lookup"><span data-stu-id="6c3d2-165">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c3d2-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c3d2-166">JSON representation</span></span>
<span data-ttu-id="6c3d2-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c3d2-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedapproval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
