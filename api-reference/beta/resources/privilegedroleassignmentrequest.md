---
title: tipo de recurso de privilegedRoleAssignmentRequest
description: Representa a solicitação para operações de atribuição de função no gerenciamento de identidades Privilegd.
ms.openlocfilehash: b715c88157a7df52dabcb4c746dfe70bc2523d18
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039586"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="a806b-103">tipo de recurso de privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="a806b-103">privilegedRoleAssignmentRequest resource type</span></span>

> <span data-ttu-id="a806b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a806b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a806b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a806b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a806b-106">Representa a solicitação para operações de atribuição de função no gerenciamento de identidades Privilegd.</span><span class="sxs-lookup"><span data-stu-id="a806b-106">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="a806b-107">`privilegedRoleAssignmentRequest`uma entidade modelada de tíquete é usada para gerenciar o ciclo de vida de atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="a806b-107">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="a806b-108">Ele representa a intenção/decisão dos usuários e administradores e também oferece flexibilidade para permitir a implementação de schduling recorrente, entradas de aprovação e assim por diante, em relação ao diretamente expondo `POST` e `LIST` operações bem como `MY` e `Cancel` funciona em `governanceRoleAssignment`.</span><span class="sxs-lookup"><span data-stu-id="a806b-108">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="a806b-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="a806b-109">Methods</span></span>

