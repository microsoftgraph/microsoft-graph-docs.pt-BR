---
title: tipo de recurso de privilegedRoleAssignmentRequest
description: Representa a solicitação para operações de atribuição de função no gerenciamento de identidades Privilegd.
localization_priority: Normal
ms.openlocfilehash: c0e0bbfa76b7ffb4e122d381d45dd4092f0843c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509004"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="7f8cc-103">tipo de recurso de privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="7f8cc-103">privilegedRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f8cc-104">Representa a solicitação para operações de atribuição de função no gerenciamento de identidades Privilegd.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="7f8cc-105">`privilegedRoleAssignmentRequest`uma entidade modelada de tíquete é usada para gerenciar o ciclo de vida de atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-105">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="7f8cc-106">Ele representa a intenção/decisão dos usuários e administradores e também oferece flexibilidade para permitir a implementação de schduling recorrente, entradas de aprovação e assim por diante, em relação ao diretamente expondo `POST` e `LIST` operações bem como `MY` e `Cancel` funciona em `governanceRoleAssignment`.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="7f8cc-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="7f8cc-107">Methods</span></span>

| <span data-ttu-id="7f8cc-108">Método</span><span class="sxs-lookup"><span data-stu-id="7f8cc-108">Method</span></span>       | <span data-ttu-id="7f8cc-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7f8cc-109">Return Type</span></span> | <span data-ttu-id="7f8cc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f8cc-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="7f8cc-111">List</span><span class="sxs-lookup"><span data-stu-id="7f8cc-111">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="7f8cc-112">coleção [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="7f8cc-112">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="7f8cc-113">Lista solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-113">List role assignment requests.</span></span>|
|[<span data-ttu-id="7f8cc-114">Create</span><span class="sxs-lookup"><span data-stu-id="7f8cc-114">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="7f8cc-115">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="7f8cc-115">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="7f8cc-116">Crie uma solicitação para gerenciar o ciclo de vida de atribuição de função de novo ou existente.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-116">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="7f8cc-117">Cancel</span><span class="sxs-lookup"><span data-stu-id="7f8cc-117">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="7f8cc-118">Cancele uma solicitação de atribuição de função pendente.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-118">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="7f8cc-119">Pessoal</span><span class="sxs-lookup"><span data-stu-id="7f8cc-119">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="7f8cc-120">Obtenha a solicitação de atribuição de função para requstor atual.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-120">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f8cc-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f8cc-121">Properties</span></span>

| <span data-ttu-id="7f8cc-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f8cc-122">Property</span></span>     | <span data-ttu-id="7f8cc-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f8cc-123">Type</span></span>        | <span data-ttu-id="7f8cc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f8cc-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7f8cc-125">id</span><span class="sxs-lookup"><span data-stu-id="7f8cc-125">id</span></span>|<span data-ttu-id="7f8cc-126">String</span><span class="sxs-lookup"><span data-stu-id="7f8cc-126">String</span></span>| <span data-ttu-id="7f8cc-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-127">Read-only.</span></span> <span data-ttu-id="7f8cc-128">A identificação da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-128">The id of the role assignment request.</span></span>|
|<span data-ttu-id="7f8cc-129">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7f8cc-129">assignmentState</span></span>|<span data-ttu-id="7f8cc-130">String</span><span class="sxs-lookup"><span data-stu-id="7f8cc-130">String</span></span>| <span data-ttu-id="7f8cc-131">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-131">The state of the assignment.</span></span> <span data-ttu-id="7f8cc-132">O valor pode ser `Eligible` para atribuição elegível `Active` - se ele é atribuído diretamente `Active` pelos administradores, ou ativado em uma atribuição elegível pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-132">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="7f8cc-133">duration</span><span class="sxs-lookup"><span data-stu-id="7f8cc-133">duration</span></span>|<span data-ttu-id="7f8cc-134">String</span><span class="sxs-lookup"><span data-stu-id="7f8cc-134">String</span></span>| <span data-ttu-id="7f8cc-135">A duração de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-135">The duration of a role assignment.</span></span>|
|<span data-ttu-id="7f8cc-136">Reason</span><span class="sxs-lookup"><span data-stu-id="7f8cc-136">reason</span></span>|<span data-ttu-id="7f8cc-137">String</span><span class="sxs-lookup"><span data-stu-id="7f8cc-137">String</span></span>| <span data-ttu-id="7f8cc-138">O motivo para a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-138">The reason for the role assignment.</span></span>|
|<span data-ttu-id="7f8cc-139">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f8cc-139">requestedDateTime</span></span>|<span data-ttu-id="7f8cc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f8cc-140">DateTimeOffset</span></span>| <span data-ttu-id="7f8cc-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-141">Read-only.</span></span> <span data-ttu-id="7f8cc-142">A solicitação criar horário.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-142">The request create time.</span></span> <span data-ttu-id="7f8cc-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7f8cc-144">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7f8cc-145">roleId</span><span class="sxs-lookup"><span data-stu-id="7f8cc-145">roleId</span></span>|<span data-ttu-id="7f8cc-146">String</span><span class="sxs-lookup"><span data-stu-id="7f8cc-146">String</span></span>| <span data-ttu-id="7f8cc-147">A identificação da função.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-147">The id of the role.</span></span>|
|<span data-ttu-id="7f8cc-148">Schedule</span><span class="sxs-lookup"><span data-stu-id="7f8cc-148">schedule</span></span>|[<span data-ttu-id="7f8cc-149">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7f8cc-149">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="7f8cc-150">O objeto de agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-150">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="7f8cc-151">status</span><span class="sxs-lookup"><span data-stu-id="7f8cc-151">status</span></span>|<span data-ttu-id="7f8cc-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f8cc-152">String</span></span>| <span data-ttu-id="7f8cc-153">Leitura-only.The o status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-153">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="7f8cc-154">O valor pode ser `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-154">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="7f8cc-155">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="7f8cc-155">ticketNumber</span></span>|<span data-ttu-id="7f8cc-156">String</span><span class="sxs-lookup"><span data-stu-id="7f8cc-156">String</span></span>| <span data-ttu-id="7f8cc-157">TicketNumber para a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-157">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="7f8cc-158">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="7f8cc-158">ticketSystem</span></span>|<span data-ttu-id="7f8cc-159">String</span><span class="sxs-lookup"><span data-stu-id="7f8cc-159">String</span></span>| <span data-ttu-id="7f8cc-160">TicketSystem para a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-160">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="7f8cc-161">type</span><span class="sxs-lookup"><span data-stu-id="7f8cc-161">type</span></span>|<span data-ttu-id="7f8cc-162">String</span><span class="sxs-lookup"><span data-stu-id="7f8cc-162">String</span></span>| <span data-ttu-id="7f8cc-163">Representando o o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-163">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="7f8cc-164">O valor pode ser `AdminAdd`: administradores adicionar usuários às funções; `UserAdd`: Os usuários adicionar atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-164">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="7f8cc-165">userId</span><span class="sxs-lookup"><span data-stu-id="7f8cc-165">userId</span></span>|<span data-ttu-id="7f8cc-166">String</span><span class="sxs-lookup"><span data-stu-id="7f8cc-166">String</span></span>| <span data-ttu-id="7f8cc-167">A identificação do usuário.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-167">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f8cc-168">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="7f8cc-168">Relationships</span></span>
| <span data-ttu-id="7f8cc-169">Relação</span><span class="sxs-lookup"><span data-stu-id="7f8cc-169">Relationship</span></span> | <span data-ttu-id="7f8cc-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f8cc-170">Type</span></span>        | <span data-ttu-id="7f8cc-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f8cc-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7f8cc-172">roleInfo</span><span class="sxs-lookup"><span data-stu-id="7f8cc-172">roleInfo</span></span>|[<span data-ttu-id="7f8cc-173">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="7f8cc-173">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="7f8cc-174">O objeto roleInfo da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-174">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f8cc-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f8cc-175">JSON representation</span></span>

<span data-ttu-id="7f8cc-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f8cc-176">The following is a JSON representation of the resource.</span></span>

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
