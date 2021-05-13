---
title: Criar unifiedRoleEligibilityScheduleRequest
description: Crie um novo objeto unifiedRoleEligibilityScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1316764863bbefc19ed28882f686a2e9ac03e07f
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475198"
---
# <a name="create-unifiedroleeligibilityschedulerequest"></a><span data-ttu-id="65808-103">Criar unifiedRoleEligibilityScheduleRequest</span><span class="sxs-lookup"><span data-stu-id="65808-103">Create unifiedRoleEligibilityScheduleRequest</span></span>
<span data-ttu-id="65808-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65808-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65808-105">Crie um novo [objeto unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="65808-105">Create a new [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="65808-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="65808-106">Permissions</span></span>
<span data-ttu-id="65808-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65808-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65808-109">Permission type</span></span>|<span data-ttu-id="65808-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65808-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65808-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65808-111">Delegated (work or school account)</span></span>|<span data-ttu-id="65808-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="65808-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="65808-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65808-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65808-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="65808-114">Not supported</span></span>|
|<span data-ttu-id="65808-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65808-115">Application</span></span>|<span data-ttu-id="65808-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="65808-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="65808-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65808-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleEligibilityScheduleRequests
```

## <a name="request-headers"></a><span data-ttu-id="65808-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65808-118">Request headers</span></span>
|<span data-ttu-id="65808-119">Nome</span><span class="sxs-lookup"><span data-stu-id="65808-119">Name</span></span>|<span data-ttu-id="65808-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="65808-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="65808-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="65808-121">Authorization</span></span>|<span data-ttu-id="65808-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65808-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="65808-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65808-124">Content-Type</span></span>|<span data-ttu-id="65808-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65808-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65808-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65808-127">Request body</span></span>
<span data-ttu-id="65808-128">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="65808-128">In the request body, supply a JSON representation of the [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object.</span></span>

<span data-ttu-id="65808-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md).</span><span class="sxs-lookup"><span data-stu-id="65808-129">The following table shows the properties that are required when you create the [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md).</span></span>

|<span data-ttu-id="65808-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65808-130">Property</span></span>|<span data-ttu-id="65808-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="65808-131">Type</span></span>|<span data-ttu-id="65808-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="65808-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65808-133">id</span><span class="sxs-lookup"><span data-stu-id="65808-133">id</span></span>|<span data-ttu-id="65808-134">String</span><span class="sxs-lookup"><span data-stu-id="65808-134">String</span></span>|<span data-ttu-id="65808-135">O identificador exclusivo para unifiedRoleEligibilityScheduleRequest.</span><span class="sxs-lookup"><span data-stu-id="65808-135">The unique identifier for the unifiedRoleEligibilityScheduleRequest.</span></span> <span data-ttu-id="65808-136">Chave, não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="65808-136">Key, not nullable, Read-only.</span></span>|
|<span data-ttu-id="65808-137">ação</span><span class="sxs-lookup"><span data-stu-id="65808-137">action</span></span>|<span data-ttu-id="65808-138">String</span><span class="sxs-lookup"><span data-stu-id="65808-138">String</span></span>|<span data-ttu-id="65808-139">Representando o tipo da operação na atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="65808-139">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="65808-140">O valor pode ser</span><span class="sxs-lookup"><span data-stu-id="65808-140">The value can be</span></span> <ul><li><span data-ttu-id="65808-141">`AdminAdd`: Os administradores atribuem usuários/grupos a funções;</span><span class="sxs-lookup"><span data-stu-id="65808-141">`AdminAdd`: Administrators assign users/groups to roles;</span></span></li><li><span data-ttu-id="65808-142">`UserAdd`: Os usuários ativam atribuições qualificadas;</span><span class="sxs-lookup"><span data-stu-id="65808-142">`UserAdd`: Users activate eligible assignments;</span></span></li><li> <span data-ttu-id="65808-143">`AdminUpdate`: Os administradores alteram as atribuições de função existentes</span><span class="sxs-lookup"><span data-stu-id="65808-143">`AdminUpdate`: Administrators change existing role assignments</span></span></li><li><span data-ttu-id="65808-144">`AdminRemove`: Os administradores removem usuários/grupos de funções;</span><span class="sxs-lookup"><span data-stu-id="65808-144">`AdminRemove`: Administrators remove users/groups from roles;</span></span><li><span data-ttu-id="65808-145">`UserRemove`: Os usuários desativam as atribuições ativas;</span><span class="sxs-lookup"><span data-stu-id="65808-145">`UserRemove`: Users deactivate active assignments;</span></span><li><span data-ttu-id="65808-146">`UserExtend`: Os usuários solicitam estender suas atribuições de expiração;</span><span class="sxs-lookup"><span data-stu-id="65808-146">`UserExtend`: Users request to extend their expiring assignments;</span></span></li><li><span data-ttu-id="65808-147">`AdminExtend`: Os administradores estendem atribuições expiradas.</span><span class="sxs-lookup"><span data-stu-id="65808-147">`AdminExtend`: Administrators extend expiring assignments.</span></span></li><li><span data-ttu-id="65808-148">`UserRenew`: Os usuários solicitam a renovação de suas atribuições expiradas;</span><span class="sxs-lookup"><span data-stu-id="65808-148">`UserRenew`: Users request to renew their expired assignments;</span></span></li><li><span data-ttu-id="65808-149">`AdminRenew`: Os administradores estendem atribuições expiradas.</span><span class="sxs-lookup"><span data-stu-id="65808-149">`AdminRenew`: Administrators extend expiring assignments.</span></span></li></ul>|
|<span data-ttu-id="65808-150">principalId</span><span class="sxs-lookup"><span data-stu-id="65808-150">principalId</span></span>|<span data-ttu-id="65808-151">String</span><span class="sxs-lookup"><span data-stu-id="65808-151">String</span></span>|<span data-ttu-id="65808-152">Objectid da entidade à qual a atribuição está sendo concedida.</span><span class="sxs-lookup"><span data-stu-id="65808-152">Objectid of the principal to which the assignment is being granted to.</span></span>|
|<span data-ttu-id="65808-153">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="65808-153">roleDefinitionId</span></span>|<span data-ttu-id="65808-154">String</span><span class="sxs-lookup"><span data-stu-id="65808-154">String</span></span>|<span data-ttu-id="65808-155">ID do unifiedRoleDefinition para o que a atribuição se destina.</span><span class="sxs-lookup"><span data-stu-id="65808-155">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="65808-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="65808-156">Read only.</span></span>|
|<span data-ttu-id="65808-157">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="65808-157">directoryScopeId</span></span>|<span data-ttu-id="65808-158">String</span><span class="sxs-lookup"><span data-stu-id="65808-158">String</span></span>|<span data-ttu-id="65808-159">ID do objeto directory que representa o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="65808-159">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="65808-160">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso.</span><span class="sxs-lookup"><span data-stu-id="65808-160">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="65808-161">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="65808-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="65808-162">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="65808-162">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="65808-163">appScopeId</span><span class="sxs-lookup"><span data-stu-id="65808-163">appScopeId</span></span>|<span data-ttu-id="65808-164">String</span><span class="sxs-lookup"><span data-stu-id="65808-164">String</span></span>|<span data-ttu-id="65808-165">ID do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="65808-165">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="65808-166">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso.</span><span class="sxs-lookup"><span data-stu-id="65808-166">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="65808-167">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="65808-167">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="65808-168">Use "/" para o escopo de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="65808-168">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="65808-169">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="65808-169">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="65808-170">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="65808-170">isValidationOnly</span></span>|<span data-ttu-id="65808-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="65808-171">Boolean</span></span>|<span data-ttu-id="65808-172">Um booleano que determina se a chamada é uma validação ou uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65808-172">A boolean that determines whether the call is a validation or an actual call.</span></span> <span data-ttu-id="65808-173">De definir essa propriedade somente se você quiser verificar se uma ativação está sujeita a regras adicionais, como MFA, antes de realmente enviar a solicitação.</span><span class="sxs-lookup"><span data-stu-id="65808-173">Only set this property if you want to check whether an activation is subject to additional rules like MFA before actually submitting the request.</span></span>|
|<span data-ttu-id="65808-174">targetScheduleId</span><span class="sxs-lookup"><span data-stu-id="65808-174">targetScheduleId</span></span>|<span data-ttu-id="65808-175">String</span><span class="sxs-lookup"><span data-stu-id="65808-175">String</span></span>|<span data-ttu-id="65808-176">ID do objeto schedule anexado à atribuição.</span><span class="sxs-lookup"><span data-stu-id="65808-176">ID of the schedule object attached to the assignment.</span></span>|
|<span data-ttu-id="65808-177">justification</span><span class="sxs-lookup"><span data-stu-id="65808-177">justification</span></span>|<span data-ttu-id="65808-178">String</span><span class="sxs-lookup"><span data-stu-id="65808-178">String</span></span>|<span data-ttu-id="65808-179">Uma mensagem fornecida por usuários e administradores ao criar a solicitação sobre por que ela é necessária.</span><span class="sxs-lookup"><span data-stu-id="65808-179">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="65808-180">scheduleInfo</span><span class="sxs-lookup"><span data-stu-id="65808-180">scheduleInfo</span></span>|[<span data-ttu-id="65808-181">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="65808-181">requestSchedule</span></span>](../resources/requestschedule.md)|<span data-ttu-id="65808-182">O objeto schedule da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="65808-182">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="65808-183">ticketInfo</span><span class="sxs-lookup"><span data-stu-id="65808-183">ticketInfo</span></span>|[<span data-ttu-id="65808-184">ticketInfo</span><span class="sxs-lookup"><span data-stu-id="65808-184">ticketInfo</span></span>](../resources/ticketinfo.md)|<span data-ttu-id="65808-185">O objeto ticketInfo anexado à solicitação de atribuição de função que inclui detalhes do número do tíquete e do sistema de tíquetes.</span><span class="sxs-lookup"><span data-stu-id="65808-185">The ticketInfo object attached to the role assignment request which includes details of the ticket number and ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="65808-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="65808-186">Response</span></span>

<span data-ttu-id="65808-187">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65808-187">If successful, this method returns a `201 Created` response code and an [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65808-188">Exemplos</span><span class="sxs-lookup"><span data-stu-id="65808-188">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65808-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65808-189">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="65808-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="65808-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleeligibilityschedulerequest_from_unifiedroleeligibilityschedulerequests"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
Content-Type: application/json
Content-length: 511

{
  "@odata.type": "#Microsoft.Identity.Governance.Common.Data.ExternalModels.V1.unifiedRoleEligibilityScheduleRequest",
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
# <a name="c"></a>[<span data-ttu-id="65808-191">C#</span><span class="sxs-lookup"><span data-stu-id="65808-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65808-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65808-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65808-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65808-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65808-194">Java</span><span class="sxs-lookup"><span data-stu-id="65808-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="65808-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="65808-195">Response</span></span>
<span data-ttu-id="65808-196">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="65808-196">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "a2e242a0-42a0-a2e2-a042-e2a2a042e2a2",
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

