---
title: Criar unifiedRoleAssignmentScheduleRequest
description: Crie um novo objeto unifiedRoleAssignmentScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a487a8cba0d5f14906eafea5fe0844d419709853
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334343"
---
# <a name="create-unifiedroleassignmentschedulerequest"></a><span data-ttu-id="22320-103">Criar unifiedRoleAssignmentScheduleRequest</span><span class="sxs-lookup"><span data-stu-id="22320-103">Create unifiedRoleAssignmentScheduleRequest</span></span>
<span data-ttu-id="22320-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22320-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22320-105">Crie um novo [objeto unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="22320-105">Create a new [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22320-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="22320-106">Permissions</span></span>
<span data-ttu-id="22320-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22320-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22320-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22320-109">Permission type</span></span>|<span data-ttu-id="22320-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22320-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22320-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22320-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22320-112">RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="22320-112">RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="22320-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22320-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22320-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="22320-114">Not supported</span></span>|
|<span data-ttu-id="22320-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22320-115">Application</span></span>|<span data-ttu-id="22320-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="22320-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="22320-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22320-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleAssignmentScheduleRequests
```

## <a name="request-headers"></a><span data-ttu-id="22320-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22320-118">Request headers</span></span>
|<span data-ttu-id="22320-119">Nome</span><span class="sxs-lookup"><span data-stu-id="22320-119">Name</span></span>|<span data-ttu-id="22320-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="22320-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="22320-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="22320-121">Authorization</span></span>|<span data-ttu-id="22320-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22320-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="22320-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="22320-124">Content-Type</span></span>|<span data-ttu-id="22320-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22320-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22320-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22320-127">Request body</span></span>
<span data-ttu-id="22320-128">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="22320-128">In the request body, supply a JSON representation of the [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object.</span></span>

<span data-ttu-id="22320-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md).</span><span class="sxs-lookup"><span data-stu-id="22320-129">The following table shows the properties that are required when you create the [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md).</span></span>

|<span data-ttu-id="22320-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22320-130">Property</span></span>|<span data-ttu-id="22320-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="22320-131">Type</span></span>|<span data-ttu-id="22320-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="22320-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22320-133">id</span><span class="sxs-lookup"><span data-stu-id="22320-133">id</span></span>|<span data-ttu-id="22320-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22320-134">String</span></span>|<span data-ttu-id="22320-135">O identificador exclusivo para unifiedRoleAssignmentScheduleRequest.</span><span class="sxs-lookup"><span data-stu-id="22320-135">The unique identifier for the unifiedRoleAssignmentScheduleRequest.</span></span> <span data-ttu-id="22320-136">Chave, não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22320-136">Key, not nullable, Read-only.</span></span>|
|<span data-ttu-id="22320-137">ação</span><span class="sxs-lookup"><span data-stu-id="22320-137">action</span></span>|<span data-ttu-id="22320-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22320-138">String</span></span>|<span data-ttu-id="22320-139">Representando o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="22320-139">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="22320-140">O valor pode ser</span><span class="sxs-lookup"><span data-stu-id="22320-140">The value can be</span></span> <ul><li><span data-ttu-id="22320-141">`AdminAdd`: Os administradores atribuem usuários/grupos a funções;</span><span class="sxs-lookup"><span data-stu-id="22320-141">`AdminAdd`: Administrators assign users/groups to roles;</span></span></li><li><span data-ttu-id="22320-142">`UserAdd`: Os usuários ativam atribuições qualificadas;</span><span class="sxs-lookup"><span data-stu-id="22320-142">`UserAdd`: Users activate eligible assignments;</span></span></li><li> <span data-ttu-id="22320-143">`AdminUpdate`: Os administradores alteram as atribuições de função existentes</span><span class="sxs-lookup"><span data-stu-id="22320-143">`AdminUpdate`: Administrators change existing role assignments</span></span></li><li><span data-ttu-id="22320-144">`AdminRemove`: Os administradores removem usuários/grupos de funções;</span><span class="sxs-lookup"><span data-stu-id="22320-144">`AdminRemove`: Administrators remove users/groups from roles;</span></span><li><span data-ttu-id="22320-145">`UserRemove`: Os usuários desativam as atribuições ativas;</span><span class="sxs-lookup"><span data-stu-id="22320-145">`UserRemove`: Users deactivate active assignments;</span></span><li><span data-ttu-id="22320-146">`UserExtend`: Os usuários solicitam estender suas atribuições de expiração;</span><span class="sxs-lookup"><span data-stu-id="22320-146">`UserExtend`: Users request to extend their expiring assignments;</span></span></li><li><span data-ttu-id="22320-147">`AdminExtend`: Os administradores estendem atribuições expiradas.</span><span class="sxs-lookup"><span data-stu-id="22320-147">`AdminExtend`: Administrators extend expiring assignments.</span></span></li><li><span data-ttu-id="22320-148">`UserRenew`: Os usuários solicitam a renovação de suas atribuições expiradas;</span><span class="sxs-lookup"><span data-stu-id="22320-148">`UserRenew`: Users request to renew their expired assignments;</span></span></li><li><span data-ttu-id="22320-149">`AdminRenew`: Os administradores estendem atribuições expiradas.</span><span class="sxs-lookup"><span data-stu-id="22320-149">`AdminRenew`: Administrators extend expiring assignments.</span></span></li></ul>|
|<span data-ttu-id="22320-150">principalId</span><span class="sxs-lookup"><span data-stu-id="22320-150">principalId</span></span>|<span data-ttu-id="22320-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22320-151">String</span></span>|<span data-ttu-id="22320-152">Objectid da entidade à qual a atribuição está sendo concedida.</span><span class="sxs-lookup"><span data-stu-id="22320-152">Objectid of the principal to which the assignment is being granted to.</span></span>|
|<span data-ttu-id="22320-153">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="22320-153">roleDefinitionId</span></span>|<span data-ttu-id="22320-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22320-154">String</span></span>|<span data-ttu-id="22320-155">ID do unifiedRoleDefinition para o que a atribuição se destina.</span><span class="sxs-lookup"><span data-stu-id="22320-155">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="22320-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22320-156">Read only.</span></span>|
|<span data-ttu-id="22320-157">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="22320-157">directoryScopeId</span></span>|<span data-ttu-id="22320-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22320-158">String</span></span>|<span data-ttu-id="22320-159">ID do objeto directory que representa o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="22320-159">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="22320-160">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso.</span><span class="sxs-lookup"><span data-stu-id="22320-160">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="22320-161">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="22320-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="22320-162">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="22320-162">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="22320-163">appScopeId</span><span class="sxs-lookup"><span data-stu-id="22320-163">appScopeId</span></span>|<span data-ttu-id="22320-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22320-164">String</span></span>|<span data-ttu-id="22320-165">ID do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="22320-165">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="22320-166">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso.</span><span class="sxs-lookup"><span data-stu-id="22320-166">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="22320-167">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="22320-167">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="22320-168">Use "/" para o escopo de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="22320-168">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="22320-169">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="22320-169">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="22320-170">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="22320-170">isValidationOnly</span></span>|<span data-ttu-id="22320-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="22320-171">Boolean</span></span>|<span data-ttu-id="22320-172">Um booleano que determina se a chamada é uma validação ou uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22320-172">A boolean that determines whether the call is a validation or an actual call.</span></span> <span data-ttu-id="22320-173">De definir essa propriedade somente se você quiser verificar se uma ativação está sujeita a regras adicionais, como MFA, antes de realmente enviar a solicitação.</span><span class="sxs-lookup"><span data-stu-id="22320-173">Only set this property if you want to check whether an activation is subject to additional rules like MFA before actually submitting the request.</span></span>|
|<span data-ttu-id="22320-174">targetScheduleId</span><span class="sxs-lookup"><span data-stu-id="22320-174">targetScheduleId</span></span>|<span data-ttu-id="22320-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22320-175">String</span></span>|<span data-ttu-id="22320-176">ID do objeto schedule anexado à atribuição.</span><span class="sxs-lookup"><span data-stu-id="22320-176">ID of the schedule object attached to the assignment.</span></span>|
|<span data-ttu-id="22320-177">justification</span><span class="sxs-lookup"><span data-stu-id="22320-177">justification</span></span>|<span data-ttu-id="22320-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22320-178">String</span></span>|<span data-ttu-id="22320-179">Uma mensagem fornecida por usuários e administradores ao criar a solicitação sobre por que ela é necessária.</span><span class="sxs-lookup"><span data-stu-id="22320-179">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="22320-180">scheduleInfo</span><span class="sxs-lookup"><span data-stu-id="22320-180">scheduleInfo</span></span>|[<span data-ttu-id="22320-181">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="22320-181">requestSchedule</span></span>](../resources/requestschedule.md)|<span data-ttu-id="22320-182">O objeto schedule da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="22320-182">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="22320-183">ticketInfo</span><span class="sxs-lookup"><span data-stu-id="22320-183">ticketInfo</span></span>|[<span data-ttu-id="22320-184">ticketInfo</span><span class="sxs-lookup"><span data-stu-id="22320-184">ticketInfo</span></span>](../resources/ticketinfo.md)|<span data-ttu-id="22320-185">O objeto ticketInfo anexado à solicitação de atribuição de função que inclui detalhes do número do tíquete e do sistema de tíquetes.</span><span class="sxs-lookup"><span data-stu-id="22320-185">The ticketInfo object attached to the role assignment request which includes details of the ticket number and ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="22320-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="22320-186">Response</span></span>

<span data-ttu-id="22320-187">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22320-187">If successful, this method returns a `201 Created` response code and an [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22320-188">Exemplos</span><span class="sxs-lookup"><span data-stu-id="22320-188">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22320-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22320-189">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="22320-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="22320-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentschedulerequest_from_unifiedroleassignmentschedulerequests"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/
Content-Type: application/json
Content-length: 510

{
  "@odata.type": "#Microsoft.Identity.Governance.Common.Data.ExternalModels.V1.unifiedRoleAssignmentScheduleRequest",
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="22320-191">C#</span><span class="sxs-lookup"><span data-stu-id="22320-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22320-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22320-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22320-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22320-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22320-194">Java</span><span class="sxs-lookup"><span data-stu-id="22320-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="22320-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="22320-195">Response</span></span>
<span data-ttu-id="22320-196">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="22320-196">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "c13ee236-e236-c13e-36e2-3ec136e23ec1",
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```

