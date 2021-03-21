---
title: Tipo de recurso privilegedApproval
description: Representa uma aprovação solicitada no Privileged Identity Management para entrar em uma função.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8d092d6c877f9fa2bdce2d645ef56a84508c510d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962585"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="d8353-103">Tipo de recurso privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8353-103">privilegedApproval resource type</span></span>

<span data-ttu-id="d8353-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8353-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8353-105">Representa uma aprovação solicitada no Privileged Identity Management para entrar em uma função.</span><span class="sxs-lookup"><span data-stu-id="d8353-105">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="d8353-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="d8353-106">Methods</span></span>

| <span data-ttu-id="d8353-107">Método</span><span class="sxs-lookup"><span data-stu-id="d8353-107">Method</span></span>           | <span data-ttu-id="d8353-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d8353-108">Return Type</span></span>    |<span data-ttu-id="d8353-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8353-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8353-110">Get privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8353-110">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="d8353-111">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8353-111">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="d8353-112">Ler propriedades e relações do objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="d8353-112">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="d8353-113">Listar objetos privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8353-113">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="d8353-114">[privilegedApproval](privilegedapproval.md) collection</span><span class="sxs-lookup"><span data-stu-id="d8353-114">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="d8353-115">Obter a coleção privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="d8353-115">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="d8353-116">Create privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8353-116">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="d8353-117">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8353-117">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="d8353-118">Crie um objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="d8353-118">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="d8353-119">Update privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8353-119">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="d8353-120">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8353-120">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="d8353-121">Atualize um objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="d8353-121">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="d8353-122">Myrequests</span><span class="sxs-lookup"><span data-stu-id="d8353-122">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="d8353-123">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8353-123">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="d8353-124">Receba solicitações de aprovação do solicitante.</span><span class="sxs-lookup"><span data-stu-id="d8353-124">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8353-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8353-125">Properties</span></span>
| <span data-ttu-id="d8353-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8353-126">Property</span></span>     | <span data-ttu-id="d8353-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8353-127">Type</span></span>   |<span data-ttu-id="d8353-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8353-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8353-129">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="d8353-129">approvalDuration</span></span>|<span data-ttu-id="d8353-130">Duration</span><span class="sxs-lookup"><span data-stu-id="d8353-130">Duration</span></span>||
|<span data-ttu-id="d8353-131">approvalState</span><span class="sxs-lookup"><span data-stu-id="d8353-131">approvalState</span></span>|<span data-ttu-id="d8353-132">approvalState</span><span class="sxs-lookup"><span data-stu-id="d8353-132">approvalState</span></span>| <span data-ttu-id="d8353-133">Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="d8353-133">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="d8353-134">approvalType</span><span class="sxs-lookup"><span data-stu-id="d8353-134">approvalType</span></span>|<span data-ttu-id="d8353-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8353-135">String</span></span>||
|<span data-ttu-id="d8353-136">approverReason</span><span class="sxs-lookup"><span data-stu-id="d8353-136">approverReason</span></span>|<span data-ttu-id="d8353-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8353-137">String</span></span>||
|<span data-ttu-id="d8353-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d8353-138">endDateTime</span></span>|<span data-ttu-id="d8353-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8353-139">DateTimeOffset</span></span>|<span data-ttu-id="d8353-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d8353-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d8353-141">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="d8353-141">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="d8353-142">id</span><span class="sxs-lookup"><span data-stu-id="d8353-142">id</span></span>|<span data-ttu-id="d8353-143">String</span><span class="sxs-lookup"><span data-stu-id="d8353-143">String</span></span>| <span data-ttu-id="d8353-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8353-144">Read-only.</span></span>|
|<span data-ttu-id="d8353-145">requestorReason</span><span class="sxs-lookup"><span data-stu-id="d8353-145">requestorReason</span></span>|<span data-ttu-id="d8353-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8353-146">String</span></span>||
|<span data-ttu-id="d8353-147">roleId</span><span class="sxs-lookup"><span data-stu-id="d8353-147">roleId</span></span>|<span data-ttu-id="d8353-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8353-148">String</span></span>||
|<span data-ttu-id="d8353-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d8353-149">startDateTime</span></span>|<span data-ttu-id="d8353-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8353-150">DateTimeOffset</span></span>|<span data-ttu-id="d8353-151">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d8353-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d8353-152">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="d8353-152">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="d8353-153">userId</span><span class="sxs-lookup"><span data-stu-id="d8353-153">userId</span></span>|<span data-ttu-id="d8353-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8353-154">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="d8353-155">Relações</span><span class="sxs-lookup"><span data-stu-id="d8353-155">Relationships</span></span>
| <span data-ttu-id="d8353-156">Relação</span><span class="sxs-lookup"><span data-stu-id="d8353-156">Relationship</span></span> | <span data-ttu-id="d8353-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8353-157">Type</span></span>   |<span data-ttu-id="d8353-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8353-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8353-159">roleInfo</span><span class="sxs-lookup"><span data-stu-id="d8353-159">roleInfo</span></span>|[<span data-ttu-id="d8353-160">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="d8353-160">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="d8353-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8353-161">Read-only.</span></span> <span data-ttu-id="d8353-162">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d8353-162">Nullable.</span></span>|
|<span data-ttu-id="d8353-163">request</span><span class="sxs-lookup"><span data-stu-id="d8353-163">request</span></span>|[<span data-ttu-id="d8353-164">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="d8353-164">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="d8353-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8353-165">Read-only.</span></span> <span data-ttu-id="d8353-166">A solicitação de atribuição de função para este objeto de aprovação</span><span class="sxs-lookup"><span data-stu-id="d8353-166">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8353-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8353-167">JSON representation</span></span>
<span data-ttu-id="d8353-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8353-168">Here is a JSON representation of the resource.</span></span>

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


