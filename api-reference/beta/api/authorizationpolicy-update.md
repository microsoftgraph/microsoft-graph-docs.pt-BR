---
title: Atualizar a política de autorização
description: Atualize as propriedades do objeto authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 723f8b174a256cc3b739922101f897067594bd43
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786850"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="8e148-103">Atualizar authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="8e148-103">Update authorizationPolicy</span></span>

<span data-ttu-id="8e148-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e148-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e148-105">Atualize as propriedades de um [objeto authorizationPolicy.](../resources/authorizationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8e148-105">Update the properties of a [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e148-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8e148-106">Permissions</span></span>

<span data-ttu-id="8e148-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e148-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e148-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e148-109">Permission type</span></span>                        | <span data-ttu-id="8e148-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e148-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8e148-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e148-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e148-112">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="8e148-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="8e148-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e148-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e148-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e148-114">Not supported.</span></span> |
| <span data-ttu-id="8e148-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e148-115">Application</span></span>                            | <span data-ttu-id="8e148-116">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="8e148-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e148-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e148-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="8e148-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e148-118">Request headers</span></span>

| <span data-ttu-id="8e148-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8e148-119">Name</span></span>       | <span data-ttu-id="8e148-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e148-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8e148-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e148-121">Authorization</span></span> | <span data-ttu-id="8e148-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8e148-122">Bearer {token}</span></span> |
| <span data-ttu-id="8e148-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="8e148-123">Content-type</span></span> | <span data-ttu-id="8e148-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8e148-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e148-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e148-125">Request body</span></span>

<span data-ttu-id="8e148-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="8e148-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8e148-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="8e148-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8e148-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8e148-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8e148-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e148-129">Property</span></span>     | <span data-ttu-id="8e148-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e148-130">Type</span></span>        | <span data-ttu-id="8e148-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e148-131">Description</span></span> |
|:-------------|:------------|:------------|  
|<span data-ttu-id="8e148-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8e148-132">displayName</span></span>|<span data-ttu-id="8e148-133">String</span><span class="sxs-lookup"><span data-stu-id="8e148-133">String</span></span>| <span data-ttu-id="8e148-134">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="8e148-134">Display name for this policy.</span></span> |  
|<span data-ttu-id="8e148-135">description</span><span class="sxs-lookup"><span data-stu-id="8e148-135">description</span></span>|<span data-ttu-id="8e148-136">String</span><span class="sxs-lookup"><span data-stu-id="8e148-136">String</span></span>| <span data-ttu-id="8e148-137">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="8e148-137">Description of this policy.</span></span> |  
|<span data-ttu-id="8e148-138">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="8e148-138">guestUserRoleId</span></span>|<span data-ttu-id="8e148-139">Guid</span><span class="sxs-lookup"><span data-stu-id="8e148-139">Guid</span></span>| <span data-ttu-id="8e148-140">Representa modelo de funçãoId para a função que deve ser concedida ao usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="8e148-140">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="8e148-141">Consulte [Listar unifiedRoleDefinitions](./rbacapplication-list-roledefinitions.md) para encontrar a lista de modelos de função disponíveis.</span><span class="sxs-lookup"><span data-stu-id="8e148-141">Refer to [List unifiedRoleDefinitions](./rbacapplication-list-roledefinitions.md) to find the list of available role templates.</span></span> <span data-ttu-id="8e148-142">Atualmente, somente as funções com suporte são User ( `a0b1b346-4d3e-4e8b-98f8-753987be4970` ), Guest User ( ) e `10dae51f-b6af-4016-8d66-8c2a99b929b3` Restricted Guest User ( `2af84b1e-32c8-42b7-82bc-daa82404023b` ).</span><span class="sxs-lookup"><span data-stu-id="8e148-142">Only supported roles today are User (`a0b1b346-4d3e-4e8b-98f8-753987be4970`), Guest User (`10dae51f-b6af-4016-8d66-8c2a99b929b3`), and Restricted Guest User (`2af84b1e-32c8-42b7-82bc-daa82404023b`).</span></span> | 
|<span data-ttu-id="8e148-143">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="8e148-143">enabledPreviewFeatures</span></span>|<span data-ttu-id="8e148-144">Collection(string)</span><span class="sxs-lookup"><span data-stu-id="8e148-144">Collection(string)</span></span>| <span data-ttu-id="8e148-145">Lista de recursos habilitados para visualização privada no locatário.</span><span class="sxs-lookup"><span data-stu-id="8e148-145">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="8e148-146">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="8e148-146">blockMsolPowerShell</span></span>|<span data-ttu-id="8e148-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e148-147">Boolean</span></span>| <span data-ttu-id="8e148-148">Para desabilitar o uso do MSOL PowerShell, de definir essa propriedade como `true` .</span><span class="sxs-lookup"><span data-stu-id="8e148-148">To disable the use of MSOL PowerShell, set this property to `true`.</span></span> <span data-ttu-id="8e148-149">Isso também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8e148-149">This will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="8e148-150">Isso não afeta o Azure AD Conexão ou o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8e148-150">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="8e148-151">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="8e148-151">defaultUserRolePermissions</span></span>|[<span data-ttu-id="8e148-152">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="8e148-152">defaultUserRolePermissions</span></span>](../resources/defaultUserRolePermissions.md)| <span data-ttu-id="8e148-153">Especifica determinadas permissões personalizáveis para a função de usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="8e148-153">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="8e148-154">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="8e148-154">allowedToUseSSPR</span></span>|<span data-ttu-id="8e148-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e148-155">Boolean</span></span>| <span data-ttu-id="8e148-156">Indica se o recurso Self-Serve redefinição de senha pode ser usado pelos usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="8e148-156">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="8e148-157">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="8e148-157">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="8e148-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e148-158">Boolean</span></span>| <span data-ttu-id="8e148-159">Indica se os usuários podem se inscrever para assinaturas baseadas em email.</span><span class="sxs-lookup"><span data-stu-id="8e148-159">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="8e148-160">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="8e148-160">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="8e148-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e148-161">Boolean</span></span>| <span data-ttu-id="8e148-162">Indica se um usuário pode ingressar no locatário por validação de email.</span><span class="sxs-lookup"><span data-stu-id="8e148-162">Indicates whether a user can join the tenant by email validation.</span></span> |
| <span data-ttu-id="8e148-163">permissionGrantPolicyIdsAssignedToDefaultUserRole</span><span class="sxs-lookup"><span data-stu-id="8e148-163">permissionGrantPolicyIdsAssignedToDefaultUserRole</span></span> | <span data-ttu-id="8e148-164">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e148-164">String collection</span></span> | <span data-ttu-id="8e148-165">Indica se o consentimento do usuário para aplicativos [](/azure/active-directory/manage-apps/manage-app-consent-policies) é permitido e, se for, qual política de consentimento de aplicativo rege a permissão para que os usuários concedam consentimento.</span><span class="sxs-lookup"><span data-stu-id="8e148-165">Indicates whether user consent to apps is allowed, and if it is, which [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) governs the permission for users to grant consent.</span></span> <span data-ttu-id="8e148-166">Os valores devem estar no formato `managePermissionGrantsForSelf.{id}` , onde é a id de uma política de consentimento de aplicativo interna ou `{id}` [personalizada.](/azure/active-directory/manage-apps/manage-app-consent-policies) </span><span class="sxs-lookup"><span data-stu-id="8e148-166">Values should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="8e148-167">Uma lista vazia indica que o consentimento do usuário para aplicativos está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="8e148-167">An empty list indicates user consent to apps is disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="8e148-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e148-168">Response</span></span>

<span data-ttu-id="8e148-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e148-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8e148-171">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8e148-171">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="8e148-172">Exemplo 1: atualizar ou definir o nível de acesso do usuário convidado para o locatário</span><span class="sxs-lookup"><span data-stu-id="8e148-172">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="8e148-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e148-173">Request</span></span>

<span data-ttu-id="8e148-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e148-174">The following is an example of the request.</span></span> <span data-ttu-id="8e148-175">Neste exemplo, o nível de acesso de convidado é modificado para Usuário Convidado Restrito.</span><span class="sxs-lookup"><span data-stu-id="8e148-175">In this example, guest access level is modified to Restricted Guest User.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_guestUserLevel"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "guestUserRole":"2af84b1e-32c8-42b7-82bc-daa82404023b"
}
```

#### <a name="response"></a><span data-ttu-id="8e148-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e148-176">Response</span></span>

<span data-ttu-id="8e148-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e148-177">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a><span data-ttu-id="8e148-178">Exemplo 2: Habilitar novo recurso para visualização no locatário</span><span class="sxs-lookup"><span data-stu-id="8e148-178">Example 2: Enable new feature for preview on tenant</span></span>

#### <a name="request"></a><span data-ttu-id="8e148-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e148-179">Request</span></span>

<span data-ttu-id="8e148-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e148-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e148-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e148-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_preview"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "enabledPreviewFeatures":[
      "assignGroupsToRoles"
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="8e148-182">C#</span><span class="sxs-lookup"><span data-stu-id="8e148-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-preview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e148-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e148-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-preview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e148-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e148-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-preview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e148-185">Java</span><span class="sxs-lookup"><span data-stu-id="8e148-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-preview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8e148-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e148-186">Response</span></span>

<span data-ttu-id="8e148-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e148-187">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-block-msol-powershell-in-tenant"></a><span data-ttu-id="8e148-188">Exemplo 3: Bloquear o MSOL PowerShell no locatário</span><span class="sxs-lookup"><span data-stu-id="8e148-188">Example 3: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="8e148-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e148-189">Request</span></span>

<span data-ttu-id="8e148-190">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e148-190">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e148-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e148-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_blockMSOLPowerShell"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "blockMsolPowerShell":true
}
```
# <a name="c"></a>[<span data-ttu-id="8e148-192">C#</span><span class="sxs-lookup"><span data-stu-id="8e148-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e148-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e148-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e148-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e148-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e148-195">Java</span><span class="sxs-lookup"><span data-stu-id="8e148-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-blockmsolpowershell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8e148-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e148-196">Response</span></span>

