---
title: Tipo de recurso privilegedRoleAssignmentRequest
description: Representa a solicitação de operações de atribuição de função em Gerenciamento de Identidade Privilegd.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 2a976632c038f87a1a3e09c3683ebcdd6d448b35
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443997"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="ba923-103">Tipo de recurso privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="ba923-103">privilegedRoleAssignmentRequest resource type</span></span>

<span data-ttu-id="ba923-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba923-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba923-105">Representa a solicitação de operações de atribuição de função em Gerenciamento de Identidade Privilegd.</span><span class="sxs-lookup"><span data-stu-id="ba923-105">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="ba923-106">`privilegedRoleAssignmentRequest` é uma entidade modelada por tíquete usada para gerenciar o ciclo de vida das atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="ba923-106">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="ba923-107">Ele representa a intenção/decisão dos usuários e administradores e também oferece a flexibilidade para habilitar a implementação de esquemas `POST` `LIST` `MY` `Cancel` recorrentes, portais de aprovação e assim por diante, em comparação com a exposição direta e operações, bem como e funções em `governanceRoleAssignment` .</span><span class="sxs-lookup"><span data-stu-id="ba923-107">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="ba923-108">Methods</span><span class="sxs-lookup"><span data-stu-id="ba923-108">Methods</span></span>

