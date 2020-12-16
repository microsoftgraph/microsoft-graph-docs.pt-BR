---
title: Atualizar AuthorizationPolicy
description: Atualize as propriedades do objeto authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e8ae872ad6a78f7faee94802d7d93f8775900903
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691357"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="2d088-103">Atualizar authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="2d088-103">Update authorizationPolicy</span></span>

<span data-ttu-id="2d088-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d088-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d088-105">Atualiza as propriedades de um objeto [authorizationPolicy](../resources/authorizationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="2d088-105">Update the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d088-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2d088-106">Permissions</span></span>

<span data-ttu-id="2d088-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d088-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d088-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d088-109">Permission type</span></span>                        | <span data-ttu-id="2d088-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2d088-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2d088-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d088-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d088-112">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="2d088-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="2d088-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d088-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d088-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d088-114">Not supported.</span></span> |
| <span data-ttu-id="2d088-115">Application</span><span class="sxs-lookup"><span data-stu-id="2d088-115">Application</span></span>                            | <span data-ttu-id="2d088-116">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="2d088-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d088-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d088-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="2d088-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d088-118">Request headers</span></span>

| <span data-ttu-id="2d088-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2d088-119">Name</span></span>       | <span data-ttu-id="2d088-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d088-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2d088-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d088-121">Authorization</span></span> | <span data-ttu-id="2d088-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d088-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2d088-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="2d088-124">Content-type</span></span> | <span data-ttu-id="2d088-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d088-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d088-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d088-127">Request body</span></span>

<span data-ttu-id="2d088-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="2d088-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2d088-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="2d088-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2d088-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2d088-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2d088-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d088-131">Property</span></span>     | <span data-ttu-id="2d088-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d088-132">Type</span></span>        | <span data-ttu-id="2d088-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d088-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2d088-134">displayName</span><span class="sxs-lookup"><span data-stu-id="2d088-134">displayName</span></span>|<span data-ttu-id="2d088-135">String</span><span class="sxs-lookup"><span data-stu-id="2d088-135">String</span></span>| <span data-ttu-id="2d088-136">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="2d088-136">Display name for this policy.</span></span> |
|<span data-ttu-id="2d088-137">description</span><span class="sxs-lookup"><span data-stu-id="2d088-137">description</span></span>|<span data-ttu-id="2d088-138">String</span><span class="sxs-lookup"><span data-stu-id="2d088-138">String</span></span>| <span data-ttu-id="2d088-139">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="2d088-139">Description of this policy.</span></span>|
|<span data-ttu-id="2d088-140">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="2d088-140">blockMsolPowerShell</span></span>|<span data-ttu-id="2d088-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d088-141">Boolean</span></span>| <span data-ttu-id="2d088-142">Para desabilitar o uso do MSOL PowerShell defina essa propriedade como true.</span><span class="sxs-lookup"><span data-stu-id="2d088-142">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="2d088-143">A configuração como true também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2d088-143">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="2d088-144">Isso não afeta o Azure AD Connect ou o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2d088-144">This does not affect Azure AD Connect or Microsoft Graph.</span></span> |
|<span data-ttu-id="2d088-145">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="2d088-145">defaultUserRolePermissions</span></span>|[<span data-ttu-id="2d088-146">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="2d088-146">defaultUserRolePermissions</span></span>](../resources/defaultuserrolepermissions.md)| <span data-ttu-id="2d088-147">Especifica determinadas permissões personalizáveis para a função de usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="2d088-147">Specifies certain customizable permissions for default user role.</span></span> |
|<span data-ttu-id="2d088-148">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="2d088-148">allowedToUseSSPR</span></span>|<span data-ttu-id="2d088-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d088-149">Boolean</span></span>| <span data-ttu-id="2d088-150">Indica se o Self-Serve recurso de redefinição de senha pode ser usado por usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="2d088-150">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> |
|<span data-ttu-id="2d088-151">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="2d088-151">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="2d088-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d088-152">Boolean</span></span>| <span data-ttu-id="2d088-153">Indica se os usuários podem se inscrever para assinaturas baseadas em email.</span><span class="sxs-lookup"><span data-stu-id="2d088-153">Indicates whether users can sign up for email based subscriptions.</span></span> |
|<span data-ttu-id="2d088-154">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="2d088-154">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="2d088-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d088-155">Boolean</span></span>| <span data-ttu-id="2d088-156">Indica se um usuário pode ingressar no locatário por validação de email.</span><span class="sxs-lookup"><span data-stu-id="2d088-156">Indicates whether a user can join the tenant by email validation.</span></span> |
|<span data-ttu-id="2d088-157">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="2d088-157">allowInvitesFrom</span></span>|<span data-ttu-id="2d088-158">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2d088-158">String</span></span>|<span data-ttu-id="2d088-159">Indica quem pode convidar usuários externos para a organização.</span><span class="sxs-lookup"><span data-stu-id="2d088-159">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="2d088-160">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="2d088-160">Possible values are:</span></span><ul><li><span data-ttu-id="2d088-161">`none` – Impedir que todos, incluindo administradores, convidarem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="2d088-161">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="2d088-162">Configuração padrão para o governo dos EUA.</span><span class="sxs-lookup"><span data-stu-id="2d088-162">Default setting for US Government.</span></span></li><li><span data-ttu-id="2d088-163">`adminsAndGuestInviters` – Permitir que membros de administradores globais, administradores de usuários e funções do convidado de convidados convidarem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="2d088-163">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="2d088-164">`adminsGuestInvitersAndAllMembers` – Permitir que as funções de administrador acima e todos os outros membros da função de usuário convidem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="2d088-164">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="2d088-165">`everyone` – Permitir que todos na organização, incluindo usuários convidados, convidem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="2d088-165">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="2d088-166">Configuração padrão para todos os ambientes de nuvem, exceto o governo dos EUA.</span><span class="sxs-lookup"><span data-stu-id="2d088-166">Default setting for all cloud environments except US Government.</span></span></li></ul> |

## <a name="response"></a><span data-ttu-id="2d088-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d088-167">Response</span></span>

<span data-ttu-id="2d088-p109">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d088-p109">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d088-170">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2d088-170">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="2d088-171">Exemplo 1: atualizar ou definir o nível de acesso do usuário convidado para o locatário</span><span class="sxs-lookup"><span data-stu-id="2d088-171">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="2d088-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d088-172">Request</span></span>

<span data-ttu-id="2d088-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d088-173">The following is an example of the request.</span></span> <span data-ttu-id="2d088-174">Neste exemplo, o nível de acesso de convidado é modificado para o usuário convidado restrito.</span><span class="sxs-lookup"><span data-stu-id="2d088-174">In this example, guest access level is modified to Restricted Guest User.</span></span>


# <a name="http"></a>[<span data-ttu-id="2d088-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d088-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_guestUserLevel"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
  "allowEmailVerifiedUsersToJoinOrganization":false
}
```
# <a name="c"></a>[<span data-ttu-id="2d088-176">C#</span><span class="sxs-lookup"><span data-stu-id="2d088-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-guestuserlevel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d088-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d088-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-guestuserlevel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d088-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d088-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-guestuserlevel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d088-179">Java</span><span class="sxs-lookup"><span data-stu-id="2d088-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-guestuserlevel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2d088-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d088-180">Response</span></span>

<span data-ttu-id="2d088-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2d088-181">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-block-msol-powershell-in-tenant"></a><span data-ttu-id="2d088-182">Exemplo 2: bloquear o MSOL PowerShell no locatário</span><span class="sxs-lookup"><span data-stu-id="2d088-182">Example 2: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="2d088-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d088-183">Request</span></span>

<span data-ttu-id="2d088-184">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d088-184">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2d088-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d088-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_blockMSOLPowerShell"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "blockMsolPowerShell":true
}
```
# <a name="c"></a>[<span data-ttu-id="2d088-186">C#</span><span class="sxs-lookup"><span data-stu-id="2d088-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d088-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d088-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d088-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d088-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d088-189">Java</span><span class="sxs-lookup"><span data-stu-id="2d088-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-blockmsolpowershell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2d088-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d088-190">Response</span></span>

