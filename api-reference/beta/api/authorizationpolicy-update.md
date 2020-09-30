---
title: Atualizar AuthorizationPolicy
description: Atualize as propriedades do objeto authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d4f8bd9053db7b58e3aec81e82a5d0c2d20c2407
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312418"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="70e75-103">Atualizar authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="70e75-103">Update authorizationPolicy</span></span>

<span data-ttu-id="70e75-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70e75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70e75-105">Atualiza as propriedades de um objeto [authorizationPolicy](../resources/authorizationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="70e75-105">Update the properties of a [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="70e75-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="70e75-106">Permissions</span></span>

<span data-ttu-id="70e75-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70e75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70e75-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70e75-109">Permission type</span></span>                        | <span data-ttu-id="70e75-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70e75-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="70e75-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70e75-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="70e75-112">Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="70e75-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="70e75-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70e75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70e75-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70e75-114">Not supported.</span></span> |
| <span data-ttu-id="70e75-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70e75-115">Application</span></span>                            | <span data-ttu-id="70e75-116">Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="70e75-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="70e75-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70e75-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="70e75-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70e75-118">Request headers</span></span>

| <span data-ttu-id="70e75-119">Nome</span><span class="sxs-lookup"><span data-stu-id="70e75-119">Name</span></span>       | <span data-ttu-id="70e75-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="70e75-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="70e75-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="70e75-121">Authorization</span></span> | <span data-ttu-id="70e75-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="70e75-122">Bearer {token}</span></span> |
| <span data-ttu-id="70e75-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="70e75-123">Content-type</span></span> | <span data-ttu-id="70e75-124">application/json</span><span class="sxs-lookup"><span data-stu-id="70e75-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="70e75-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70e75-125">Request body</span></span>

<span data-ttu-id="70e75-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="70e75-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="70e75-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="70e75-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="70e75-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="70e75-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="70e75-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70e75-129">Property</span></span>     | <span data-ttu-id="70e75-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="70e75-130">Type</span></span>        | <span data-ttu-id="70e75-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="70e75-131">Description</span></span> |
|:-------------|:------------|:------------|  
|<span data-ttu-id="70e75-132">displayName</span><span class="sxs-lookup"><span data-stu-id="70e75-132">displayName</span></span>|<span data-ttu-id="70e75-133">String</span><span class="sxs-lookup"><span data-stu-id="70e75-133">String</span></span>| <span data-ttu-id="70e75-134">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="70e75-134">Display name for this policy.</span></span> |  
|<span data-ttu-id="70e75-135">description</span><span class="sxs-lookup"><span data-stu-id="70e75-135">description</span></span>|<span data-ttu-id="70e75-136">String</span><span class="sxs-lookup"><span data-stu-id="70e75-136">String</span></span>| <span data-ttu-id="70e75-137">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="70e75-137">Description of this policy.</span></span> |  
|<span data-ttu-id="70e75-138">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="70e75-138">guestUserRoleId</span></span>|<span data-ttu-id="70e75-139">Guid</span><span class="sxs-lookup"><span data-stu-id="70e75-139">Guid</span></span>| <span data-ttu-id="70e75-140">Representa o modelo de função para a função que deve ser concedida ao usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="70e75-140">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="70e75-141">Consulte [list unifiedRoleDefinitions](./rbacapplication-list-roledefinitions.md) para encontrar a lista de modelos de função disponíveis.</span><span class="sxs-lookup"><span data-stu-id="70e75-141">Refer to [List unifiedRoleDefinitions](./rbacapplication-list-roledefinitions.md) to find the list of available role templates.</span></span> <span data-ttu-id="70e75-142">Somente as funções suportadas hoje são usuário (a0b1b346-4d3e-4e8b-98f8-753987be4970), usuário convidado (10dae51f-b6af-4016-8d66-8c2a99b929b3) e usuário convidado restrito (2af84b1e-32c8-42b7-82bc-daa82404023b).</span><span class="sxs-lookup"><span data-stu-id="70e75-142">Only supported roles today are User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="70e75-143">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="70e75-143">enabledPreviewFeatures</span></span>|<span data-ttu-id="70e75-144">Coleção (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="70e75-144">Collection(string)</span></span>| <span data-ttu-id="70e75-145">Lista de recursos habilitados para visualização privada no locatário.</span><span class="sxs-lookup"><span data-stu-id="70e75-145">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="70e75-146">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="70e75-146">blockMsolPowerShell</span></span>|<span data-ttu-id="70e75-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="70e75-147">Boolean</span></span>| <span data-ttu-id="70e75-148">Para desabilitar o uso do MSOL PowerShell, defina essa propriedade como `true` .</span><span class="sxs-lookup"><span data-stu-id="70e75-148">To disable the use of MSOL PowerShell, set this property to `true`.</span></span> <span data-ttu-id="70e75-149">A configuração `true` também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSol PowerShell.</span><span class="sxs-lookup"><span data-stu-id="70e75-149">Setting to `true` will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="70e75-150">Isso não afeta o Azure AD Connect ou o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="70e75-150">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="70e75-151">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="70e75-151">defaultUserRolePermissions</span></span>|[<span data-ttu-id="70e75-152">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="70e75-152">defaultUserRolePermissions</span></span>](../resources/defaultUserRolePermissions.md)| <span data-ttu-id="70e75-153">Especifica determinadas permissões personalizáveis para a função de usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="70e75-153">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="70e75-154">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="70e75-154">allowedToUseSSPR</span></span>|<span data-ttu-id="70e75-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="70e75-155">Boolean</span></span>| <span data-ttu-id="70e75-156">Indica se o recurso de redefinição de senha de autoatendimento pode ser usado por usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="70e75-156">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="70e75-157">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="70e75-157">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="70e75-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="70e75-158">Boolean</span></span>| <span data-ttu-id="70e75-159">Indica se os usuários podem se inscrever para assinaturas baseadas em email.</span><span class="sxs-lookup"><span data-stu-id="70e75-159">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="70e75-160">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="70e75-160">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="70e75-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="70e75-161">Boolean</span></span>| <span data-ttu-id="70e75-162">Indica se um usuário pode ingressar no locatário por validação de email.</span><span class="sxs-lookup"><span data-stu-id="70e75-162">Indicates whether a user can join the tenant by email validation.</span></span> | 

## <a name="response"></a><span data-ttu-id="70e75-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="70e75-163">Response</span></span>

<span data-ttu-id="70e75-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70e75-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="70e75-166">Exemplos</span><span class="sxs-lookup"><span data-stu-id="70e75-166">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="70e75-167">Exemplo 1: atualizar ou definir o nível de acesso do usuário convidado para o locatário</span><span class="sxs-lookup"><span data-stu-id="70e75-167">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="70e75-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70e75-168">Request</span></span>

<span data-ttu-id="70e75-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="70e75-169">The following is an example of the request.</span></span> <span data-ttu-id="70e75-170">Neste exemplo, o nível de acesso de convidado é modificado para o usuário convidado restrito.</span><span class="sxs-lookup"><span data-stu-id="70e75-170">In this example, guest access level is modified to Restricted Guest User.</span></span>

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
#### <a name="response"></a><span data-ttu-id="70e75-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="70e75-171">Response</span></span>

<span data-ttu-id="70e75-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="70e75-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content

```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a><span data-ttu-id="70e75-173">Exemplo 2: habilitar novo recurso para visualização no locatário</span><span class="sxs-lookup"><span data-stu-id="70e75-173">Example 2: Enable new feature for preview on tenant</span></span>

#### <a name="request"></a><span data-ttu-id="70e75-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70e75-174">Request</span></span>

<span data-ttu-id="70e75-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="70e75-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="70e75-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="70e75-176">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="70e75-177">C#</span><span class="sxs-lookup"><span data-stu-id="70e75-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-preview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70e75-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70e75-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-preview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70e75-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70e75-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-preview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="70e75-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="70e75-180">Response</span></span>

<span data-ttu-id="70e75-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="70e75-181">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```


### <a name="example-3-block-msol-powershell-in-tenant"></a><span data-ttu-id="70e75-182">Exemplo 3: bloquear o MSOL PowerShell no locatário</span><span class="sxs-lookup"><span data-stu-id="70e75-182">Example 3: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="70e75-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70e75-183">Request</span></span>

<span data-ttu-id="70e75-184">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="70e75-184">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="70e75-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="70e75-185">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="70e75-186">C#</span><span class="sxs-lookup"><span data-stu-id="70e75-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70e75-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70e75-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70e75-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70e75-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="70e75-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="70e75-189">Response</span></span>

<span data-ttu-id="70e75-190">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="70e75-190">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-4-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="70e75-191">Exemplo 4: desabilitar a permissão de função de usuário padrão para criar aplicativos</span><span class="sxs-lookup"><span data-stu-id="70e75-191">Example 4: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="70e75-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70e75-192">Request</span></span>

<span data-ttu-id="70e75-193">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="70e75-193">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="70e75-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="70e75-194">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="70e75-195">C#</span><span class="sxs-lookup"><span data-stu-id="70e75-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70e75-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70e75-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70e75-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70e75-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="70e75-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="70e75-198">Response</span></span>

<span data-ttu-id="70e75-199">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="70e75-199">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="70e75-200">Exemplo 5: habilitar a função de usuário padrão para usar o recurso de redefinição de senha de autoatendimento</span><span class="sxs-lookup"><span data-stu-id="70e75-200">Example 5: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="70e75-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70e75-201">Request</span></span>

<span data-ttu-id="70e75-202">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="70e75-202">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="70e75-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="70e75-203">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="70e75-204">C#</span><span class="sxs-lookup"><span data-stu-id="70e75-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70e75-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70e75-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70e75-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70e75-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="70e75-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="70e75-207">Response</span></span>

<span data-ttu-id="70e75-208">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="70e75-208">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
