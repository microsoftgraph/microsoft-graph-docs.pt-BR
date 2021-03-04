---
title: Criar privilegedRoleAssignmentRequest
description: Crie um objeto privilegedroleassignmentrequest.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8899aa70125809f73e2f247a8cf5b83cad0c7731
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441141"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="2c947-103">Criar privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2c947-103">Create privilegedRoleAssignmentRequest</span></span>

<span data-ttu-id="2c947-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c947-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c947-105">Crie um [objeto privilegedroleassignmentrequest.](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="2c947-105">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c947-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c947-106">Permissions</span></span>
<span data-ttu-id="2c947-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c947-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c947-109">Permission type</span></span>                        | <span data-ttu-id="2c947-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c947-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c947-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c947-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2c947-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c947-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2c947-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c947-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c947-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c947-114">Not supported.</span></span> |
|<span data-ttu-id="2c947-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c947-115">Application</span></span>                            | <span data-ttu-id="2c947-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c947-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c947-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c947-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="2c947-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c947-118">Request headers</span></span>
| <span data-ttu-id="2c947-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2c947-119">Name</span></span>      |<span data-ttu-id="2c947-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c947-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2c947-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c947-121">Authorization</span></span>  | <span data-ttu-id="2c947-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c947-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c947-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c947-124">Request body</span></span>
<span data-ttu-id="2c947-125">No corpo da solicitação, fornece uma representação JSON [do objeto privilegedroleassignmentrequest.](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="2c947-125">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="2c947-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c947-126">Property</span></span>     | <span data-ttu-id="2c947-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c947-127">Type</span></span>    |  <span data-ttu-id="2c947-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c947-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c947-129">roleId</span><span class="sxs-lookup"><span data-stu-id="2c947-129">roleId</span></span>|<span data-ttu-id="2c947-130">String</span><span class="sxs-lookup"><span data-stu-id="2c947-130">String</span></span>|<span data-ttu-id="2c947-131">A ID da função.</span><span class="sxs-lookup"><span data-stu-id="2c947-131">The ID of the role.</span></span> <span data-ttu-id="2c947-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c947-132">Required.</span></span>|
|<span data-ttu-id="2c947-133">type</span><span class="sxs-lookup"><span data-stu-id="2c947-133">type</span></span>|<span data-ttu-id="2c947-134">String</span><span class="sxs-lookup"><span data-stu-id="2c947-134">String</span></span>|<span data-ttu-id="2c947-135">Representa o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="2c947-135">Represents the type of the operation on the role assignment.</span></span> <span data-ttu-id="2c947-136">O valor pode ser `AdminAdd` : Administradores adicionam usuários a funções; `UserAdd` : Os usuários adicionam atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="2c947-136">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="2c947-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c947-137">Required.</span></span>|
|<span data-ttu-id="2c947-138">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2c947-138">assignmentState</span></span>|<span data-ttu-id="2c947-139">String</span><span class="sxs-lookup"><span data-stu-id="2c947-139">String</span></span>|<span data-ttu-id="2c947-140">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="2c947-140">The state of the assignment.</span></span> <span data-ttu-id="2c947-141">O valor pode ser para atribuição qualificada - se ele for atribuído diretamente pelos administradores ou ativado em uma atribuição qualificada `Eligible` `Active` pelos `Active` usuários.</span><span class="sxs-lookup"><span data-stu-id="2c947-141">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="2c947-142">Os valores possíveis são: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="2c947-142">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="2c947-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c947-143">Required.</span></span>|
|<span data-ttu-id="2c947-144">motivo</span><span class="sxs-lookup"><span data-stu-id="2c947-144">reason</span></span>|<span data-ttu-id="2c947-145">String</span><span class="sxs-lookup"><span data-stu-id="2c947-145">String</span></span>|<span data-ttu-id="2c947-146">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e revisão.</span><span class="sxs-lookup"><span data-stu-id="2c947-146">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="2c947-147">Cronograma</span><span class="sxs-lookup"><span data-stu-id="2c947-147">schedule</span></span>|[<span data-ttu-id="2c947-148">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2c947-148">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="2c947-149">O cronograma da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="2c947-149">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="2c947-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c947-150">Response</span></span>
<span data-ttu-id="2c947-151">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c947-151">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="2c947-152">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="2c947-152">Error codes</span></span>
<span data-ttu-id="2c947-153">Esta API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="2c947-153">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="2c947-154">Além disso, ele pode retornar os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="2c947-154">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="2c947-155">Código de erro</span><span class="sxs-lookup"><span data-stu-id="2c947-155">Error code</span></span>     | <span data-ttu-id="2c947-156">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="2c947-156">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="2c947-157">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2c947-157">400 BadRequest</span></span> | <span data-ttu-id="2c947-158">A propriedade RoleAssignmentRequest foi NULL</span><span class="sxs-lookup"><span data-stu-id="2c947-158">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="2c947-159">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2c947-159">400 BadRequest</span></span> | <span data-ttu-id="2c947-160">Não é possível deserializar o objeto roleAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="2c947-160">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="2c947-161">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2c947-161">400 BadRequest</span></span> | <span data-ttu-id="2c947-162">RoleId é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c947-162">RoleId is required.</span></span> |
| <span data-ttu-id="2c947-163">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2c947-163">400 BadRequest</span></span> | <span data-ttu-id="2c947-164">A data de início do agendamento deve ser especificada e deve ser maior do que Agora.</span><span class="sxs-lookup"><span data-stu-id="2c947-164">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="2c947-165">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2c947-165">400 BadRequest</span></span> | <span data-ttu-id="2c947-166">Já existe uma agenda para esse usuário, função e tipo de agendamento.</span><span class="sxs-lookup"><span data-stu-id="2c947-166">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="2c947-167">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2c947-167">400 BadRequest</span></span> | <span data-ttu-id="2c947-168">Já existe uma aprovação pendente para esse usuário, função e tipo de aprovação.</span><span class="sxs-lookup"><span data-stu-id="2c947-168">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="2c947-169">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2c947-169">400 BadRequest</span></span> | <span data-ttu-id="2c947-170">O motivo do solicitante está ausente.</span><span class="sxs-lookup"><span data-stu-id="2c947-170">Requestor reason is missing.</span></span> |
| <span data-ttu-id="2c947-171">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2c947-171">400 BadRequest</span></span> | <span data-ttu-id="2c947-172">O motivo do solicitante deve ter menos de 500 caracteres.</span><span class="sxs-lookup"><span data-stu-id="2c947-172">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="2c947-173">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2c947-173">400 BadRequest</span></span> | <span data-ttu-id="2c947-174">A duração da elevação deve estar entre 0,5 e {from setting}.</span><span class="sxs-lookup"><span data-stu-id="2c947-174">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="2c947-175">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2c947-175">400 BadRequest</span></span> | <span data-ttu-id="2c947-176">Há uma sobreposição entre a ativação agendada e a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c947-176">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="2c947-177">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2c947-177">400 BadRequest</span></span> | <span data-ttu-id="2c947-178">A função já está ativada.</span><span class="sxs-lookup"><span data-stu-id="2c947-178">The role is already activated.</span></span> |
| <span data-ttu-id="2c947-179">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2c947-179">400 BadRequest</span></span> | <span data-ttu-id="2c947-180">GenericElevateUserToRoleAssignments: As informações de escala são necessárias e não são fornecidas no processo de ativação.</span><span class="sxs-lookup"><span data-stu-id="2c947-180">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="2c947-181">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2c947-181">400 BadRequest</span></span> | <span data-ttu-id="2c947-182">Há uma sobreposição entre a ativação agendada e a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c947-182">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="2c947-183">403 Não Autorizado</span><span class="sxs-lookup"><span data-stu-id="2c947-183">403 UnAuthorized</span></span> | <span data-ttu-id="2c947-184">A elevação requer Autenticação Multifa factor.</span><span class="sxs-lookup"><span data-stu-id="2c947-184">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="2c947-185">403 Não Autorizado</span><span class="sxs-lookup"><span data-stu-id="2c947-185">403 UnAuthorized</span></span> | <span data-ttu-id="2c947-186">Em nome da elevação não é permitido.</span><span class="sxs-lookup"><span data-stu-id="2c947-186">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="2c947-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c947-187">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c947-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c947-188">Request</span></span>
<span data-ttu-id="2c947-189">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c947-189">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c947-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c947-190">HTTP</span></span>](#tab/http)
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
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
# <a name="c"></a>[<span data-ttu-id="2c947-191">C#</span><span class="sxs-lookup"><span data-stu-id="2c947-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c947-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c947-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c947-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c947-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c947-194">Java</span><span class="sxs-lookup"><span data-stu-id="2c947-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-privilegedroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2c947-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c947-195">Response</span></span>
<span data-ttu-id="2c947-196">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2c947-196">The following is an example of the response.</span></span> <span data-ttu-id="2c947-197">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="2c947-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2c947-198">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c947-198">All of the properties will be returned from an actual call.</span></span>
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


