---
title: tipo de recurso de privilegedApproval
description: Representa uma aprovação solicitada no gerenciamento de identidades privilegiado para entrar em uma função.
localization_priority: Normal
ms.openlocfilehash: 283236d945e9a71a4ae0461bbefe66260efa88a4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516886"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="ff0a8-103">tipo de recurso de privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="ff0a8-103">privilegedApproval resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff0a8-104">Representa uma aprovação solicitada no gerenciamento de identidades privilegiado para entrar em uma função.</span><span class="sxs-lookup"><span data-stu-id="ff0a8-104">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="ff0a8-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ff0a8-105">Methods</span></span>

| <span data-ttu-id="ff0a8-106">Método</span><span class="sxs-lookup"><span data-stu-id="ff0a8-106">Method</span></span>           | <span data-ttu-id="ff0a8-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ff0a8-107">Return Type</span></span>    |<span data-ttu-id="ff0a8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff0a8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff0a8-109">Obter privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="ff0a8-109">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="ff0a8-110">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="ff0a8-110">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="ff0a8-111">Leia as propriedades e os relacionamentos do objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="ff0a8-111">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="ff0a8-112">Objetos de privilegedApproval List</span><span class="sxs-lookup"><span data-stu-id="ff0a8-112">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="ff0a8-113">coleção [privilegedApproval](privilegedapproval.md)</span><span class="sxs-lookup"><span data-stu-id="ff0a8-113">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="ff0a8-114">Obtenha a coleção de privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="ff0a8-114">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="ff0a8-115">Criar privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="ff0a8-115">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="ff0a8-116">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="ff0a8-116">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="ff0a8-117">Crie objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="ff0a8-117">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="ff0a8-118">Atualizar privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="ff0a8-118">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="ff0a8-119">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="ff0a8-119">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="ff0a8-120">Atualize o objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="ff0a8-120">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="ff0a8-121">Myrequests</span><span class="sxs-lookup"><span data-stu-id="ff0a8-121">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="ff0a8-122">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="ff0a8-122">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="ff0a8-123">Obtenha as solicitações de aprovação do solicitador.</span><span class="sxs-lookup"><span data-stu-id="ff0a8-123">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff0a8-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff0a8-124">Properties</span></span>
| <span data-ttu-id="ff0a8-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff0a8-125">Property</span></span>     | <span data-ttu-id="ff0a8-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff0a8-126">Type</span></span>   |<span data-ttu-id="ff0a8-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff0a8-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff0a8-128">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="ff0a8-128">approvalDuration</span></span>|<span data-ttu-id="ff0a8-129">Duration</span><span class="sxs-lookup"><span data-stu-id="ff0a8-129">Duration</span></span>||
|<span data-ttu-id="ff0a8-130">approvalState</span><span class="sxs-lookup"><span data-stu-id="ff0a8-130">approvalState</span></span>|<span data-ttu-id="ff0a8-131">string</span><span class="sxs-lookup"><span data-stu-id="ff0a8-131">string</span></span>| <span data-ttu-id="ff0a8-132">Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="ff0a8-132">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="ff0a8-133">approvalType</span><span class="sxs-lookup"><span data-stu-id="ff0a8-133">approvalType</span></span>|<span data-ttu-id="ff0a8-134">String</span><span class="sxs-lookup"><span data-stu-id="ff0a8-134">String</span></span>||
|<span data-ttu-id="ff0a8-135">approverReason</span><span class="sxs-lookup"><span data-stu-id="ff0a8-135">approverReason</span></span>|<span data-ttu-id="ff0a8-136">String</span><span class="sxs-lookup"><span data-stu-id="ff0a8-136">String</span></span>||
|<span data-ttu-id="ff0a8-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ff0a8-137">endDateTime</span></span>|<span data-ttu-id="ff0a8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff0a8-138">DateTimeOffset</span></span>|<span data-ttu-id="ff0a8-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ff0a8-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ff0a8-141">id</span><span class="sxs-lookup"><span data-stu-id="ff0a8-141">id</span></span>|<span data-ttu-id="ff0a8-142">String</span><span class="sxs-lookup"><span data-stu-id="ff0a8-142">String</span></span>| <span data-ttu-id="ff0a8-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff0a8-143">Read-only.</span></span>|
|<span data-ttu-id="ff0a8-144">requestorReason</span><span class="sxs-lookup"><span data-stu-id="ff0a8-144">requestorReason</span></span>|<span data-ttu-id="ff0a8-145">String</span><span class="sxs-lookup"><span data-stu-id="ff0a8-145">String</span></span>||
|<span data-ttu-id="ff0a8-146">roleId</span><span class="sxs-lookup"><span data-stu-id="ff0a8-146">roleId</span></span>|<span data-ttu-id="ff0a8-147">String</span><span class="sxs-lookup"><span data-stu-id="ff0a8-147">String</span></span>||
|<span data-ttu-id="ff0a8-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ff0a8-148">startDateTime</span></span>|<span data-ttu-id="ff0a8-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff0a8-149">DateTimeOffset</span></span>|<span data-ttu-id="ff0a8-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ff0a8-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ff0a8-152">userId</span><span class="sxs-lookup"><span data-stu-id="ff0a8-152">userId</span></span>|<span data-ttu-id="ff0a8-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff0a8-153">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="ff0a8-154">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="ff0a8-154">Relationships</span></span>
| <span data-ttu-id="ff0a8-155">Relação</span><span class="sxs-lookup"><span data-stu-id="ff0a8-155">Relationship</span></span> | <span data-ttu-id="ff0a8-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff0a8-156">Type</span></span>   |<span data-ttu-id="ff0a8-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff0a8-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff0a8-158">roleInfo</span><span class="sxs-lookup"><span data-stu-id="ff0a8-158">roleInfo</span></span>|[<span data-ttu-id="ff0a8-159">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="ff0a8-159">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="ff0a8-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ff0a8-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="ff0a8-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff0a8-162">request</span></span>|[<span data-ttu-id="ff0a8-163">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="ff0a8-163">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="ff0a8-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff0a8-164">Read-only.</span></span> <span data-ttu-id="ff0a8-165">A solicitação de atribuição de função para este objeto de aprovação</span><span class="sxs-lookup"><span data-stu-id="ff0a8-165">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff0a8-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff0a8-166">JSON representation</span></span>
<span data-ttu-id="ff0a8-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff0a8-167">Here is a JSON representation of the resource.</span></span>

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
