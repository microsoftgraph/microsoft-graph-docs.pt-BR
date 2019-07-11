---
title: tipo de recurso privilegedRoleAssignmentRequest
description: Representa a solicitação de operações de atribuição de função no gerenciamento de identidade do Privilegd.
localization_priority: Normal
ms.openlocfilehash: 240c84ecb0bf4f8d0e171f647f21eb6730c28d44
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621211"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="fb536-103">tipo de recurso privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="fb536-103">privilegedRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb536-104">Representa a solicitação de operações de atribuição de função no gerenciamento de identidade do Privilegd.</span><span class="sxs-lookup"><span data-stu-id="fb536-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="fb536-105">`privilegedRoleAssignmentRequest`é uma entidade com modelo de tíquete usada para gerenciar o ciclo de vida das atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="fb536-105">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="fb536-106">Ele representa a intenção/decisão dos usuários e administradores, e também fornece a flexibilidade para permitir a implementação de Schduling recorrentes, Gates de aprovação e assim por diante, em comparação com as `POST` operações `LIST` e exposição diretas, bem como `MY` e `Cancel` funções em `governanceRoleAssignment`.</span><span class="sxs-lookup"><span data-stu-id="fb536-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="fb536-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="fb536-107">Methods</span></span>

| <span data-ttu-id="fb536-108">Método</span><span class="sxs-lookup"><span data-stu-id="fb536-108">Method</span></span>       | <span data-ttu-id="fb536-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fb536-109">Return Type</span></span> | <span data-ttu-id="fb536-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb536-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="fb536-111">List</span><span class="sxs-lookup"><span data-stu-id="fb536-111">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="fb536-112">coleção [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="fb536-112">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="fb536-113">Listar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fb536-113">List role assignment requests.</span></span>|
|[<span data-ttu-id="fb536-114">Create</span><span class="sxs-lookup"><span data-stu-id="fb536-114">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="fb536-115">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="fb536-115">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="fb536-116">Criar uma solicitação para gerenciar o ciclo de vida da atribuição de função nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="fb536-116">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="fb536-117">Cancel</span><span class="sxs-lookup"><span data-stu-id="fb536-117">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="fb536-118">Cancelar uma solicitação de atribuição de função pendente.</span><span class="sxs-lookup"><span data-stu-id="fb536-118">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="fb536-119">Pessoal</span><span class="sxs-lookup"><span data-stu-id="fb536-119">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="fb536-120">Obter solicitação de atribuição de função para o requstor atual.</span><span class="sxs-lookup"><span data-stu-id="fb536-120">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="fb536-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb536-121">Properties</span></span>

| <span data-ttu-id="fb536-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb536-122">Property</span></span>     | <span data-ttu-id="fb536-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb536-123">Type</span></span>        | <span data-ttu-id="fb536-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb536-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fb536-125">id</span><span class="sxs-lookup"><span data-stu-id="fb536-125">id</span></span>|<span data-ttu-id="fb536-126">String</span><span class="sxs-lookup"><span data-stu-id="fb536-126">String</span></span>| <span data-ttu-id="fb536-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fb536-127">Read-only.</span></span> <span data-ttu-id="fb536-128">A ID da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fb536-128">The id of the role assignment request.</span></span>|
|<span data-ttu-id="fb536-129">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="fb536-129">assignmentState</span></span>|<span data-ttu-id="fb536-130">String</span><span class="sxs-lookup"><span data-stu-id="fb536-130">String</span></span>| <span data-ttu-id="fb536-131">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="fb536-131">The state of the assignment.</span></span> <span data-ttu-id="fb536-132">O valor pode ser `Eligible` para atribuição `Active` qualificada-se for diretamente atribuído `Active` por administradores ou ativado em uma atribuição qualificada pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="fb536-132">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="fb536-133">duration</span><span class="sxs-lookup"><span data-stu-id="fb536-133">duration</span></span>|<span data-ttu-id="fb536-134">String</span><span class="sxs-lookup"><span data-stu-id="fb536-134">String</span></span>| <span data-ttu-id="fb536-135">A duração de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fb536-135">The duration of a role assignment.</span></span>|
|<span data-ttu-id="fb536-136">motivos</span><span class="sxs-lookup"><span data-stu-id="fb536-136">reason</span></span>|<span data-ttu-id="fb536-137">String</span><span class="sxs-lookup"><span data-stu-id="fb536-137">String</span></span>| <span data-ttu-id="fb536-138">O motivo da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fb536-138">The reason for the role assignment.</span></span>|
|<span data-ttu-id="fb536-139">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb536-139">requestedDateTime</span></span>|<span data-ttu-id="fb536-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb536-140">DateTimeOffset</span></span>| <span data-ttu-id="fb536-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fb536-141">Read-only.</span></span> <span data-ttu-id="fb536-142">O tempo de criação da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb536-142">The request create time.</span></span> <span data-ttu-id="fb536-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="fb536-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fb536-144">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fb536-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="fb536-145">roleId</span><span class="sxs-lookup"><span data-stu-id="fb536-145">roleId</span></span>|<span data-ttu-id="fb536-146">String</span><span class="sxs-lookup"><span data-stu-id="fb536-146">String</span></span>| <span data-ttu-id="fb536-147">A ID da função.</span><span class="sxs-lookup"><span data-stu-id="fb536-147">The id of the role.</span></span>|
|<span data-ttu-id="fb536-148">Cronograma</span><span class="sxs-lookup"><span data-stu-id="fb536-148">schedule</span></span>|[<span data-ttu-id="fb536-149">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="fb536-149">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="fb536-150">O objeto Schedule da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fb536-150">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="fb536-151">status</span><span class="sxs-lookup"><span data-stu-id="fb536-151">status</span></span>|<span data-ttu-id="fb536-152">String</span><span class="sxs-lookup"><span data-stu-id="fb536-152">String</span></span>| <span data-ttu-id="fb536-153">Somente leitura. o status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fb536-153">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="fb536-154">O valor pode ser `NotStarted`,`Completed`,`RequestedApproval``Scheduled``Approved``ApprovalDenied``ApprovalAborted``Cancelling`,,,,,,,`RequestExpired``Cancelled``Revoked`</span><span class="sxs-lookup"><span data-stu-id="fb536-154">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="fb536-155">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="fb536-155">ticketNumber</span></span>|<span data-ttu-id="fb536-156">String</span><span class="sxs-lookup"><span data-stu-id="fb536-156">String</span></span>| <span data-ttu-id="fb536-157">O ticketNumber da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fb536-157">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="fb536-158">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="fb536-158">ticketSystem</span></span>|<span data-ttu-id="fb536-159">String</span><span class="sxs-lookup"><span data-stu-id="fb536-159">String</span></span>| <span data-ttu-id="fb536-160">O ticketSystem da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fb536-160">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="fb536-161">type</span><span class="sxs-lookup"><span data-stu-id="fb536-161">type</span></span>|<span data-ttu-id="fb536-162">String</span><span class="sxs-lookup"><span data-stu-id="fb536-162">String</span></span>| <span data-ttu-id="fb536-163">Representando o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fb536-163">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="fb536-164">O valor pode ser `AdminAdd`: os administradores adicionam usuários a funções; `UserAdd`: Os usuários adicionam atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="fb536-164">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="fb536-165">userId</span><span class="sxs-lookup"><span data-stu-id="fb536-165">userId</span></span>|<span data-ttu-id="fb536-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb536-166">String</span></span>| <span data-ttu-id="fb536-167">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="fb536-167">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb536-168">Relações</span><span class="sxs-lookup"><span data-stu-id="fb536-168">Relationships</span></span>
| <span data-ttu-id="fb536-169">Relação</span><span class="sxs-lookup"><span data-stu-id="fb536-169">Relationship</span></span> | <span data-ttu-id="fb536-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb536-170">Type</span></span>        | <span data-ttu-id="fb536-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb536-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fb536-172">roleInfo</span><span class="sxs-lookup"><span data-stu-id="fb536-172">roleInfo</span></span>|[<span data-ttu-id="fb536-173">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="fb536-173">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="fb536-174">O objeto roleInfo da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fb536-174">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb536-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb536-175">JSON representation</span></span>

<span data-ttu-id="fb536-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb536-176">The following is a JSON representation of the resource.</span></span>

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
