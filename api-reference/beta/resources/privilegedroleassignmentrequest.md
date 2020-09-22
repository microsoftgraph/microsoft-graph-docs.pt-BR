---
title: tipo de recurso privilegedRoleAssignmentRequest
description: Representa a solicitação de operações de atribuição de função no gerenciamento de identidade do Privilegd.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 5daeeee6f784c31f1e15843a8a1903ca41565118
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070506"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="d5b8e-103">tipo de recurso privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="d5b8e-103">privilegedRoleAssignmentRequest resource type</span></span>

<span data-ttu-id="d5b8e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5b8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5b8e-105">Representa a solicitação de operações de atribuição de função no gerenciamento de identidade do Privilegd.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-105">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="d5b8e-106">`privilegedRoleAssignmentRequest` é uma entidade com modelo de tíquete usada para gerenciar o ciclo de vida das atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-106">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="d5b8e-107">Ele representa a intenção/decisão dos usuários e administradores, e também fornece a flexibilidade para permitir a implementação de Schduling recorrentes, Gates de aprovação e assim por diante, em comparação com a exposição e operações diretas, `POST` `LIST` bem como `MY` e `Cancel` funções `governanceRoleAssignment` .</span><span class="sxs-lookup"><span data-stu-id="d5b8e-107">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="d5b8e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d5b8e-108">Methods</span></span>

