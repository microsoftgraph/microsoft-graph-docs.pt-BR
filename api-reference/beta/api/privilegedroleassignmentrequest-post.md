---
title: Criar privilegedRoleAssignmentRequest
description: Crie um objeto privilegedroleassignmentrequest.
localization_priority: Normal
ms.openlocfilehash: e3158e918d061f09dec9e74c9e3bfd66d95fa48d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521065"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="a9654-103">Criar privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="a9654-103">Create privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9654-104">Crie um objeto [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="a9654-104">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9654-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9654-105">Permissions</span></span>
<span data-ttu-id="a9654-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9654-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9654-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9654-108">Permission type</span></span>                        | <span data-ttu-id="a9654-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9654-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9654-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9654-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a9654-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a9654-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a9654-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9654-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9654-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9654-113">Not supported.</span></span> |
|<span data-ttu-id="a9654-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9654-114">Application</span></span>                            | <span data-ttu-id="a9654-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9654-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9654-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9654-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="a9654-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9654-117">Request headers</span></span>
| <span data-ttu-id="a9654-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a9654-118">Name</span></span>      |<span data-ttu-id="a9654-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9654-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9654-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9654-120">Authorization</span></span>  | <span data-ttu-id="a9654-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9654-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9654-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9654-123">Request body</span></span>
<span data-ttu-id="a9654-124">No corpo da solicitação, fornece uma representação JSON do objeto [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="a9654-124">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="a9654-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9654-125">Property</span></span>     | <span data-ttu-id="a9654-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9654-126">Type</span></span>    |  <span data-ttu-id="a9654-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9654-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9654-128">roleId</span><span class="sxs-lookup"><span data-stu-id="a9654-128">roleId</span></span>|<span data-ttu-id="a9654-129">String</span><span class="sxs-lookup"><span data-stu-id="a9654-129">String</span></span>|<span data-ttu-id="a9654-130">A identificação da função.</span><span class="sxs-lookup"><span data-stu-id="a9654-130">The ID of the role.</span></span> <span data-ttu-id="a9654-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9654-131">Required.</span></span>|
|<span data-ttu-id="a9654-132">type</span><span class="sxs-lookup"><span data-stu-id="a9654-132">type</span></span>|<span data-ttu-id="a9654-133">String</span><span class="sxs-lookup"><span data-stu-id="a9654-133">String</span></span>|<span data-ttu-id="a9654-134">Representa o o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a9654-134">Represents the the type of the operation on the role assignment.</span></span> <span data-ttu-id="a9654-135">O valor pode ser `AdminAdd`: administradores adicionar usuários às funções; `UserAdd`: Os usuários adicionar atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="a9654-135">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="a9654-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9654-136">Required.</span></span>|
|<span data-ttu-id="a9654-137">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a9654-137">assignmentState</span></span>|<span data-ttu-id="a9654-138">String</span><span class="sxs-lookup"><span data-stu-id="a9654-138">String</span></span>|<span data-ttu-id="a9654-139">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="a9654-139">The state of the assignment.</span></span> <span data-ttu-id="a9654-140">O valor pode ser `Eligible` para atribuição elegível `Active` - se ele é atribuído diretamente `Active` pelos administradores, ou ativado em uma atribuição elegível pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="a9654-140">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="a9654-141">Os valores possíveis são: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="a9654-141">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="a9654-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9654-142">Required.</span></span>|
|<span data-ttu-id="a9654-143">Reason</span><span class="sxs-lookup"><span data-stu-id="a9654-143">reason</span></span>|<span data-ttu-id="a9654-144">String</span><span class="sxs-lookup"><span data-stu-id="a9654-144">String</span></span>|<span data-ttu-id="a9654-145">O motivo pelo qual deve ser fornecido para a solicitação de atribuição de função de auditoria e revise finalidade.</span><span class="sxs-lookup"><span data-stu-id="a9654-145">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="a9654-146">Schedule</span><span class="sxs-lookup"><span data-stu-id="a9654-146">schedule</span></span>|[<span data-ttu-id="a9654-147">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a9654-147">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="a9654-148">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a9654-148">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="a9654-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9654-149">Response</span></span>
<span data-ttu-id="a9654-150">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9654-150">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="a9654-151">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="a9654-151">Error codes</span></span>
<span data-ttu-id="a9654-152">Essa API retorna esse padrão códigos de erro HTTP.</span><span class="sxs-lookup"><span data-stu-id="a9654-152">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="a9654-153">Além disso, ele pode retornar os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a9654-153">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="a9654-154">Código de erro</span><span class="sxs-lookup"><span data-stu-id="a9654-154">Error code</span></span>     | <span data-ttu-id="a9654-155">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="a9654-155">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="a9654-156">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9654-156">400 BadRequest</span></span> | <span data-ttu-id="a9654-157">Propriedade RoleAssignmentRequest foi NULL</span><span class="sxs-lookup"><span data-stu-id="a9654-157">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="a9654-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9654-158">400 BadRequest</span></span> | <span data-ttu-id="a9654-159">Não é possível desserializar roleAssignmentRequest objeto.</span><span class="sxs-lookup"><span data-stu-id="a9654-159">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="a9654-160">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9654-160">400 BadRequest</span></span> | <span data-ttu-id="a9654-161">RoleId é necessário.</span><span class="sxs-lookup"><span data-stu-id="a9654-161">RoleId is required.</span></span> |
| <span data-ttu-id="a9654-162">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9654-162">400 BadRequest</span></span> | <span data-ttu-id="a9654-163">Data de início de agendamento deve ser especificada e deve ser maior do que agora.</span><span class="sxs-lookup"><span data-stu-id="a9654-163">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="a9654-164">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9654-164">400 BadRequest</span></span> | <span data-ttu-id="a9654-165">Já existe um agendamento para esse tipo de usuário, a função e a agenda.</span><span class="sxs-lookup"><span data-stu-id="a9654-165">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="a9654-166">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9654-166">400 BadRequest</span></span> | <span data-ttu-id="a9654-167">Uma aprovação pendente já existe para esse tipo de usuário, função e aprovação.</span><span class="sxs-lookup"><span data-stu-id="a9654-167">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="a9654-168">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9654-168">400 BadRequest</span></span> | <span data-ttu-id="a9654-169">Motivo solicitante está faltando.</span><span class="sxs-lookup"><span data-stu-id="a9654-169">Requestor reason is missing.</span></span> |
| <span data-ttu-id="a9654-170">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9654-170">400 BadRequest</span></span> | <span data-ttu-id="a9654-171">Motivo solicitante deve ser menor do que 500 caracteres.</span><span class="sxs-lookup"><span data-stu-id="a9654-171">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="a9654-172">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9654-172">400 BadRequest</span></span> | <span data-ttu-id="a9654-173">Duração de elevação deve estar entre 0,5 e {de configuração}.</span><span class="sxs-lookup"><span data-stu-id="a9654-173">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="a9654-174">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9654-174">400 BadRequest</span></span> | <span data-ttu-id="a9654-175">Não há uma sobreposição entre a ativação agendada e a solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9654-175">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="a9654-176">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9654-176">400 BadRequest</span></span> | <span data-ttu-id="a9654-177">A função já está ativada.</span><span class="sxs-lookup"><span data-stu-id="a9654-177">The role is already activated.</span></span> |
| <span data-ttu-id="a9654-178">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9654-178">400 BadRequest</span></span> | <span data-ttu-id="a9654-179">GenericElevateUserToRoleAssignments: Tickting informações é necessário e não são fornecidas no processo de ativação.</span><span class="sxs-lookup"><span data-stu-id="a9654-179">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="a9654-180">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a9654-180">400 BadRequest</span></span> | <span data-ttu-id="a9654-181">Não há uma sobreposição entre a ativação agendada e a solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9654-181">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="a9654-182">403 não autorizado</span><span class="sxs-lookup"><span data-stu-id="a9654-182">403 UnAuthorized</span></span> | <span data-ttu-id="a9654-183">Elevação exige a autenticação multifator.</span><span class="sxs-lookup"><span data-stu-id="a9654-183">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="a9654-184">403 não autorizado</span><span class="sxs-lookup"><span data-stu-id="a9654-184">403 UnAuthorized</span></span> | <span data-ttu-id="a9654-185">Em nome de elevação não é permitida.</span><span class="sxs-lookup"><span data-stu-id="a9654-185">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="a9654-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9654-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9654-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9654-187">Request</span></span>
<span data-ttu-id="a9654-188">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9654-188">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_privilegedroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
Content-type: application/json

{
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "schedule": {
        "startDateTime": "2018-02-08T02:35:17.903Z"
    },
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
##### <a name="response"></a><span data-ttu-id="a9654-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9654-189">Response</span></span>
<span data-ttu-id="a9654-190">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9654-190">The following is an example of the response.</span></span> <span data-ttu-id="a9654-191">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a9654-191">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a9654-192">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9654-192">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "NotStarted",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self"，
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
