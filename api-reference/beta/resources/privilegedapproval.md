---
title: tipo de recurso de privilegedApproval
description: Representa uma aprovação solicitada no gerenciamento de identidades privilegiado para entrar em uma função.
localization_priority: Normal
ms.openlocfilehash: 03cdba4eee7b031645928b2f512288a18ba18bf8
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571014"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="0e7d7-103">tipo de recurso de privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="0e7d7-103">privilegedApproval resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e7d7-104">Representa uma aprovação solicitada no gerenciamento de identidades privilegiado para entrar em uma função.</span><span class="sxs-lookup"><span data-stu-id="0e7d7-104">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="0e7d7-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="0e7d7-105">Methods</span></span>

| <span data-ttu-id="0e7d7-106">Método</span><span class="sxs-lookup"><span data-stu-id="0e7d7-106">Method</span></span>           | <span data-ttu-id="0e7d7-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0e7d7-107">Return Type</span></span>    |<span data-ttu-id="0e7d7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e7d7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0e7d7-109">Obter privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="0e7d7-109">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="0e7d7-110">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="0e7d7-110">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="0e7d7-111">Leia as propriedades e os relacionamentos do objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="0e7d7-111">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="0e7d7-112">Objetos de privilegedApproval List</span><span class="sxs-lookup"><span data-stu-id="0e7d7-112">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="0e7d7-113">coleção [privilegedApproval](privilegedapproval.md)</span><span class="sxs-lookup"><span data-stu-id="0e7d7-113">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="0e7d7-114">Obtenha a coleção de privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="0e7d7-114">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="0e7d7-115">Criar privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="0e7d7-115">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="0e7d7-116">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="0e7d7-116">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="0e7d7-117">Crie objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="0e7d7-117">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="0e7d7-118">Atualizar privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="0e7d7-118">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="0e7d7-119">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="0e7d7-119">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="0e7d7-120">Atualize o objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="0e7d7-120">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="0e7d7-121">Myrequests</span><span class="sxs-lookup"><span data-stu-id="0e7d7-121">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="0e7d7-122">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="0e7d7-122">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="0e7d7-123">Obtenha as solicitações de aprovação do solicitador.</span><span class="sxs-lookup"><span data-stu-id="0e7d7-123">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e7d7-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e7d7-124">Properties</span></span>
| <span data-ttu-id="0e7d7-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e7d7-125">Property</span></span>     | <span data-ttu-id="0e7d7-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e7d7-126">Type</span></span>   |<span data-ttu-id="0e7d7-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e7d7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e7d7-128">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="0e7d7-128">approvalDuration</span></span>|<span data-ttu-id="0e7d7-129">Duration</span><span class="sxs-lookup"><span data-stu-id="0e7d7-129">Duration</span></span>||
|<span data-ttu-id="0e7d7-130">approvalState</span><span class="sxs-lookup"><span data-stu-id="0e7d7-130">approvalState</span></span>|<span data-ttu-id="0e7d7-131">string</span><span class="sxs-lookup"><span data-stu-id="0e7d7-131">string</span></span>| <span data-ttu-id="0e7d7-132">Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="0e7d7-132">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="0e7d7-133">approvalType</span><span class="sxs-lookup"><span data-stu-id="0e7d7-133">approvalType</span></span>|<span data-ttu-id="0e7d7-134">String</span><span class="sxs-lookup"><span data-stu-id="0e7d7-134">String</span></span>||
|<span data-ttu-id="0e7d7-135">approverReason</span><span class="sxs-lookup"><span data-stu-id="0e7d7-135">approverReason</span></span>|<span data-ttu-id="0e7d7-136">String</span><span class="sxs-lookup"><span data-stu-id="0e7d7-136">String</span></span>||
|<span data-ttu-id="0e7d7-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0e7d7-137">endDateTime</span></span>|<span data-ttu-id="0e7d7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e7d7-138">DateTimeOffset</span></span>|<span data-ttu-id="0e7d7-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0e7d7-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0e7d7-141">id</span><span class="sxs-lookup"><span data-stu-id="0e7d7-141">id</span></span>|<span data-ttu-id="0e7d7-142">String</span><span class="sxs-lookup"><span data-stu-id="0e7d7-142">String</span></span>| <span data-ttu-id="0e7d7-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e7d7-143">Read-only.</span></span>|
|<span data-ttu-id="0e7d7-144">requestorReason</span><span class="sxs-lookup"><span data-stu-id="0e7d7-144">requestorReason</span></span>|<span data-ttu-id="0e7d7-145">String</span><span class="sxs-lookup"><span data-stu-id="0e7d7-145">String</span></span>||
|<span data-ttu-id="0e7d7-146">roleId</span><span class="sxs-lookup"><span data-stu-id="0e7d7-146">roleId</span></span>|<span data-ttu-id="0e7d7-147">String</span><span class="sxs-lookup"><span data-stu-id="0e7d7-147">String</span></span>||
|<span data-ttu-id="0e7d7-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0e7d7-148">startDateTime</span></span>|<span data-ttu-id="0e7d7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e7d7-149">DateTimeOffset</span></span>|<span data-ttu-id="0e7d7-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0e7d7-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0e7d7-152">userId</span><span class="sxs-lookup"><span data-stu-id="0e7d7-152">userId</span></span>|<span data-ttu-id="0e7d7-153">String</span><span class="sxs-lookup"><span data-stu-id="0e7d7-153">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="0e7d7-154">Relações</span><span class="sxs-lookup"><span data-stu-id="0e7d7-154">Relationships</span></span>
| <span data-ttu-id="0e7d7-155">Relação</span><span class="sxs-lookup"><span data-stu-id="0e7d7-155">Relationship</span></span> | <span data-ttu-id="0e7d7-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e7d7-156">Type</span></span>   |<span data-ttu-id="0e7d7-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e7d7-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e7d7-158">roleInfo</span><span class="sxs-lookup"><span data-stu-id="0e7d7-158">roleInfo</span></span>| [<span data-ttu-id="0e7d7-159">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="0e7d7-159">privilegedRole</span></span>](privilegedrole.md) | <span data-ttu-id="0e7d7-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0e7d7-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="0e7d7-162">solicitação</span><span class="sxs-lookup"><span data-stu-id="0e7d7-162">request</span></span>| [<span data-ttu-id="0e7d7-163">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="0e7d7-163">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md) | <span data-ttu-id="0e7d7-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e7d7-164">Read-only.</span></span> <span data-ttu-id="0e7d7-165">A solicitação de atribuição de função para este objeto de aprovação</span><span class="sxs-lookup"><span data-stu-id="0e7d7-165">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e7d7-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e7d7-166">JSON representation</span></span>
<span data-ttu-id="0e7d7-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e7d7-167">Here is a JSON representation of the resource.</span></span>

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