<span data-ttu-id="2d088-191">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2d088-191">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="2d088-192">Exemplo 3: desabilitar a permissão de função de usuário padrão para criar aplicativos</span><span class="sxs-lookup"><span data-stu-id="2d088-192">Example 3: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="2d088-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d088-193">Request</span></span>

<span data-ttu-id="2d088-194">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d088-194">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2d088-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d088-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_applications"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions":{
      "allowedToCreateApps":false
   }
}
```
# <a name="c"></a>[<span data-ttu-id="2d088-196">C#</span><span class="sxs-lookup"><span data-stu-id="2d088-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d088-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d088-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d088-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d088-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d088-199">Java</span><span class="sxs-lookup"><span data-stu-id="2d088-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2d088-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d088-200">Response</span></span>

<span data-ttu-id="2d088-201">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2d088-201">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-4-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="2d088-202">Exemplo 4: habilitar a função de usuário padrão para usar Self-Serve recurso de redefinição de senha</span><span class="sxs-lookup"><span data-stu-id="2d088-202">Example 4: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="2d088-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d088-203">Request</span></span>

<span data-ttu-id="2d088-204">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d088-204">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2d088-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d088-205">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_SSPR"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "allowedToUseSSPR":true
}
```
# <a name="c"></a>[<span data-ttu-id="2d088-206">C#</span><span class="sxs-lookup"><span data-stu-id="2d088-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d088-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d088-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d088-208">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d088-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d088-209">Java</span><span class="sxs-lookup"><span data-stu-id="2d088-209">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-sspr-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2d088-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d088-210">Response</span></span>

