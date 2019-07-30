---
title: Criar privilegedRoleAssignmentRequest
description: Criar um objeto privilegedroleassignmentrequest.
localization_priority: Normal
ms.openlocfilehash: 0cb7e958e9eaf8550d1262ed00e66ee477cbd195
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931848"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="50887-103">Criar privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="50887-103">Create privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50887-104">Criar um objeto [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="50887-104">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="50887-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="50887-105">Permissions</span></span>
<span data-ttu-id="50887-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50887-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50887-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50887-108">Permission type</span></span>                        | <span data-ttu-id="50887-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50887-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="50887-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50887-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50887-111">PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="50887-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="50887-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50887-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50887-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50887-113">Not supported.</span></span> |
|<span data-ttu-id="50887-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50887-114">Application</span></span>                            | <span data-ttu-id="50887-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50887-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="50887-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50887-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="50887-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50887-117">Request headers</span></span>
| <span data-ttu-id="50887-118">Nome</span><span class="sxs-lookup"><span data-stu-id="50887-118">Name</span></span>      |<span data-ttu-id="50887-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="50887-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="50887-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="50887-120">Authorization</span></span>  | <span data-ttu-id="50887-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50887-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50887-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50887-123">Request body</span></span>
<span data-ttu-id="50887-124">No corpo da solicitação, forneça uma representação JSON do objeto [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="50887-124">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="50887-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50887-125">Property</span></span>     | <span data-ttu-id="50887-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="50887-126">Type</span></span>    |  <span data-ttu-id="50887-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="50887-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50887-128">roleId</span><span class="sxs-lookup"><span data-stu-id="50887-128">roleId</span></span>|<span data-ttu-id="50887-129">String</span><span class="sxs-lookup"><span data-stu-id="50887-129">String</span></span>|<span data-ttu-id="50887-130">A ID da função.</span><span class="sxs-lookup"><span data-stu-id="50887-130">The ID of the role.</span></span> <span data-ttu-id="50887-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50887-131">Required.</span></span>|
|<span data-ttu-id="50887-132">type</span><span class="sxs-lookup"><span data-stu-id="50887-132">type</span></span>|<span data-ttu-id="50887-133">String</span><span class="sxs-lookup"><span data-stu-id="50887-133">String</span></span>|<span data-ttu-id="50887-134">Representa o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="50887-134">Represents the type of the operation on the role assignment.</span></span> <span data-ttu-id="50887-135">O valor pode ser `AdminAdd`: os administradores adicionam usuários a funções; `UserAdd`: Os usuários adicionam atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="50887-135">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="50887-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50887-136">Required.</span></span>|
|<span data-ttu-id="50887-137">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="50887-137">assignmentState</span></span>|<span data-ttu-id="50887-138">String</span><span class="sxs-lookup"><span data-stu-id="50887-138">String</span></span>|<span data-ttu-id="50887-139">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="50887-139">The state of the assignment.</span></span> <span data-ttu-id="50887-140">O valor pode ser `Eligible` para atribuição `Active` qualificada-se for diretamente atribuído `Active` por administradores ou ativado em uma atribuição qualificada pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="50887-140">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="50887-141">Os valores possíveis são: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="50887-141">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="50887-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50887-142">Required.</span></span>|
|<span data-ttu-id="50887-143">motivos</span><span class="sxs-lookup"><span data-stu-id="50887-143">reason</span></span>|<span data-ttu-id="50887-144">String</span><span class="sxs-lookup"><span data-stu-id="50887-144">String</span></span>|<span data-ttu-id="50887-145">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e análise.</span><span class="sxs-lookup"><span data-stu-id="50887-145">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="50887-146">Cronograma</span><span class="sxs-lookup"><span data-stu-id="50887-146">schedule</span></span>|[<span data-ttu-id="50887-147">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="50887-147">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="50887-148">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="50887-148">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="50887-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="50887-149">Response</span></span>
<span data-ttu-id="50887-150">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50887-150">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="50887-151">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="50887-151">Error codes</span></span>
<span data-ttu-id="50887-152">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="50887-152">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="50887-153">Além disso, ele pode retornar os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="50887-153">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="50887-154">Código de erro</span><span class="sxs-lookup"><span data-stu-id="50887-154">Error code</span></span>     | <span data-ttu-id="50887-155">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="50887-155">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="50887-156">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="50887-156">400 BadRequest</span></span> | <span data-ttu-id="50887-157">Propriedade RoleAssignmentRequest era nula</span><span class="sxs-lookup"><span data-stu-id="50887-157">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="50887-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="50887-158">400 BadRequest</span></span> | <span data-ttu-id="50887-159">Não é possível desserializar o objeto roleAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="50887-159">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="50887-160">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="50887-160">400 BadRequest</span></span> | <span data-ttu-id="50887-161">RoleID é necessário.</span><span class="sxs-lookup"><span data-stu-id="50887-161">RoleId is required.</span></span> |
| <span data-ttu-id="50887-162">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="50887-162">400 BadRequest</span></span> | <span data-ttu-id="50887-163">A data de início agendada deve ser especificada e deve ser maior do que agora.</span><span class="sxs-lookup"><span data-stu-id="50887-163">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="50887-164">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="50887-164">400 BadRequest</span></span> | <span data-ttu-id="50887-165">Já existe um cronograma para este usuário, função e tipo de agendamento.</span><span class="sxs-lookup"><span data-stu-id="50887-165">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="50887-166">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="50887-166">400 BadRequest</span></span> | <span data-ttu-id="50887-167">Já existe uma aprovação pendente para este usuário, função e tipo de aprovação.</span><span class="sxs-lookup"><span data-stu-id="50887-167">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="50887-168">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="50887-168">400 BadRequest</span></span> | <span data-ttu-id="50887-169">Razão do solicitante ausente.</span><span class="sxs-lookup"><span data-stu-id="50887-169">Requestor reason is missing.</span></span> |
| <span data-ttu-id="50887-170">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="50887-170">400 BadRequest</span></span> | <span data-ttu-id="50887-171">O motivo do solicitante deve ser menor que 500 caracteres.</span><span class="sxs-lookup"><span data-stu-id="50887-171">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="50887-172">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="50887-172">400 BadRequest</span></span> | <span data-ttu-id="50887-173">A duração da elevação deve estar entre 0,5 e {from Setting}.</span><span class="sxs-lookup"><span data-stu-id="50887-173">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="50887-174">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="50887-174">400 BadRequest</span></span> | <span data-ttu-id="50887-175">Há uma sobreposição entre ativação agendada e a solicitação.</span><span class="sxs-lookup"><span data-stu-id="50887-175">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="50887-176">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="50887-176">400 BadRequest</span></span> | <span data-ttu-id="50887-177">A função já está ativada.</span><span class="sxs-lookup"><span data-stu-id="50887-177">The role is already activated.</span></span> |
| <span data-ttu-id="50887-178">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="50887-178">400 BadRequest</span></span> | <span data-ttu-id="50887-179">GenericElevateUserToRoleAssignments: as informações de Tickting são necessárias e não são fornecidas no processo de ativação.</span><span class="sxs-lookup"><span data-stu-id="50887-179">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="50887-180">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="50887-180">400 BadRequest</span></span> | <span data-ttu-id="50887-181">Há uma sobreposição entre ativação agendada e a solicitação.</span><span class="sxs-lookup"><span data-stu-id="50887-181">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="50887-182">403 não autorizado</span><span class="sxs-lookup"><span data-stu-id="50887-182">403 UnAuthorized</span></span> | <span data-ttu-id="50887-183">A elevação requer autenticação multifator.</span><span class="sxs-lookup"><span data-stu-id="50887-183">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="50887-184">403 não autorizado</span><span class="sxs-lookup"><span data-stu-id="50887-184">403 UnAuthorized</span></span> | <span data-ttu-id="50887-185">Em nome da elevação não é permitida.</span><span class="sxs-lookup"><span data-stu-id="50887-185">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="50887-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50887-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50887-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50887-187">Request</span></span>
<span data-ttu-id="50887-188">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="50887-188">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="50887-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="50887-189">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="50887-190">C#</span><span class="sxs-lookup"><span data-stu-id="50887-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50887-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="50887-191">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="50887-192">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="50887-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="50887-193">Java</span><span class="sxs-lookup"><span data-stu-id="50887-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-privilegedroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="50887-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="50887-194">Response</span></span>
<span data-ttu-id="50887-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="50887-195">The following is an example of the response.</span></span> <span data-ttu-id="50887-196">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="50887-196">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="50887-197">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50887-197">All of the properties will be returned from an actual call.</span></span>
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
