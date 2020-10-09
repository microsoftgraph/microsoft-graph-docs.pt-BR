---
title: Atualizar AuthorizationPolicy
description: Atualize as propriedades do objeto authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3a51767eb02765b3c6914d8b04c5758202b3df1f
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401901"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="79178-103">Atualizar authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="79178-103">Update authorizationPolicy</span></span>

<span data-ttu-id="79178-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79178-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79178-105">Atualiza as propriedades de um objeto [authorizationPolicy](../resources/authorizationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="79178-105">Update the properties of a [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="79178-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="79178-106">Permissions</span></span>

<span data-ttu-id="79178-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79178-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79178-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79178-109">Permission type</span></span>                        | <span data-ttu-id="79178-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79178-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="79178-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79178-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="79178-112">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="79178-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="79178-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79178-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79178-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79178-114">Not supported.</span></span> |
| <span data-ttu-id="79178-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79178-115">Application</span></span>                            | <span data-ttu-id="79178-116">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="79178-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="79178-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79178-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="79178-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79178-118">Request headers</span></span>

| <span data-ttu-id="79178-119">Nome</span><span class="sxs-lookup"><span data-stu-id="79178-119">Name</span></span>       | <span data-ttu-id="79178-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="79178-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="79178-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="79178-121">Authorization</span></span> | <span data-ttu-id="79178-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="79178-122">Bearer {token}</span></span> |
| <span data-ttu-id="79178-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="79178-123">Content-type</span></span> | <span data-ttu-id="79178-124">application/json</span><span class="sxs-lookup"><span data-stu-id="79178-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="79178-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79178-125">Request body</span></span>

<span data-ttu-id="79178-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="79178-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="79178-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="79178-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="79178-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="79178-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="79178-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79178-129">Property</span></span>     | <span data-ttu-id="79178-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="79178-130">Type</span></span>        | <span data-ttu-id="79178-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="79178-131">Description</span></span> |
|:-------------|:------------|:------------|  
|<span data-ttu-id="79178-132">displayName</span><span class="sxs-lookup"><span data-stu-id="79178-132">displayName</span></span>|<span data-ttu-id="79178-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79178-133">String</span></span>| <span data-ttu-id="79178-134">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="79178-134">Display name for this policy.</span></span> |  
|<span data-ttu-id="79178-135">description</span><span class="sxs-lookup"><span data-stu-id="79178-135">description</span></span>|<span data-ttu-id="79178-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79178-136">String</span></span>| <span data-ttu-id="79178-137">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="79178-137">Description of this policy.</span></span> |  
|<span data-ttu-id="79178-138">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="79178-138">guestUserRoleId</span></span>|<span data-ttu-id="79178-139">Guid</span><span class="sxs-lookup"><span data-stu-id="79178-139">Guid</span></span>| <span data-ttu-id="79178-140">Representa o modelo de função para a função que deve ser concedida ao usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="79178-140">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="79178-141">Consulte [list unifiedRoleDefinitions](./rbacapplication-list-roledefinitions.md) para encontrar a lista de modelos de função disponíveis.</span><span class="sxs-lookup"><span data-stu-id="79178-141">Refer to [List unifiedRoleDefinitions](./rbacapplication-list-roledefinitions.md) to find the list of available role templates.</span></span> <span data-ttu-id="79178-142">Somente as funções suportadas hoje são usuário (a0b1b346-4d3e-4e8b-98f8-753987be4970), usuário convidado (10dae51f-b6af-4016-8d66-8c2a99b929b3) e usuário convidado restrito (2af84b1e-32c8-42b7-82bc-daa82404023b).</span><span class="sxs-lookup"><span data-stu-id="79178-142">Only supported roles today are User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="79178-143">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="79178-143">enabledPreviewFeatures</span></span>|<span data-ttu-id="79178-144">Coleção (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="79178-144">Collection(string)</span></span>| <span data-ttu-id="79178-145">Lista de recursos habilitados para visualização privada no locatário.</span><span class="sxs-lookup"><span data-stu-id="79178-145">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="79178-146">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="79178-146">blockMsolPowerShell</span></span>|<span data-ttu-id="79178-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="79178-147">Boolean</span></span>| <span data-ttu-id="79178-148">Para desabilitar o uso do MSOL PowerShell, defina essa propriedade como `true` .</span><span class="sxs-lookup"><span data-stu-id="79178-148">To disable the use of MSOL PowerShell, set this property to `true`.</span></span> <span data-ttu-id="79178-149">A configuração `true` também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSol PowerShell.</span><span class="sxs-lookup"><span data-stu-id="79178-149">Setting to `true` will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="79178-150">Isso não afeta o Azure AD Connect ou o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="79178-150">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="79178-151">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="79178-151">defaultUserRolePermissions</span></span>|[<span data-ttu-id="79178-152">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="79178-152">defaultUserRolePermissions</span></span>](../resources/defaultUserRolePermissions.md)| <span data-ttu-id="79178-153">Especifica determinadas permissões personalizáveis para a função de usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="79178-153">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="79178-154">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="79178-154">allowedToUseSSPR</span></span>|<span data-ttu-id="79178-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="79178-155">Boolean</span></span>| <span data-ttu-id="79178-156">Indica se o Self-Serve recurso de redefinição de senha pode ser usado por usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="79178-156">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="79178-157">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="79178-157">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="79178-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="79178-158">Boolean</span></span>| <span data-ttu-id="79178-159">Indica se os usuários podem se inscrever para assinaturas baseadas em email.</span><span class="sxs-lookup"><span data-stu-id="79178-159">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="79178-160">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="79178-160">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="79178-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="79178-161">Boolean</span></span>| <span data-ttu-id="79178-162">Indica se um usuário pode ingressar no locatário por validação de email.</span><span class="sxs-lookup"><span data-stu-id="79178-162">Indicates whether a user can join the tenant by email validation.</span></span> |
| <span data-ttu-id="79178-163">permissionGrantPolicyIdsAssignedToDefaultUserRole</span><span class="sxs-lookup"><span data-stu-id="79178-163">permissionGrantPolicyIdsAssignedToDefaultUserRole</span></span> | <span data-ttu-id="79178-164">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="79178-164">String collection</span></span> | <span data-ttu-id="79178-165">Indica se o consentimento do usuário para os aplicativos é permitido e, se for, qual [política de consentimento de aplicativos](/azure/active-directory/manage-apps/manage-app-consent-policies) governará a permissão para os usuários concederem o consentimento.</span><span class="sxs-lookup"><span data-stu-id="79178-165">Indicates whether user consent to apps is allowed, and if it is, which [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) governs the permission for users to grant consent.</span></span> <span data-ttu-id="79178-166">Os valores devem estar no formato `managePermissionGrantsForSelf.{id}` , onde `{id}` é a **ID** de uma [política de consentimento de aplicativo](/azure/active-directory/manage-apps/manage-app-consent-policies)interna ou personalizada.</span><span class="sxs-lookup"><span data-stu-id="79178-166">Values should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="79178-167">Uma lista vazia indica que o consentimento do usuário para os aplicativos está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="79178-167">An empty list indicates user consent to apps is disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="79178-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="79178-168">Response</span></span>

<span data-ttu-id="79178-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79178-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79178-171">Exemplos</span><span class="sxs-lookup"><span data-stu-id="79178-171">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="79178-172">Exemplo 1: atualizar ou definir o nível de acesso do usuário convidado para o locatário</span><span class="sxs-lookup"><span data-stu-id="79178-172">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="79178-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79178-173">Request</span></span>

<span data-ttu-id="79178-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79178-174">The following is an example of the request.</span></span> <span data-ttu-id="79178-175">Neste exemplo, o nível de acesso de convidado é modificado para o usuário convidado restrito.</span><span class="sxs-lookup"><span data-stu-id="79178-175">In this example, guest access level is modified to Restricted Guest User.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_guestUserLevel"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
  "guestUserRole": "2af84b1e-32c8-42b7-82bc-daa82404023b"
}

```

#### <a name="response"></a><span data-ttu-id="79178-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="79178-176">Response</span></span>

<span data-ttu-id="79178-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79178-177">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a><span data-ttu-id="79178-178">Exemplo 2: habilitar novo recurso para visualização no locatário</span><span class="sxs-lookup"><span data-stu-id="79178-178">Example 2: Enable new feature for preview on tenant</span></span>

#### <a name="request"></a><span data-ttu-id="79178-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79178-179">Request</span></span>

<span data-ttu-id="79178-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79178-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="79178-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="79178-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_preview"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
  "enabledPreviewFeatures": ["assignGroupsToRoles"]
}

```
# <a name="c"></a>[<span data-ttu-id="79178-182">C#</span><span class="sxs-lookup"><span data-stu-id="79178-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-preview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79178-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79178-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-preview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79178-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79178-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-preview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="79178-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="79178-185">Response</span></span>

<span data-ttu-id="79178-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79178-186">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-block-msol-powershell-in-tenant"></a><span data-ttu-id="79178-187">Exemplo 3: bloquear o MSOL PowerShell no locatário</span><span class="sxs-lookup"><span data-stu-id="79178-187">Example 3: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="79178-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79178-188">Request</span></span>

<span data-ttu-id="79178-189">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79178-189">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="79178-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="79178-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_blockMSOLPowerShell"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
  "blockMsolPowerShell": true
}

```
# <a name="c"></a>[<span data-ttu-id="79178-191">C#</span><span class="sxs-lookup"><span data-stu-id="79178-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79178-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79178-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79178-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79178-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="79178-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="79178-194">Response</span></span>

<span data-ttu-id="79178-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79178-195">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-4-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="79178-196">Exemplo 4: desabilitar a permissão de função de usuário padrão para criar aplicativos</span><span class="sxs-lookup"><span data-stu-id="79178-196">Example 4: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="79178-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79178-197">Request</span></span>

<span data-ttu-id="79178-198">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79178-198">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="79178-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="79178-199">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_applications"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
    "defaultUserRolePermissions":
    {
      "allowedToCreateApps": false
    }
}

```
# <a name="c"></a>[<span data-ttu-id="79178-200">C#</span><span class="sxs-lookup"><span data-stu-id="79178-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79178-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79178-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79178-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79178-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="79178-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="79178-203">Response</span></span>

<span data-ttu-id="79178-204">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79178-204">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="79178-205">Exemplo 5: habilitar a função de usuário padrão para usar Self-Serve recurso de redefinição de senha</span><span class="sxs-lookup"><span data-stu-id="79178-205">Example 5: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="79178-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79178-206">Request</span></span>

<span data-ttu-id="79178-207">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79178-207">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="79178-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="79178-208">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_SSPR"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
    "allowedToUseSSPR": true
}