<span data-ttu-id="2d088-211">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2d088-211">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-disable-user-consent-to-apps-for-default-user-role"></a><span data-ttu-id="2d088-212">Exemplo 5: desabilitar o consentimento do usuário para os aplicativos para a função de usuário padrão</span><span class="sxs-lookup"><span data-stu-id="2d088-212">Example 5: Disable user consent to apps for default user role</span></span>

#### <a name="request"></a><span data-ttu-id="2d088-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d088-213">Request</span></span>

<span data-ttu-id="2d088-214">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d088-214">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2d088-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d088-215">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_disableUserConsent"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions": {
      "permissionGrantPoliciesAssigned": []
   }
}
```
# <a name="c"></a>[<span data-ttu-id="2d088-216">C#</span><span class="sxs-lookup"><span data-stu-id="2d088-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-disableuserconsent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d088-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d088-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-disableuserconsent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d088-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d088-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-disableuserconsent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d088-219">Java</span><span class="sxs-lookup"><span data-stu-id="2d088-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-disableuserconsent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2d088-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d088-220">Response</span></span>

<span data-ttu-id="2d088-221">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2d088-221">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-6-enable-user-consent-to-apps-subject-to-app-consent-policy"></a><span data-ttu-id="2d088-222">Exemplo 6: habilitar o consentimento do usuário para aplicativos, sujeito à política de consentimento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d088-222">Example 6: Enable user consent to apps, subject to app consent policy</span></span>

#### <a name="request"></a><span data-ttu-id="2d088-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d088-223">Request</span></span>

<span data-ttu-id="2d088-224">Veja a seguir um exemplo da solicitação que permite o consentimento do usuário para os aplicativos, sujeito à política de [consentimento de aplicativo](/azure/active-directory/manage-apps/manage-app-consent-policies) interna `microsoft-user-default-low` , que permite as permissões delegadas "baixa", para aplicativos clientes de editores verificados ou registrados no mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="2d088-224">The following is an example of the request that allows user consent to apps, subject to the built-in [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low`, which allows delegated permissions classified "low", for client apps from verified publishers or registered in the same tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="2d088-225">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d088-225">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_enableUserConsentLow"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions": {
      "permissionGrantPoliciesAssigned": [
         "managePermissionGrantsForSelf.microsoft-user-default-low"
      ]
   }
}
```
# <a name="c"></a>[<span data-ttu-id="2d088-226">C#</span><span class="sxs-lookup"><span data-stu-id="2d088-226">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-enableuserconsentlow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d088-227">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d088-227">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-enableuserconsentlow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d088-228">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d088-228">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-enableuserconsentlow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d088-229">Java</span><span class="sxs-lookup"><span data-stu-id="2d088-229">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-enableuserconsentlow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2d088-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d088-230">Response</span></span>

<span data-ttu-id="2d088-231">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2d088-231">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationpolicy"
} -->

```http
HTTP/1.1 204 No Content
```