| <span data-ttu-id="ba923-109">Método</span><span class="sxs-lookup"><span data-stu-id="ba923-109">Method</span></span>       | <span data-ttu-id="ba923-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ba923-110">Return Type</span></span> | <span data-ttu-id="ba923-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba923-111">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="ba923-112">List</span><span class="sxs-lookup"><span data-stu-id="ba923-112">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="ba923-113">[Coleção privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="ba923-113">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="ba923-114">Listar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ba923-114">List role assignment requests.</span></span>|
|[<span data-ttu-id="ba923-115">Create</span><span class="sxs-lookup"><span data-stu-id="ba923-115">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="ba923-116">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="ba923-116">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="ba923-117">Crie uma solicitação para gerenciar o ciclo de vida da atribuição de função existente ou nova.</span><span class="sxs-lookup"><span data-stu-id="ba923-117">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="ba923-118">Cancel</span><span class="sxs-lookup"><span data-stu-id="ba923-118">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="ba923-119">Cancele uma solicitação de atribuição de função pendente.</span><span class="sxs-lookup"><span data-stu-id="ba923-119">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="ba923-120">Pessoal</span><span class="sxs-lookup"><span data-stu-id="ba923-120">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="ba923-121">Obter solicitação de atribuição de função para o requstor atual.</span><span class="sxs-lookup"><span data-stu-id="ba923-121">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="ba923-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba923-122">Properties</span></span>

| <span data-ttu-id="ba923-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba923-123">Property</span></span>     | <span data-ttu-id="ba923-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba923-124">Type</span></span>        | <span data-ttu-id="ba923-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba923-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ba923-126">id</span><span class="sxs-lookup"><span data-stu-id="ba923-126">id</span></span>|<span data-ttu-id="ba923-127">String</span><span class="sxs-lookup"><span data-stu-id="ba923-127">String</span></span>| <span data-ttu-id="ba923-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ba923-128">Read-only.</span></span> <span data-ttu-id="ba923-129">A id da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ba923-129">The id of the role assignment request.</span></span>|
|<span data-ttu-id="ba923-130">assignmentState</span><span class="sxs-lookup"><span data-stu-id="ba923-130">assignmentState</span></span>|<span data-ttu-id="ba923-131">String</span><span class="sxs-lookup"><span data-stu-id="ba923-131">String</span></span>| <span data-ttu-id="ba923-132">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="ba923-132">The state of the assignment.</span></span> <span data-ttu-id="ba923-133">O valor pode ser para atribuição qualificada - se ele for atribuído diretamente pelos administradores ou ativado em uma atribuição qualificada `Eligible` `Active` pelos `Active` usuários.</span><span class="sxs-lookup"><span data-stu-id="ba923-133">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="ba923-134">duração</span><span class="sxs-lookup"><span data-stu-id="ba923-134">duration</span></span>|<span data-ttu-id="ba923-135">String</span><span class="sxs-lookup"><span data-stu-id="ba923-135">String</span></span>| <span data-ttu-id="ba923-136">A duração de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ba923-136">The duration of a role assignment.</span></span>|
|<span data-ttu-id="ba923-137">motivo</span><span class="sxs-lookup"><span data-stu-id="ba923-137">reason</span></span>|<span data-ttu-id="ba923-138">String</span><span class="sxs-lookup"><span data-stu-id="ba923-138">String</span></span>| <span data-ttu-id="ba923-139">O motivo da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ba923-139">The reason for the role assignment.</span></span>|
|<span data-ttu-id="ba923-140">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba923-140">requestedDateTime</span></span>|<span data-ttu-id="ba923-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba923-141">DateTimeOffset</span></span>| <span data-ttu-id="ba923-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ba923-142">Read-only.</span></span> <span data-ttu-id="ba923-143">A solicitação cria tempo.</span><span class="sxs-lookup"><span data-stu-id="ba923-143">The request create time.</span></span> <span data-ttu-id="ba923-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ba923-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ba923-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ba923-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ba923-146">roleId</span><span class="sxs-lookup"><span data-stu-id="ba923-146">roleId</span></span>|<span data-ttu-id="ba923-147">String</span><span class="sxs-lookup"><span data-stu-id="ba923-147">String</span></span>| <span data-ttu-id="ba923-148">A id da função.</span><span class="sxs-lookup"><span data-stu-id="ba923-148">The id of the role.</span></span>|
|<span data-ttu-id="ba923-149">Cronograma</span><span class="sxs-lookup"><span data-stu-id="ba923-149">schedule</span></span>|[<span data-ttu-id="ba923-150">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="ba923-150">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="ba923-151">O objeto schedule da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ba923-151">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="ba923-152">status</span><span class="sxs-lookup"><span data-stu-id="ba923-152">status</span></span>|<span data-ttu-id="ba923-153">String</span><span class="sxs-lookup"><span data-stu-id="ba923-153">String</span></span>| <span data-ttu-id="ba923-154">Somente leitura.O status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ba923-154">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="ba923-155">O valor pode `NotStarted` ser , , , , , , , , `Completed` , , , `RequestedApproval` `Scheduled` `Approved` `ApprovalDenied` `ApprovalAborted` `Cancelling` `Cancelled` `Revoked` `RequestExpired` .</span><span class="sxs-lookup"><span data-stu-id="ba923-155">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="ba923-156">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="ba923-156">ticketNumber</span></span>|<span data-ttu-id="ba923-157">String</span><span class="sxs-lookup"><span data-stu-id="ba923-157">String</span></span>| <span data-ttu-id="ba923-158">O ticketNumber para a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ba923-158">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="ba923-159">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="ba923-159">ticketSystem</span></span>|<span data-ttu-id="ba923-160">String</span><span class="sxs-lookup"><span data-stu-id="ba923-160">String</span></span>| <span data-ttu-id="ba923-161">O ticketSystem para a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ba923-161">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="ba923-162">type</span><span class="sxs-lookup"><span data-stu-id="ba923-162">type</span></span>|<span data-ttu-id="ba923-163">String</span><span class="sxs-lookup"><span data-stu-id="ba923-163">String</span></span>| <span data-ttu-id="ba923-164">Representando o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ba923-164">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="ba923-165">O valor pode ser `AdminAdd` : Administradores adicionam usuários a funções; `UserAdd` : Os usuários adicionam atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="ba923-165">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="ba923-166">userId</span><span class="sxs-lookup"><span data-stu-id="ba923-166">userId</span></span>|<span data-ttu-id="ba923-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba923-167">String</span></span>| <span data-ttu-id="ba923-168">A id do usuário.</span><span class="sxs-lookup"><span data-stu-id="ba923-168">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba923-169">Relações</span><span class="sxs-lookup"><span data-stu-id="ba923-169">Relationships</span></span>
| <span data-ttu-id="ba923-170">Relação</span><span class="sxs-lookup"><span data-stu-id="ba923-170">Relationship</span></span> | <span data-ttu-id="ba923-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba923-171">Type</span></span>        | <span data-ttu-id="ba923-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba923-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ba923-173">roleInfo</span><span class="sxs-lookup"><span data-stu-id="ba923-173">roleInfo</span></span>|[<span data-ttu-id="ba923-174">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="ba923-174">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="ba923-175">O objeto roleInfo da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ba923-175">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba923-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba923-176">JSON representation</span></span>

<span data-ttu-id="ba923-177">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba923-177">The following is a JSON representation of the resource.</span></span>

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