<span data-ttu-id="8e148-197">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e148-197">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-4-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="8e148-198">Exemplo 4: Desabilitar a permissão da função de usuário padrão para criar aplicativos</span><span class="sxs-lookup"><span data-stu-id="8e148-198">Example 4: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="8e148-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e148-199">Request</span></span>

<span data-ttu-id="8e148-200">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e148-200">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e148-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e148-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_applications"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "defaultUserRolePermissions":{
      "allowedToCreateApps":false
   }
}
```
# <a name="c"></a>[<span data-ttu-id="8e148-202">C#</span><span class="sxs-lookup"><span data-stu-id="8e148-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e148-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e148-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e148-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e148-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e148-205">Java</span><span class="sxs-lookup"><span data-stu-id="8e148-205">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8e148-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e148-206">Response</span></span>

<span data-ttu-id="8e148-207">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e148-207">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="8e148-208">Exemplo 5: Habilitar a função de usuário padrão para usar Self-Serve redefinição de senha</span><span class="sxs-lookup"><span data-stu-id="8e148-208">Example 5: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="8e148-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e148-209">Request</span></span>

<span data-ttu-id="8e148-210">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e148-210">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e148-211">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e148-211">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_SSPR"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "allowedToUseSSPR":true
}
```
# <a name="c"></a>[<span data-ttu-id="8e148-212">C#</span><span class="sxs-lookup"><span data-stu-id="8e148-212">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e148-213">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e148-213">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e148-214">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e148-214">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e148-215">Java</span><span class="sxs-lookup"><span data-stu-id="8e148-215">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-sspr-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8e148-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e148-216">Response</span></span>