| <span data-ttu-id="a806b-110">Método</span><span class="sxs-lookup"><span data-stu-id="a806b-110">Method</span></span>       | <span data-ttu-id="a806b-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a806b-111">Return Type</span></span> | <span data-ttu-id="a806b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a806b-112">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="a806b-113">List</span><span class="sxs-lookup"><span data-stu-id="a806b-113">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="a806b-114">coleção [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="a806b-114">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="a806b-115">Lista solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a806b-115">List role assignment requests.</span></span>|
|[<span data-ttu-id="a806b-116">Create</span><span class="sxs-lookup"><span data-stu-id="a806b-116">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="a806b-117">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="a806b-117">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="a806b-118">Crie uma solicitação para gerenciar o ciclo de vida de atribuição de função de novo ou existente.</span><span class="sxs-lookup"><span data-stu-id="a806b-118">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="a806b-119">Cancel</span><span class="sxs-lookup"><span data-stu-id="a806b-119">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="a806b-120">Cancele uma solicitação de atribuição de função pendente.</span><span class="sxs-lookup"><span data-stu-id="a806b-120">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="a806b-121">Minha</span><span class="sxs-lookup"><span data-stu-id="a806b-121">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="a806b-122">Obtenha a solicitação de atribuição de função para requstor atual.</span><span class="sxs-lookup"><span data-stu-id="a806b-122">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="a806b-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a806b-123">Properties</span></span>

| <span data-ttu-id="a806b-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a806b-124">Property</span></span>     | <span data-ttu-id="a806b-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="a806b-125">Type</span></span>        | <span data-ttu-id="a806b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="a806b-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a806b-127">id</span><span class="sxs-lookup"><span data-stu-id="a806b-127">id</span></span>|<span data-ttu-id="a806b-128">String</span><span class="sxs-lookup"><span data-stu-id="a806b-128">String</span></span>| <span data-ttu-id="a806b-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a806b-129">Read-only.</span></span> <span data-ttu-id="a806b-130">A identificação da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a806b-130">The id of the role assignment request.</span></span>|
|<span data-ttu-id="a806b-131">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a806b-131">assignmentState</span></span>|<span data-ttu-id="a806b-132">String</span><span class="sxs-lookup"><span data-stu-id="a806b-132">String</span></span>| <span data-ttu-id="a806b-133">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="a806b-133">The state of the assignment.</span></span> <span data-ttu-id="a806b-134">O valor pode ser `Eligible` para atribuição elegível `Active` - se ele é atribuído diretamente `Active` pelos administradores, ou ativado em uma atribuição elegível pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="a806b-134">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="a806b-135">duration</span><span class="sxs-lookup"><span data-stu-id="a806b-135">duration</span></span>|<span data-ttu-id="a806b-136">String</span><span class="sxs-lookup"><span data-stu-id="a806b-136">String</span></span>| <span data-ttu-id="a806b-137">A duração de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a806b-137">The duration of a role assignment.</span></span>|
|<span data-ttu-id="a806b-138">motivo</span><span class="sxs-lookup"><span data-stu-id="a806b-138">reason</span></span>|<span data-ttu-id="a806b-139">String</span><span class="sxs-lookup"><span data-stu-id="a806b-139">String</span></span>| <span data-ttu-id="a806b-140">O motivo para a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a806b-140">The reason for the role assignment.</span></span>|
|<span data-ttu-id="a806b-141">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="a806b-141">requestedDateTime</span></span>|<span data-ttu-id="a806b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a806b-142">DateTimeOffset</span></span>| <span data-ttu-id="a806b-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a806b-143">Read-only.</span></span> <span data-ttu-id="a806b-144">A solicitação criar horário.</span><span class="sxs-lookup"><span data-stu-id="a806b-144">The request create time.</span></span> <span data-ttu-id="a806b-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a806b-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a806b-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a806b-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a806b-147">roleId</span><span class="sxs-lookup"><span data-stu-id="a806b-147">roleId</span></span>|<span data-ttu-id="a806b-148">String</span><span class="sxs-lookup"><span data-stu-id="a806b-148">String</span></span>| <span data-ttu-id="a806b-149">A identificação da função.</span><span class="sxs-lookup"><span data-stu-id="a806b-149">The id of the role.</span></span>|
|<span data-ttu-id="a806b-150">agenda</span><span class="sxs-lookup"><span data-stu-id="a806b-150">schedule</span></span>|[<span data-ttu-id="a806b-151">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a806b-151">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="a806b-152">O objeto de agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a806b-152">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="a806b-153">status</span><span class="sxs-lookup"><span data-stu-id="a806b-153">status</span></span>|<span data-ttu-id="a806b-154">String</span><span class="sxs-lookup"><span data-stu-id="a806b-154">String</span></span>| <span data-ttu-id="a806b-155">Leitura-only.The o status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a806b-155">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="a806b-156">O valor pode ser `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="a806b-156">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="a806b-157">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="a806b-157">ticketNumber</span></span>|<span data-ttu-id="a806b-158">String</span><span class="sxs-lookup"><span data-stu-id="a806b-158">String</span></span>| <span data-ttu-id="a806b-159">TicketNumber para a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a806b-159">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="a806b-160">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="a806b-160">ticketSystem</span></span>|<span data-ttu-id="a806b-161">String</span><span class="sxs-lookup"><span data-stu-id="a806b-161">String</span></span>| <span data-ttu-id="a806b-162">TicketSystem para a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a806b-162">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="a806b-163">type</span><span class="sxs-lookup"><span data-stu-id="a806b-163">type</span></span>|<span data-ttu-id="a806b-164">String</span><span class="sxs-lookup"><span data-stu-id="a806b-164">String</span></span>| <span data-ttu-id="a806b-165">Representando o o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a806b-165">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="a806b-166">O valor pode ser `AdminAdd`: administradores adicionar usuários às funções; `UserAdd`: Os usuários adicionar atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="a806b-166">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="a806b-167">userId</span><span class="sxs-lookup"><span data-stu-id="a806b-167">userId</span></span>|<span data-ttu-id="a806b-168">String</span><span class="sxs-lookup"><span data-stu-id="a806b-168">String</span></span>| <span data-ttu-id="a806b-169">A identificação do usuário.</span><span class="sxs-lookup"><span data-stu-id="a806b-169">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a806b-170">Relações</span><span class="sxs-lookup"><span data-stu-id="a806b-170">Relationships</span></span>
| <span data-ttu-id="a806b-171">Relação</span><span class="sxs-lookup"><span data-stu-id="a806b-171">Relationship</span></span> | <span data-ttu-id="a806b-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="a806b-172">Type</span></span>        | <span data-ttu-id="a806b-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="a806b-173">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a806b-174">roleInfo</span><span class="sxs-lookup"><span data-stu-id="a806b-174">roleInfo</span></span>|[<span data-ttu-id="a806b-175">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="a806b-175">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="a806b-176">O objeto roleInfo da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a806b-176">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a806b-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a806b-177">JSON representation</span></span>

<span data-ttu-id="a806b-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a806b-178">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->