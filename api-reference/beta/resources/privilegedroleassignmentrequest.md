---
title: tipo de recurso privilegedRoleAssignmentRequest
description: Representa a solicitação de operações de atribuição de função no gerenciamento de identidade do Privilegd.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 26a6c46d014ae1820b0355272cbebc5b371746dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521499"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="758e7-103">tipo de recurso privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="758e7-103">privilegedRoleAssignmentRequest resource type</span></span>

<span data-ttu-id="758e7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="758e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="758e7-105">Representa a solicitação de operações de atribuição de função no gerenciamento de identidade do Privilegd.</span><span class="sxs-lookup"><span data-stu-id="758e7-105">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="758e7-106">`privilegedRoleAssignmentRequest`é uma entidade com modelo de tíquete usada para gerenciar o ciclo de vida das atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="758e7-106">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="758e7-107">Ele representa a intenção/decisão dos usuários e administradores, e também fornece a flexibilidade para permitir a implementação de Schduling recorrentes, Gates de aprovação e assim por diante, em comparação com a `POST` exposição `LIST` e operações diretas `MY` , `Cancel` bem como `governanceRoleAssignment`e funções.</span><span class="sxs-lookup"><span data-stu-id="758e7-107">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="758e7-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="758e7-108">Methods</span></span>