```
# <a name="c"></a>[<span data-ttu-id="79178-209">C#</span><span class="sxs-lookup"><span data-stu-id="79178-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79178-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79178-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79178-211">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79178-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="79178-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="79178-212">Response</span></span>

<span data-ttu-id="79178-213">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79178-213">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-6-disable-user-consent-to-apps-for-default-user-role"></a><span data-ttu-id="79178-214">Exemplo 6: desabilitar o consentimento do usuário para os aplicativos para a função de usuário padrão</span><span class="sxs-lookup"><span data-stu-id="79178-214">Example 6: Disable user consent to apps for default user role</span></span>

#### <a name="request"></a><span data-ttu-id="79178-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79178-215">Request</span></span>

<span data-ttu-id="79178-216">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79178-216">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_disableUserConsent"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
    "permissionGrantPolicyIdsAssignedToDefaultUserRole": [ ]
}
```

#### <a name="response"></a><span data-ttu-id="79178-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="79178-217">Response</span></span>

<span data-ttu-id="79178-218">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79178-218">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-7-enable-user-consent-to-apps-subject-to-app-consent-policy"></a><span data-ttu-id="79178-219">Exemplo 7: habilitar o consentimento do usuário para aplicativos, sujeito à política de consentimento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="79178-219">Example 7: Enable user consent to apps, subject to app consent policy</span></span> 

#### <a name="request"></a><span data-ttu-id="79178-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79178-220">Request</span></span>

<span data-ttu-id="79178-221">Veja a seguir um exemplo da solicitação que permite o consentimento do usuário para os aplicativos, sujeito à política de [consentimento de aplicativo](/azure/active-directory/manage-apps/manage-app-consent-policies) interna `microsoft-user-default-low` , que permite as permissões delegadas "baixa", para aplicativos clientes de editores verificados ou registrados no mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="79178-221">The following is an example of the request that allows user consent to apps, subject to the built-in [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low`, which allows delegated permissions classified "low", for client apps from verified publishers or registered in the same tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_enableUserConsentLow"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
    "permissionGrantPolicyIdsAssignedToDefaultUserRole": [
        "managePermissionGrantsForSelf.microsoft-user-default-low"
    ]
}
```

#### <a name="response"></a><span data-ttu-id="79178-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="79178-222">Response</span></span>

<span data-ttu-id="79178-223">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79178-223">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationpolicy"
} -->

```http
HTTP/1.1 204 No Content
```
