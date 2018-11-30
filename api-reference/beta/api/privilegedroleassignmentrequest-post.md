---
title: Criar privilegedRoleAssignmentRequest
description: Crie um objeto privilegedroleassignmentrequest.
ms.openlocfilehash: e262682b5a5e8bffa7fb089ae783f3bb7e67803c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037067"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="d2354-103">Criar privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="d2354-103">Create privilegedRoleAssignmentRequest</span></span>

> <span data-ttu-id="d2354-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d2354-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2354-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d2354-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2354-106">Crie um objeto [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d2354-106">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2354-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d2354-107">Permissions</span></span>
<span data-ttu-id="d2354-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2354-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2354-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2354-110">Permission type</span></span>                        | <span data-ttu-id="d2354-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2354-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2354-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2354-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d2354-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d2354-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d2354-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2354-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2354-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2354-115">Not supported.</span></span> |
|<span data-ttu-id="d2354-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2354-116">Application</span></span>                            | <span data-ttu-id="d2354-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2354-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2354-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2354-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="d2354-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2354-119">Request headers</span></span>
| <span data-ttu-id="d2354-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d2354-120">Name</span></span>      |<span data-ttu-id="d2354-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2354-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2354-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2354-122">Authorization</span></span>  | <span data-ttu-id="d2354-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2354-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2354-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2354-125">Request body</span></span>
<span data-ttu-id="d2354-126">No corpo da solicitação, fornece uma representação JSON do objeto [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d2354-126">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="d2354-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2354-127">Property</span></span>     | <span data-ttu-id="d2354-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2354-128">Type</span></span>    |  <span data-ttu-id="d2354-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2354-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2354-130">roleId</span><span class="sxs-lookup"><span data-stu-id="d2354-130">roleId</span></span>|<span data-ttu-id="d2354-131">String</span><span class="sxs-lookup"><span data-stu-id="d2354-131">String</span></span>|<span data-ttu-id="d2354-132">A identificação da função.</span><span class="sxs-lookup"><span data-stu-id="d2354-132">The ID of the role.</span></span> <span data-ttu-id="d2354-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2354-133">Required.</span></span>|
|<span data-ttu-id="d2354-134">type</span><span class="sxs-lookup"><span data-stu-id="d2354-134">type</span></span>|<span data-ttu-id="d2354-135">String</span><span class="sxs-lookup"><span data-stu-id="d2354-135">String</span></span>|<span data-ttu-id="d2354-136">Representa o o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d2354-136">Represents the the type of the operation on the role assignment.</span></span> <span data-ttu-id="d2354-137">O valor pode ser `AdminAdd`: administradores adicionar usuários às funções; `UserAdd`: Os usuários adicionar atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="d2354-137">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="d2354-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2354-138">Required.</span></span>|
|<span data-ttu-id="d2354-139">assignmentState</span><span class="sxs-lookup"><span data-stu-id="d2354-139">assignmentState</span></span>|<span data-ttu-id="d2354-140">String</span><span class="sxs-lookup"><span data-stu-id="d2354-140">String</span></span>|<span data-ttu-id="d2354-141">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="d2354-141">The state of the assignment.</span></span> <span data-ttu-id="d2354-142">O valor pode ser `Eligible` para atribuição elegível `Active` - se ele é atribuído diretamente `Active` pelos administradores, ou ativado em uma atribuição elegível pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="d2354-142">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="d2354-143">Os valores possíveis são: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="d2354-143">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="d2354-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2354-144">Required.</span></span>|
|<span data-ttu-id="d2354-145">motivo</span><span class="sxs-lookup"><span data-stu-id="d2354-145">reason</span></span>|<span data-ttu-id="d2354-146">String</span><span class="sxs-lookup"><span data-stu-id="d2354-146">String</span></span>|<span data-ttu-id="d2354-147">O motivo pelo qual deve ser fornecido para a solicitação de atribuição de função de auditoria e revise finalidade.</span><span class="sxs-lookup"><span data-stu-id="d2354-147">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="d2354-148">agenda</span><span class="sxs-lookup"><span data-stu-id="d2354-148">schedule</span></span>|[<span data-ttu-id="d2354-149">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="d2354-149">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="d2354-150">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d2354-150">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="d2354-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2354-151">Response</span></span>
<span data-ttu-id="d2354-152">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2354-152">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="d2354-153">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="d2354-153">Error codes</span></span>
<span data-ttu-id="d2354-154">Essa API retorna esse padrão códigos de erro HTTP.</span><span class="sxs-lookup"><span data-stu-id="d2354-154">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="d2354-155">Além disso, ele pode retornar os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="d2354-155">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="d2354-156">Código de erro</span><span class="sxs-lookup"><span data-stu-id="d2354-156">Error code</span></span>     | <span data-ttu-id="d2354-157">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="d2354-157">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="d2354-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d2354-158">400 BadRequest</span></span> | <span data-ttu-id="d2354-159">Propriedade RoleAssignmentRequest foi NULL</span><span class="sxs-lookup"><span data-stu-id="d2354-159">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="d2354-160">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d2354-160">400 BadRequest</span></span> | <span data-ttu-id="d2354-161">Não é possível desserializar roleAssignmentRequest objeto.</span><span class="sxs-lookup"><span data-stu-id="d2354-161">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="d2354-162">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d2354-162">400 BadRequest</span></span> | <span data-ttu-id="d2354-163">RoleId é necessário.</span><span class="sxs-lookup"><span data-stu-id="d2354-163">RoleId is required.</span></span> |
| <span data-ttu-id="d2354-164">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d2354-164">400 BadRequest</span></span> | <span data-ttu-id="d2354-165">Data de início de agendamento deve ser especificada e deve ser maior do que agora.</span><span class="sxs-lookup"><span data-stu-id="d2354-165">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="d2354-166">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d2354-166">400 BadRequest</span></span> | <span data-ttu-id="d2354-167">Já existe um agendamento para esse tipo de usuário, a função e a agenda.</span><span class="sxs-lookup"><span data-stu-id="d2354-167">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="d2354-168">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d2354-168">400 BadRequest</span></span> | <span data-ttu-id="d2354-169">Uma aprovação pendente já existe para esse tipo de usuário, função e aprovação.</span><span class="sxs-lookup"><span data-stu-id="d2354-169">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="d2354-170">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d2354-170">400 BadRequest</span></span> | <span data-ttu-id="d2354-171">Motivo solicitante está faltando.</span><span class="sxs-lookup"><span data-stu-id="d2354-171">Requestor reason is missing.</span></span> |
| <span data-ttu-id="d2354-172">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d2354-172">400 BadRequest</span></span> | <span data-ttu-id="d2354-173">Motivo solicitante deve ser menor do que 500 caracteres.</span><span class="sxs-lookup"><span data-stu-id="d2354-173">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="d2354-174">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d2354-174">400 BadRequest</span></span> | <span data-ttu-id="d2354-175">Duração de elevação deve estar entre 0,5 e {de configuração}.</span><span class="sxs-lookup"><span data-stu-id="d2354-175">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="d2354-176">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d2354-176">400 BadRequest</span></span> | <span data-ttu-id="d2354-177">Não há uma sobreposição entre a ativação agendada e a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2354-177">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="d2354-178">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d2354-178">400 BadRequest</span></span> | <span data-ttu-id="d2354-179">A função já está ativada.</span><span class="sxs-lookup"><span data-stu-id="d2354-179">The role is already activated.</span></span> |
| <span data-ttu-id="d2354-180">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d2354-180">400 BadRequest</span></span> | <span data-ttu-id="d2354-181">GenericElevateUserToRoleAssignments: Tickting informações é necessário e não são fornecidas no processo de ativação.</span><span class="sxs-lookup"><span data-stu-id="d2354-181">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="d2354-182">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d2354-182">400 BadRequest</span></span> | <span data-ttu-id="d2354-183">Não há uma sobreposição entre a ativação agendada e a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2354-183">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="d2354-184">403 não autorizado</span><span class="sxs-lookup"><span data-stu-id="d2354-184">403 UnAuthorized</span></span> | <span data-ttu-id="d2354-185">Elevação exige a autenticação multifator.</span><span class="sxs-lookup"><span data-stu-id="d2354-185">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="d2354-186">403 não autorizado</span><span class="sxs-lookup"><span data-stu-id="d2354-186">403 UnAuthorized</span></span> | <span data-ttu-id="d2354-187">Em nome de elevação não é permitida.</span><span class="sxs-lookup"><span data-stu-id="d2354-187">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="d2354-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2354-188">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2354-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2354-189">Request</span></span>
<span data-ttu-id="d2354-190">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2354-190">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="d2354-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2354-191">Response</span></span>
<span data-ttu-id="d2354-192">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d2354-192">The following is an example of the response.</span></span> <span data-ttu-id="d2354-193">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="d2354-193">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d2354-194">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2354-194">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
