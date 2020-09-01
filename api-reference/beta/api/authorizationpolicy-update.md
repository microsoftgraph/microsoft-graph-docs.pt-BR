---
title: Atualizar AuthorizationPolicy
description: Atualize as propriedades do objeto authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 23263f65277f7635a5e03b1a955b6300845d2731
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319369"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="9f13a-103">Atualizar authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="9f13a-103">Update authorizationPolicy</span></span>

<span data-ttu-id="9f13a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f13a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f13a-105">Atualiza as propriedades de um objeto [authorizationPolicy](../resources/authorizationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="9f13a-105">Update the properties of a [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f13a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f13a-106">Permissions</span></span>

<span data-ttu-id="9f13a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f13a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f13a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f13a-109">Permission type</span></span>                        | <span data-ttu-id="9f13a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f13a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9f13a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f13a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f13a-112">Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="9f13a-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="9f13a-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f13a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f13a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f13a-114">Not supported.</span></span> |
| <span data-ttu-id="9f13a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f13a-115">Application</span></span>                            | <span data-ttu-id="9f13a-116">Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="9f13a-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f13a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f13a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="9f13a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f13a-118">Request headers</span></span>

| <span data-ttu-id="9f13a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9f13a-119">Name</span></span>       | <span data-ttu-id="9f13a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f13a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9f13a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f13a-121">Authorization</span></span> | <span data-ttu-id="9f13a-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="9f13a-122">Bearer {token}</span></span> |
| <span data-ttu-id="9f13a-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="9f13a-123">Content-type</span></span> | <span data-ttu-id="9f13a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9f13a-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f13a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f13a-125">Request body</span></span>

<span data-ttu-id="9f13a-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="9f13a-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9f13a-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="9f13a-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9f13a-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9f13a-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9f13a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f13a-129">Property</span></span>     | <span data-ttu-id="9f13a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f13a-130">Type</span></span>        | <span data-ttu-id="9f13a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f13a-131">Description</span></span> |
|:-------------|:------------|:------------|  
|<span data-ttu-id="9f13a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="9f13a-132">displayName</span></span>|<span data-ttu-id="9f13a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f13a-133">String</span></span>| <span data-ttu-id="9f13a-134">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="9f13a-134">Display name for this policy.</span></span> |  
|<span data-ttu-id="9f13a-135">descrição</span><span class="sxs-lookup"><span data-stu-id="9f13a-135">description</span></span>|<span data-ttu-id="9f13a-136">String</span><span class="sxs-lookup"><span data-stu-id="9f13a-136">String</span></span>| <span data-ttu-id="9f13a-137">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="9f13a-137">Description of this policy.</span></span> |  
|<span data-ttu-id="9f13a-138">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="9f13a-138">guestUserRoleId</span></span>|<span data-ttu-id="9f13a-139">Guid</span><span class="sxs-lookup"><span data-stu-id="9f13a-139">Guid</span></span>| <span data-ttu-id="9f13a-140">Representa o modelo de função para a função que deve ser concedida ao usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="9f13a-140">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="9f13a-141">Consulte [list unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) para encontrar a lista de modelos de função disponíveis.</span><span class="sxs-lookup"><span data-stu-id="9f13a-141">Refer to [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) to find the list of available role templates.</span></span> <span data-ttu-id="9f13a-142">Somente as funções suportadas hoje são usuário (a0b1b346-4d3e-4e8b-98f8-753987be4970), usuário convidado (10dae51f-b6af-4016-8d66-8c2a99b929b3) e usuário convidado restrito (2af84b1e-32c8-42b7-82bc-daa82404023b).</span><span class="sxs-lookup"><span data-stu-id="9f13a-142">Only supported roles today are User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="9f13a-143">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="9f13a-143">enabledPreviewFeatures</span></span>|<span data-ttu-id="9f13a-144">Coleção (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="9f13a-144">Collection(string)</span></span>| <span data-ttu-id="9f13a-145">Lista de recursos habilitados para visualização privada no locatário.</span><span class="sxs-lookup"><span data-stu-id="9f13a-145">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="9f13a-146">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="9f13a-146">blockMsolPowerShell</span></span>|<span data-ttu-id="9f13a-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="9f13a-147">Boolean</span></span>| <span data-ttu-id="9f13a-148">Para desabilitar o uso do MSOL PowerShell, defina essa propriedade como `true` .</span><span class="sxs-lookup"><span data-stu-id="9f13a-148">To disable the use of MSOL PowerShell, set this property to `true`.</span></span> <span data-ttu-id="9f13a-149">A configuração `true` também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSol PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9f13a-149">Setting to `true` will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="9f13a-150">Isso não afeta o Azure AD Connect ou o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9f13a-150">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="9f13a-151">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="9f13a-151">defaultUserRolePermissions</span></span>|[<span data-ttu-id="9f13a-152">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="9f13a-152">defaultUserRolePermissions</span></span>](../resources/defaultUserRolePermissions.md)| <span data-ttu-id="9f13a-153">Especifica determinadas permissões personalizáveis para a função de usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="9f13a-153">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="9f13a-154">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="9f13a-154">allowedToUseSSPR</span></span>|<span data-ttu-id="9f13a-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="9f13a-155">Boolean</span></span>| <span data-ttu-id="9f13a-156">Indica se o recurso de redefinição de senha de autoatendimento pode ser usado por usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="9f13a-156">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="9f13a-157">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="9f13a-157">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="9f13a-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="9f13a-158">Boolean</span></span>| <span data-ttu-id="9f13a-159">Indica se os usuários podem se inscrever para assinaturas baseadas em email.</span><span class="sxs-lookup"><span data-stu-id="9f13a-159">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="9f13a-160">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="9f13a-160">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="9f13a-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="9f13a-161">Boolean</span></span>| <span data-ttu-id="9f13a-162">Indica se um usuário pode ingressar no locatário por validação de email.</span><span class="sxs-lookup"><span data-stu-id="9f13a-162">Indicates whether a user can join the tenant by email validation.</span></span> | 

## <a name="response"></a><span data-ttu-id="9f13a-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f13a-163">Response</span></span>

<span data-ttu-id="9f13a-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f13a-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f13a-166">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9f13a-166">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="9f13a-167">Exemplo 1: atualizar ou definir o nível de acesso do usuário convidado para o locatário</span><span class="sxs-lookup"><span data-stu-id="9f13a-167">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="9f13a-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f13a-168">Request</span></span>

<span data-ttu-id="9f13a-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f13a-169">The following is an example of the request.</span></span> <span data-ttu-id="9f13a-170">Neste exemplo, o nível de acesso de convidado é modificado para o usuário convidado restrito.</span><span class="sxs-lookup"><span data-stu-id="9f13a-170">In this example, guest access level is modified to Restricted Guest User.</span></span>

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
#### <a name="response"></a><span data-ttu-id="9f13a-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f13a-171">Response</span></span>

<span data-ttu-id="9f13a-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f13a-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content

```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a><span data-ttu-id="9f13a-173">Exemplo 2: habilitar novo recurso para visualização no locatário</span><span class="sxs-lookup"><span data-stu-id="9f13a-173">Example 2: Enable new feature for preview on tenant</span></span>

#### <a name="request"></a><span data-ttu-id="9f13a-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f13a-174">Request</span></span>

<span data-ttu-id="9f13a-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f13a-175">The following is an example of the request.</span></span>

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
#### <a name="response"></a><span data-ttu-id="9f13a-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f13a-176">Response</span></span>

<span data-ttu-id="9f13a-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f13a-177">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```


### <a name="example-3-block-msol-powershell-in-tenant"></a><span data-ttu-id="9f13a-178">Exemplo 3: bloquear o MSOL PowerShell no locatário</span><span class="sxs-lookup"><span data-stu-id="9f13a-178">Example 3: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="9f13a-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f13a-179">Request</span></span>

<span data-ttu-id="9f13a-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f13a-180">The following is an example of the request.</span></span>

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
#### <a name="response"></a><span data-ttu-id="9f13a-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f13a-181">Response</span></span>

<span data-ttu-id="9f13a-182">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f13a-182">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-4-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="9f13a-183">Exemplo 4: desabilitar a permissão de função de usuário padrão para criar aplicativos</span><span class="sxs-lookup"><span data-stu-id="9f13a-183">Example 4: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="9f13a-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f13a-184">Request</span></span>

<span data-ttu-id="9f13a-185">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f13a-185">The following is an example of the request.</span></span>

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
#### <a name="response"></a><span data-ttu-id="9f13a-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f13a-186">Response</span></span>

<span data-ttu-id="9f13a-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f13a-187">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="9f13a-188">Exemplo 5: habilitar a função de usuário padrão para usar o recurso de redefinição de senha de autoatendimento</span><span class="sxs-lookup"><span data-stu-id="9f13a-188">Example 5: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="9f13a-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f13a-189">Request</span></span>

<span data-ttu-id="9f13a-190">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f13a-190">The following is an example of the request.</span></span>

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
#### <a name="response"></a><span data-ttu-id="9f13a-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f13a-191">Response</span></span>

<span data-ttu-id="9f13a-192">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f13a-192">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
