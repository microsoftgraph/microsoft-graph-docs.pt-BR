---
title: tipo de recurso de privilegedRoleAssignmentRequest
description: Representa a solicitação para operações de atribuição de função no gerenciamento de identidades Privilegd.
localization_priority: Normal
ms.openlocfilehash: a0cb0bc03d8bb2436e45139bc9db5322cc3970cf
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571741"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="f097b-103">tipo de recurso de privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f097b-103">privilegedRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f097b-104">Representa a solicitação para operações de atribuição de função no gerenciamento de identidades Privilegd.</span><span class="sxs-lookup"><span data-stu-id="f097b-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="f097b-105">`privilegedRoleAssignmentRequest`uma entidade modelada de tíquete é usada para gerenciar o ciclo de vida de atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="f097b-105">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="f097b-106">Ele representa a intenção/decisão dos usuários e administradores e também oferece flexibilidade para permitir a implementação de schduling recorrente, entradas de aprovação e assim por diante, em relação ao diretamente expondo `POST` e `LIST` operações bem como `MY` e `Cancel` funciona em `governanceRoleAssignment`.</span><span class="sxs-lookup"><span data-stu-id="f097b-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="f097b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f097b-107">Methods</span></span>

| <span data-ttu-id="f097b-108">Método</span><span class="sxs-lookup"><span data-stu-id="f097b-108">Method</span></span>       | <span data-ttu-id="f097b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f097b-109">Return Type</span></span> | <span data-ttu-id="f097b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f097b-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="f097b-111">List</span><span class="sxs-lookup"><span data-stu-id="f097b-111">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="f097b-112">coleção [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f097b-112">[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="f097b-113">Lista solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f097b-113">List role assignment requests.</span></span>|
|[<span data-ttu-id="f097b-114">Create</span><span class="sxs-lookup"><span data-stu-id="f097b-114">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="f097b-115">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f097b-115">privilegedRoleAssignmentRequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="f097b-116">Crie uma solicitação para gerenciar o ciclo de vida de atribuição de função de novo ou existente.</span><span class="sxs-lookup"><span data-stu-id="f097b-116">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="f097b-117">Cancel</span><span class="sxs-lookup"><span data-stu-id="f097b-117">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="f097b-118">Cancele uma solicitação de atribuição de função pendente.</span><span class="sxs-lookup"><span data-stu-id="f097b-118">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="f097b-119">Pessoal</span><span class="sxs-lookup"><span data-stu-id="f097b-119">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="f097b-120">Obtenha a solicitação de atribuição de função para o solicitante atual.</span><span class="sxs-lookup"><span data-stu-id="f097b-120">Get role assignment request for current requestor.</span></span>|

## <a name="properties"></a><span data-ttu-id="f097b-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f097b-121">Properties</span></span>

| <span data-ttu-id="f097b-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f097b-122">Property</span></span>     | <span data-ttu-id="f097b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f097b-123">Type</span></span>        | <span data-ttu-id="f097b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f097b-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f097b-125">id</span><span class="sxs-lookup"><span data-stu-id="f097b-125">id</span></span>|<span data-ttu-id="f097b-126">String</span><span class="sxs-lookup"><span data-stu-id="f097b-126">String</span></span>| <span data-ttu-id="f097b-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f097b-127">Read-only.</span></span> <span data-ttu-id="f097b-128">A identificação da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f097b-128">The id of the role assignment request.</span></span>|
|<span data-ttu-id="f097b-129">assignmentState</span><span class="sxs-lookup"><span data-stu-id="f097b-129">assignmentState</span></span>|<span data-ttu-id="f097b-130">String</span><span class="sxs-lookup"><span data-stu-id="f097b-130">String</span></span>| <span data-ttu-id="f097b-131">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="f097b-131">The state of the assignment.</span></span> <span data-ttu-id="f097b-132">O valor pode ser `Eligible` para atribuição elegível `Active` - se ele é atribuído diretamente `Active` pelos administradores, ou ativado em uma atribuição elegível pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="f097b-132">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="f097b-133">duration</span><span class="sxs-lookup"><span data-stu-id="f097b-133">duration</span></span>|<span data-ttu-id="f097b-134">String</span><span class="sxs-lookup"><span data-stu-id="f097b-134">String</span></span>| <span data-ttu-id="f097b-135">A duração de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f097b-135">The duration of a role assignment.</span></span>|
|<span data-ttu-id="f097b-136">motivo</span><span class="sxs-lookup"><span data-stu-id="f097b-136">reason</span></span>|<span data-ttu-id="f097b-137">String</span><span class="sxs-lookup"><span data-stu-id="f097b-137">String</span></span>| <span data-ttu-id="f097b-138">O motivo para a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f097b-138">The reason for the role assignment.</span></span>|
|<span data-ttu-id="f097b-139">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="f097b-139">requestedDateTime</span></span>|<span data-ttu-id="f097b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f097b-140">DateTimeOffset</span></span>| <span data-ttu-id="f097b-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f097b-141">Read-only.</span></span> <span data-ttu-id="f097b-142">A solicitação criar horário.</span><span class="sxs-lookup"><span data-stu-id="f097b-142">The request create time.</span></span> <span data-ttu-id="f097b-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f097b-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f097b-144">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f097b-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f097b-145">roleId</span><span class="sxs-lookup"><span data-stu-id="f097b-145">roleId</span></span>|<span data-ttu-id="f097b-146">String</span><span class="sxs-lookup"><span data-stu-id="f097b-146">String</span></span>| <span data-ttu-id="f097b-147">A identificação da função.</span><span class="sxs-lookup"><span data-stu-id="f097b-147">The id of the role.</span></span>|
|<span data-ttu-id="f097b-148">agenda</span><span class="sxs-lookup"><span data-stu-id="f097b-148">schedule</span></span>|[<span data-ttu-id="f097b-149">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f097b-149"> microsoft.graph.governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="f097b-150">O objeto de agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f097b-150">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="f097b-151">status</span><span class="sxs-lookup"><span data-stu-id="f097b-151">status</span></span>|<span data-ttu-id="f097b-152">String</span><span class="sxs-lookup"><span data-stu-id="f097b-152">String</span></span>| <span data-ttu-id="f097b-153">Leitura-only.The o status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f097b-153">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="f097b-154">O valor pode ser `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="f097b-154">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="f097b-155">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="f097b-155">ticketNumber</span></span>|<span data-ttu-id="f097b-156">String</span><span class="sxs-lookup"><span data-stu-id="f097b-156">String</span></span>| <span data-ttu-id="f097b-157">TicketNumber para a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f097b-157">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="f097b-158">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="f097b-158">ticketSystem</span></span>|<span data-ttu-id="f097b-159">String</span><span class="sxs-lookup"><span data-stu-id="f097b-159">String</span></span>| <span data-ttu-id="f097b-160">TicketSystem para a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f097b-160">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="f097b-161">type</span><span class="sxs-lookup"><span data-stu-id="f097b-161">type</span></span>|<span data-ttu-id="f097b-162">String</span><span class="sxs-lookup"><span data-stu-id="f097b-162">String</span></span>| <span data-ttu-id="f097b-163">Representando o o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f097b-163">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="f097b-164">O valor pode ser `AdminAdd`: administradores adicionar usuários às funções; `UserAdd`: Os usuários adicionar atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="f097b-164">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="f097b-165">userId</span><span class="sxs-lookup"><span data-stu-id="f097b-165">userId</span></span>|<span data-ttu-id="f097b-166">String</span><span class="sxs-lookup"><span data-stu-id="f097b-166">String</span></span>| <span data-ttu-id="f097b-167">A identificação do usuário.</span><span class="sxs-lookup"><span data-stu-id="f097b-167">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f097b-168">Relações</span><span class="sxs-lookup"><span data-stu-id="f097b-168">Relationships</span></span>
| <span data-ttu-id="f097b-169">Relação</span><span class="sxs-lookup"><span data-stu-id="f097b-169">Relationship</span></span> | <span data-ttu-id="f097b-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="f097b-170">Type</span></span>        | <span data-ttu-id="f097b-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="f097b-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f097b-172">roleInfo</span><span class="sxs-lookup"><span data-stu-id="f097b-172">roleInfo</span></span>|[<span data-ttu-id="f097b-173">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="f097b-173">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="f097b-174">O objeto roleInfo da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f097b-174">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f097b-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f097b-175">JSON representation</span></span>

<span data-ttu-id="f097b-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f097b-176">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedroleassignmentrequest.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