| <span data-ttu-id="d5b8e-109">Método</span><span class="sxs-lookup"><span data-stu-id="d5b8e-109">Method</span></span>       | <span data-ttu-id="d5b8e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d5b8e-110">Return Type</span></span> | <span data-ttu-id="d5b8e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5b8e-111">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="d5b8e-112">List</span><span class="sxs-lookup"><span data-stu-id="d5b8e-112">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="d5b8e-113">coleção [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="d5b8e-113">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="d5b8e-114">Listar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-114">List role assignment requests.</span></span>|
|[<span data-ttu-id="d5b8e-115">Create</span><span class="sxs-lookup"><span data-stu-id="d5b8e-115">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="d5b8e-116">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="d5b8e-116">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="d5b8e-117">Criar uma solicitação para gerenciar o ciclo de vida da atribuição de função nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-117">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="d5b8e-118">Cancel</span><span class="sxs-lookup"><span data-stu-id="d5b8e-118">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="d5b8e-119">Cancelar uma solicitação de atribuição de função pendente.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-119">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="d5b8e-120">Pessoal</span><span class="sxs-lookup"><span data-stu-id="d5b8e-120">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="d5b8e-121">Obter solicitação de atribuição de função para o requstor atual.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-121">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5b8e-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5b8e-122">Properties</span></span>

| <span data-ttu-id="d5b8e-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5b8e-123">Property</span></span>     | <span data-ttu-id="d5b8e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5b8e-124">Type</span></span>        | <span data-ttu-id="d5b8e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5b8e-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d5b8e-126">id</span><span class="sxs-lookup"><span data-stu-id="d5b8e-126">id</span></span>|<span data-ttu-id="d5b8e-127">String</span><span class="sxs-lookup"><span data-stu-id="d5b8e-127">String</span></span>| <span data-ttu-id="d5b8e-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-128">Read-only.</span></span> <span data-ttu-id="d5b8e-129">A ID da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-129">The id of the role assignment request.</span></span>|
|<span data-ttu-id="d5b8e-130">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="d5b8e-130">assignmentState</span></span>|<span data-ttu-id="d5b8e-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5b8e-131">String</span></span>| <span data-ttu-id="d5b8e-132">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-132">The state of the assignment.</span></span> <span data-ttu-id="d5b8e-133">O valor pode ser `Eligible` para atribuição qualificada `Active` -se for diretamente atribuído `Active` por administradores ou ativado em uma atribuição qualificada pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-133">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="d5b8e-134">duration</span><span class="sxs-lookup"><span data-stu-id="d5b8e-134">duration</span></span>|<span data-ttu-id="d5b8e-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5b8e-135">String</span></span>| <span data-ttu-id="d5b8e-136">A duração de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-136">The duration of a role assignment.</span></span>|
|<span data-ttu-id="d5b8e-137">motivo</span><span class="sxs-lookup"><span data-stu-id="d5b8e-137">reason</span></span>|<span data-ttu-id="d5b8e-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5b8e-138">String</span></span>| <span data-ttu-id="d5b8e-139">O motivo da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-139">The reason for the role assignment.</span></span>|
|<span data-ttu-id="d5b8e-140">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5b8e-140">requestedDateTime</span></span>|<span data-ttu-id="d5b8e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5b8e-141">DateTimeOffset</span></span>| <span data-ttu-id="d5b8e-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-142">Read-only.</span></span> <span data-ttu-id="d5b8e-143">O tempo de criação da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-143">The request create time.</span></span> <span data-ttu-id="d5b8e-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d5b8e-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d5b8e-146">roleId</span><span class="sxs-lookup"><span data-stu-id="d5b8e-146">roleId</span></span>|<span data-ttu-id="d5b8e-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5b8e-147">String</span></span>| <span data-ttu-id="d5b8e-148">A ID da função.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-148">The id of the role.</span></span>|
|<span data-ttu-id="d5b8e-149">Cronograma</span><span class="sxs-lookup"><span data-stu-id="d5b8e-149">schedule</span></span>|[<span data-ttu-id="d5b8e-150">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="d5b8e-150">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="d5b8e-151">O objeto Schedule da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-151">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="d5b8e-152">status</span><span class="sxs-lookup"><span data-stu-id="d5b8e-152">status</span></span>|<span data-ttu-id="d5b8e-153">String</span><span class="sxs-lookup"><span data-stu-id="d5b8e-153">String</span></span>| <span data-ttu-id="d5b8e-154">Somente leitura. o status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-154">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="d5b8e-155">O valor pode ser,,,,,,,,, `NotStarted` `Completed` `RequestedApproval` `Scheduled` `Approved` `ApprovalDenied` `ApprovalAborted` `Cancelling` `Cancelled` `Revoked` `RequestExpired` .</span><span class="sxs-lookup"><span data-stu-id="d5b8e-155">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="d5b8e-156">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="d5b8e-156">ticketNumber</span></span>|<span data-ttu-id="d5b8e-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5b8e-157">String</span></span>| <span data-ttu-id="d5b8e-158">O ticketNumber da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-158">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="d5b8e-159">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="d5b8e-159">ticketSystem</span></span>|<span data-ttu-id="d5b8e-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5b8e-160">String</span></span>| <span data-ttu-id="d5b8e-161">O ticketSystem da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-161">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="d5b8e-162">tipo</span><span class="sxs-lookup"><span data-stu-id="d5b8e-162">type</span></span>|<span data-ttu-id="d5b8e-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5b8e-163">String</span></span>| <span data-ttu-id="d5b8e-164">Representando o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-164">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="d5b8e-165">O valor pode ser `AdminAdd` : os administradores adicionam usuários a funções; `UserAdd` : os usuários adicionam atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-165">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="d5b8e-166">userId</span><span class="sxs-lookup"><span data-stu-id="d5b8e-166">userId</span></span>|<span data-ttu-id="d5b8e-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5b8e-167">String</span></span>| <span data-ttu-id="d5b8e-168">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-168">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5b8e-169">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="d5b8e-169">Relationships</span></span>
| <span data-ttu-id="d5b8e-170">Relação</span><span class="sxs-lookup"><span data-stu-id="d5b8e-170">Relationship</span></span> | <span data-ttu-id="d5b8e-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5b8e-171">Type</span></span>        | <span data-ttu-id="d5b8e-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5b8e-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d5b8e-173">roleInfo</span><span class="sxs-lookup"><span data-stu-id="d5b8e-173">roleInfo</span></span>|[<span data-ttu-id="d5b8e-174">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="d5b8e-174">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="d5b8e-175">O objeto roleInfo da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-175">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5b8e-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5b8e-176">JSON representation</span></span>

<span data-ttu-id="d5b8e-177">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5b8e-177">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
}-->

```json
{
  "assignmentState": "String",
  "duration": "String",
  "id": "String (identifier)",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "roleId": "String",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": "String",
  "ticketNumber": "String",
  "ticketSystem": "String",
  "type": "String",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