| <span data-ttu-id="758e7-109">Método</span><span class="sxs-lookup"><span data-stu-id="758e7-109">Method</span></span>       | <span data-ttu-id="758e7-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="758e7-110">Return Type</span></span> | <span data-ttu-id="758e7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="758e7-111">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="758e7-112">List</span><span class="sxs-lookup"><span data-stu-id="758e7-112">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="758e7-113">coleção [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="758e7-113">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="758e7-114">Listar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="758e7-114">List role assignment requests.</span></span>|
|[<span data-ttu-id="758e7-115">Create</span><span class="sxs-lookup"><span data-stu-id="758e7-115">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="758e7-116">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="758e7-116">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="758e7-117">Criar uma solicitação para gerenciar o ciclo de vida da atribuição de função nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="758e7-117">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="758e7-118">Cancel</span><span class="sxs-lookup"><span data-stu-id="758e7-118">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="758e7-119">Cancelar uma solicitação de atribuição de função pendente.</span><span class="sxs-lookup"><span data-stu-id="758e7-119">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="758e7-120">Pessoal</span><span class="sxs-lookup"><span data-stu-id="758e7-120">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="758e7-121">Obter solicitação de atribuição de função para o requstor atual.</span><span class="sxs-lookup"><span data-stu-id="758e7-121">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="758e7-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="758e7-122">Properties</span></span>

| <span data-ttu-id="758e7-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="758e7-123">Property</span></span>     | <span data-ttu-id="758e7-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="758e7-124">Type</span></span>        | <span data-ttu-id="758e7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="758e7-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="758e7-126">id</span><span class="sxs-lookup"><span data-stu-id="758e7-126">id</span></span>|<span data-ttu-id="758e7-127">String</span><span class="sxs-lookup"><span data-stu-id="758e7-127">String</span></span>| <span data-ttu-id="758e7-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="758e7-128">Read-only.</span></span> <span data-ttu-id="758e7-129">A ID da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="758e7-129">The id of the role assignment request.</span></span>|
|<span data-ttu-id="758e7-130">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="758e7-130">assignmentState</span></span>|<span data-ttu-id="758e7-131">String</span><span class="sxs-lookup"><span data-stu-id="758e7-131">String</span></span>| <span data-ttu-id="758e7-132">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="758e7-132">The state of the assignment.</span></span> <span data-ttu-id="758e7-133">O valor pode ser `Eligible` para atribuição `Active` qualificada-se for diretamente atribuído `Active` por administradores ou ativado em uma atribuição qualificada pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="758e7-133">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="758e7-134">duration</span><span class="sxs-lookup"><span data-stu-id="758e7-134">duration</span></span>|<span data-ttu-id="758e7-135">String</span><span class="sxs-lookup"><span data-stu-id="758e7-135">String</span></span>| <span data-ttu-id="758e7-136">A duração de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="758e7-136">The duration of a role assignment.</span></span>|
|<span data-ttu-id="758e7-137">motivo</span><span class="sxs-lookup"><span data-stu-id="758e7-137">reason</span></span>|<span data-ttu-id="758e7-138">String</span><span class="sxs-lookup"><span data-stu-id="758e7-138">String</span></span>| <span data-ttu-id="758e7-139">O motivo da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="758e7-139">The reason for the role assignment.</span></span>|
|<span data-ttu-id="758e7-140">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="758e7-140">requestedDateTime</span></span>|<span data-ttu-id="758e7-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="758e7-141">DateTimeOffset</span></span>| <span data-ttu-id="758e7-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="758e7-142">Read-only.</span></span> <span data-ttu-id="758e7-143">O tempo de criação da solicitação.</span><span class="sxs-lookup"><span data-stu-id="758e7-143">The request create time.</span></span> <span data-ttu-id="758e7-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="758e7-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="758e7-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="758e7-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="758e7-146">roleId</span><span class="sxs-lookup"><span data-stu-id="758e7-146">roleId</span></span>|<span data-ttu-id="758e7-147">String</span><span class="sxs-lookup"><span data-stu-id="758e7-147">String</span></span>| <span data-ttu-id="758e7-148">A ID da função.</span><span class="sxs-lookup"><span data-stu-id="758e7-148">The id of the role.</span></span>|
|<span data-ttu-id="758e7-149">Cronograma</span><span class="sxs-lookup"><span data-stu-id="758e7-149">schedule</span></span>|[<span data-ttu-id="758e7-150">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="758e7-150">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="758e7-151">O objeto Schedule da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="758e7-151">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="758e7-152">status</span><span class="sxs-lookup"><span data-stu-id="758e7-152">status</span></span>|<span data-ttu-id="758e7-153">String</span><span class="sxs-lookup"><span data-stu-id="758e7-153">String</span></span>| <span data-ttu-id="758e7-154">Somente leitura. o status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="758e7-154">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="758e7-155">O valor pode ser `NotStarted`,`Completed`,`RequestedApproval``Scheduled``Approved``ApprovalDenied``ApprovalAborted``Cancelling`,,,,,,,`RequestExpired``Cancelled``Revoked`</span><span class="sxs-lookup"><span data-stu-id="758e7-155">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="758e7-156">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="758e7-156">ticketNumber</span></span>|<span data-ttu-id="758e7-157">String</span><span class="sxs-lookup"><span data-stu-id="758e7-157">String</span></span>| <span data-ttu-id="758e7-158">O ticketNumber da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="758e7-158">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="758e7-159">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="758e7-159">ticketSystem</span></span>|<span data-ttu-id="758e7-160">String</span><span class="sxs-lookup"><span data-stu-id="758e7-160">String</span></span>| <span data-ttu-id="758e7-161">O ticketSystem da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="758e7-161">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="758e7-162">type</span><span class="sxs-lookup"><span data-stu-id="758e7-162">type</span></span>|<span data-ttu-id="758e7-163">String</span><span class="sxs-lookup"><span data-stu-id="758e7-163">String</span></span>| <span data-ttu-id="758e7-164">Representando o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="758e7-164">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="758e7-165">O valor pode ser `AdminAdd`: os administradores adicionam usuários a funções; `UserAdd`: Os usuários adicionam atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="758e7-165">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="758e7-166">userId</span><span class="sxs-lookup"><span data-stu-id="758e7-166">userId</span></span>|<span data-ttu-id="758e7-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="758e7-167">String</span></span>| <span data-ttu-id="758e7-168">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="758e7-168">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="758e7-169">Relações</span><span class="sxs-lookup"><span data-stu-id="758e7-169">Relationships</span></span>
| <span data-ttu-id="758e7-170">Relação</span><span class="sxs-lookup"><span data-stu-id="758e7-170">Relationship</span></span> | <span data-ttu-id="758e7-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="758e7-171">Type</span></span>        | <span data-ttu-id="758e7-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="758e7-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="758e7-173">roleInfo</span><span class="sxs-lookup"><span data-stu-id="758e7-173">roleInfo</span></span>|[<span data-ttu-id="758e7-174">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="758e7-174">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="758e7-175">O objeto roleInfo da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="758e7-175">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="758e7-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="758e7-176">JSON representation</span></span>

<span data-ttu-id="758e7-177">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="758e7-177">The following is a JSON representation of the resource.</span></span>

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