<span data-ttu-id="8e148-217">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e148-217">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-6-disable-user-consent-to-apps-for-default-user-role"></a><span data-ttu-id="8e148-218">Exemplo 6: Desabilitar o consentimento do usuário para aplicativos para a função de usuário padrão</span><span class="sxs-lookup"><span data-stu-id="8e148-218">Example 6: Disable user consent to apps for default user role</span></span>

#### <a name="request"></a><span data-ttu-id="8e148-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e148-219">Request</span></span>

<span data-ttu-id="8e148-220">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e148-220">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e148-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e148-221">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_disableUserConsent"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "permissionGrantPolicyIdsAssignedToDefaultUserRole":[
   
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="8e148-222">C#</span><span class="sxs-lookup"><span data-stu-id="8e148-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-disableuserconsent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e148-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e148-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-disableuserconsent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e148-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e148-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-disableuserconsent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e148-225">Java</span><span class="sxs-lookup"><span data-stu-id="8e148-225">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-disableuserconsent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e148-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e148-226">Response</span></span>

<span data-ttu-id="8e148-227">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e148-227">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-7-enable-user-consent-to-apps-subject-to-app-consent-policy"></a><span data-ttu-id="8e148-228">Exemplo 7: Habilitar o consentimento do usuário para aplicativos, sujeito à política de consentimento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e148-228">Example 7: Enable user consent to apps, subject to app consent policy</span></span> 

#### <a name="request"></a><span data-ttu-id="8e148-229">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e148-229">Request</span></span>

<span data-ttu-id="8e148-230">A seguir, um exemplo da solicitação que permite o consentimento [](/azure/active-directory/manage-apps/manage-app-consent-policies) do usuário para aplicativos, sujeito à política de consentimento de aplicativo interna , que permite permissões delegadas `microsoft-user-default-low` classificadas como "baixas", para aplicativos cliente de editores verificados ou registrados no mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="8e148-230">The following is an example of the request that allows user consent to apps, subject to the built-in [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low`, which allows delegated permissions classified "low", for client apps from verified publishers or registered in the same tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e148-231">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e148-231">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_enableUserConsentLow"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "permissionGrantPolicyIdsAssignedToDefaultUserRole":[
      "managePermissionGrantsForSelf.microsoft-user-default-low"
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="8e148-232">C#</span><span class="sxs-lookup"><span data-stu-id="8e148-232">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-enableuserconsentlow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e148-233">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e148-233">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-enableuserconsentlow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e148-234">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e148-234">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-enableuserconsentlow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e148-235">Java</span><span class="sxs-lookup"><span data-stu-id="8e148-235">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-enableuserconsentlow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e148-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e148-236">Response</span></span>

<span data-ttu-id="8e148-237">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e148-237">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
