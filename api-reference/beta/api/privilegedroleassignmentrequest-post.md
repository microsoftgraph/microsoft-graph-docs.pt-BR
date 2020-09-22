---
title: Criar privilegedRoleAssignmentRequest
description: Criar um objeto privilegedroleassignmentrequest.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 0184824c47bc13120122df15b4c2473e0ad3cb12
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034932"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="98146-103">Criar privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="98146-103">Create privilegedRoleAssignmentRequest</span></span>

<span data-ttu-id="98146-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98146-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98146-105">Criar um objeto [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="98146-105">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="98146-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="98146-106">Permissions</span></span>
<span data-ttu-id="98146-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98146-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98146-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98146-109">Permission type</span></span>                        | <span data-ttu-id="98146-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98146-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="98146-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98146-111">Delegated (work or school account)</span></span> | <span data-ttu-id="98146-112">PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="98146-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="98146-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98146-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98146-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98146-114">Not supported.</span></span> |
|<span data-ttu-id="98146-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98146-115">Application</span></span>                            | <span data-ttu-id="98146-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98146-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98146-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98146-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="98146-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98146-118">Request headers</span></span>
| <span data-ttu-id="98146-119">Nome</span><span class="sxs-lookup"><span data-stu-id="98146-119">Name</span></span>      |<span data-ttu-id="98146-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="98146-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="98146-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="98146-121">Authorization</span></span>  | <span data-ttu-id="98146-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98146-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98146-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98146-124">Request body</span></span>
<span data-ttu-id="98146-125">No corpo da solicitação, forneça uma representação JSON do objeto [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="98146-125">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="98146-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98146-126">Property</span></span>     | <span data-ttu-id="98146-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="98146-127">Type</span></span>    |  <span data-ttu-id="98146-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="98146-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98146-129">roleId</span><span class="sxs-lookup"><span data-stu-id="98146-129">roleId</span></span>|<span data-ttu-id="98146-130">String</span><span class="sxs-lookup"><span data-stu-id="98146-130">String</span></span>|<span data-ttu-id="98146-131">A ID da função.</span><span class="sxs-lookup"><span data-stu-id="98146-131">The ID of the role.</span></span> <span data-ttu-id="98146-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98146-132">Required.</span></span>|
|<span data-ttu-id="98146-133">tipo</span><span class="sxs-lookup"><span data-stu-id="98146-133">type</span></span>|<span data-ttu-id="98146-134">String</span><span class="sxs-lookup"><span data-stu-id="98146-134">String</span></span>|<span data-ttu-id="98146-135">Representa o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="98146-135">Represents the type of the operation on the role assignment.</span></span> <span data-ttu-id="98146-136">O valor pode ser `AdminAdd` : os administradores adicionam usuários a funções; `UserAdd` : os usuários adicionam atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="98146-136">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="98146-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98146-137">Required.</span></span>|
|<span data-ttu-id="98146-138">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="98146-138">assignmentState</span></span>|<span data-ttu-id="98146-139">String</span><span class="sxs-lookup"><span data-stu-id="98146-139">String</span></span>|<span data-ttu-id="98146-140">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="98146-140">The state of the assignment.</span></span> <span data-ttu-id="98146-141">O valor pode ser `Eligible` para atribuição qualificada `Active` -se for diretamente atribuído `Active` por administradores ou ativado em uma atribuição qualificada pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="98146-141">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="98146-142">Os valores possíveis são: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="98146-142">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="98146-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98146-143">Required.</span></span>|
|<span data-ttu-id="98146-144">motivo</span><span class="sxs-lookup"><span data-stu-id="98146-144">reason</span></span>|<span data-ttu-id="98146-145">String</span><span class="sxs-lookup"><span data-stu-id="98146-145">String</span></span>|<span data-ttu-id="98146-146">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e análise.</span><span class="sxs-lookup"><span data-stu-id="98146-146">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="98146-147">Cronograma</span><span class="sxs-lookup"><span data-stu-id="98146-147">schedule</span></span>|[<span data-ttu-id="98146-148">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="98146-148">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="98146-149">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="98146-149">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="98146-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="98146-150">Response</span></span>
<span data-ttu-id="98146-151">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98146-151">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="98146-152">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="98146-152">Error codes</span></span>
<span data-ttu-id="98146-153">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="98146-153">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="98146-154">Além disso, ele pode retornar os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="98146-154">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="98146-155">Código de erro</span><span class="sxs-lookup"><span data-stu-id="98146-155">Error code</span></span>     | <span data-ttu-id="98146-156">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="98146-156">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="98146-157">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="98146-157">400 BadRequest</span></span> | <span data-ttu-id="98146-158">Propriedade RoleAssignmentRequest era nula</span><span class="sxs-lookup"><span data-stu-id="98146-158">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="98146-159">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="98146-159">400 BadRequest</span></span> | <span data-ttu-id="98146-160">Não é possível desserializar o objeto roleAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="98146-160">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="98146-161">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="98146-161">400 BadRequest</span></span> | <span data-ttu-id="98146-162">RoleID é necessário.</span><span class="sxs-lookup"><span data-stu-id="98146-162">RoleId is required.</span></span> |
| <span data-ttu-id="98146-163">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="98146-163">400 BadRequest</span></span> | <span data-ttu-id="98146-164">A data de início agendada deve ser especificada e deve ser maior do que agora.</span><span class="sxs-lookup"><span data-stu-id="98146-164">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="98146-165">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="98146-165">400 BadRequest</span></span> | <span data-ttu-id="98146-166">Já existe um cronograma para este usuário, função e tipo de agendamento.</span><span class="sxs-lookup"><span data-stu-id="98146-166">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="98146-167">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="98146-167">400 BadRequest</span></span> | <span data-ttu-id="98146-168">Já existe uma aprovação pendente para este usuário, função e tipo de aprovação.</span><span class="sxs-lookup"><span data-stu-id="98146-168">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="98146-169">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="98146-169">400 BadRequest</span></span> | <span data-ttu-id="98146-170">Razão do solicitante ausente.</span><span class="sxs-lookup"><span data-stu-id="98146-170">Requestor reason is missing.</span></span> |
| <span data-ttu-id="98146-171">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="98146-171">400 BadRequest</span></span> | <span data-ttu-id="98146-172">O motivo do solicitante deve ser menor que 500 caracteres.</span><span class="sxs-lookup"><span data-stu-id="98146-172">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="98146-173">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="98146-173">400 BadRequest</span></span> | <span data-ttu-id="98146-174">A duração da elevação deve estar entre 0,5 e {from Setting}.</span><span class="sxs-lookup"><span data-stu-id="98146-174">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="98146-175">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="98146-175">400 BadRequest</span></span> | <span data-ttu-id="98146-176">Há uma sobreposição entre ativação agendada e a solicitação.</span><span class="sxs-lookup"><span data-stu-id="98146-176">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="98146-177">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="98146-177">400 BadRequest</span></span> | <span data-ttu-id="98146-178">A função já está ativada.</span><span class="sxs-lookup"><span data-stu-id="98146-178">The role is already activated.</span></span> |
| <span data-ttu-id="98146-179">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="98146-179">400 BadRequest</span></span> | <span data-ttu-id="98146-180">GenericElevateUserToRoleAssignments: as informações de Tickting são necessárias e não são fornecidas no processo de ativação.</span><span class="sxs-lookup"><span data-stu-id="98146-180">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="98146-181">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="98146-181">400 BadRequest</span></span> | <span data-ttu-id="98146-182">Há uma sobreposição entre ativação agendada e a solicitação.</span><span class="sxs-lookup"><span data-stu-id="98146-182">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="98146-183">403 não autorizado</span><span class="sxs-lookup"><span data-stu-id="98146-183">403 UnAuthorized</span></span> | <span data-ttu-id="98146-184">A elevação requer autenticação multifator.</span><span class="sxs-lookup"><span data-stu-id="98146-184">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="98146-185">403 não autorizado</span><span class="sxs-lookup"><span data-stu-id="98146-185">403 UnAuthorized</span></span> | <span data-ttu-id="98146-186">Em nome da elevação não é permitida.</span><span class="sxs-lookup"><span data-stu-id="98146-186">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="98146-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98146-187">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98146-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98146-188">Request</span></span>
<span data-ttu-id="98146-189">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="98146-189">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="98146-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="98146-190">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="98146-191">C#</span><span class="sxs-lookup"><span data-stu-id="98146-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98146-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98146-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98146-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98146-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="98146-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="98146-194">Response</span></span>
<span data-ttu-id="98146-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="98146-195">The following is an example of the response.</span></span> <span data-ttu-id="98146-196">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="98146-196">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="98146-197">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98146-197">All of the properties will be returned from an actual call.</span></span>
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
    "userId": "Self",
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
  ]
}
-->


