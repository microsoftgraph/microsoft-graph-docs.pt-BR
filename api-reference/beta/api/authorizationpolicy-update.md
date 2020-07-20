---
title: Atualizar AuthorizationPolicy
description: Atualize as propriedades do objeto authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac605e93603cb39491fd980e78a9b0f0026541eb
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492194"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="4e6be-103">Atualizar authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="4e6be-103">Update authorizationPolicy</span></span>

<span data-ttu-id="4e6be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e6be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e6be-105">Atualiza as propriedades de um objeto [authorizationPolicy](../resources/authorizationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="4e6be-105">Update the properties of a [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e6be-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4e6be-106">Permissions</span></span>

<span data-ttu-id="4e6be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e6be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4e6be-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e6be-109">Permission type</span></span>                        | <span data-ttu-id="4e6be-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e6be-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4e6be-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e6be-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e6be-112">Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="4e6be-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="4e6be-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e6be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e6be-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e6be-114">Not supported.</span></span> |
| <span data-ttu-id="4e6be-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e6be-115">Application</span></span>                            | <span data-ttu-id="4e6be-116">Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="4e6be-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e6be-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e6be-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="4e6be-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e6be-118">Request headers</span></span>

| <span data-ttu-id="4e6be-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4e6be-119">Name</span></span>       | <span data-ttu-id="4e6be-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e6be-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4e6be-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e6be-121">Authorization</span></span> | <span data-ttu-id="4e6be-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="4e6be-122">Bearer {token}</span></span> |
| <span data-ttu-id="4e6be-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="4e6be-123">Content-type</span></span> | <span data-ttu-id="4e6be-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4e6be-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e6be-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e6be-125">Request body</span></span>

<span data-ttu-id="4e6be-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="4e6be-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4e6be-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="4e6be-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4e6be-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4e6be-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4e6be-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e6be-129">Property</span></span>     | <span data-ttu-id="4e6be-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e6be-130">Type</span></span>        | <span data-ttu-id="4e6be-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e6be-131">Description</span></span> |
|:-------------|:------------|:------------|  
|<span data-ttu-id="4e6be-132">displayName</span><span class="sxs-lookup"><span data-stu-id="4e6be-132">displayName</span></span>|<span data-ttu-id="4e6be-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e6be-133">String</span></span>| <span data-ttu-id="4e6be-134">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="4e6be-134">Display name for this policy.</span></span> |  
|<span data-ttu-id="4e6be-135">description</span><span class="sxs-lookup"><span data-stu-id="4e6be-135">description</span></span>|<span data-ttu-id="4e6be-136">String</span><span class="sxs-lookup"><span data-stu-id="4e6be-136">String</span></span>| <span data-ttu-id="4e6be-137">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="4e6be-137">Description of this policy.</span></span> |  
|<span data-ttu-id="4e6be-138">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="4e6be-138">guestUserRoleId</span></span>|<span data-ttu-id="4e6be-139">Guid</span><span class="sxs-lookup"><span data-stu-id="4e6be-139">Guid</span></span>| <span data-ttu-id="4e6be-140">Representa o modelo de função para a função que deve ser concedida ao usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="4e6be-140">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="4e6be-141">Consulte [list unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) para encontrar a lista de modelos de função disponíveis.</span><span class="sxs-lookup"><span data-stu-id="4e6be-141">Refer to [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) to find the list of available role templates.</span></span> <span data-ttu-id="4e6be-142">Somente as funções suportadas hoje são usuário (a0b1b346-4d3e-4e8b-98f8-753987be4970), usuário convidado (10dae51f-b6af-4016-8d66-8c2a99b929b3) e usuário convidado restrito (2af84b1e-32c8-42b7-82bc-daa82404023b).</span><span class="sxs-lookup"><span data-stu-id="4e6be-142">Only supported roles today are User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="4e6be-143">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="4e6be-143">enabledPreviewFeatures</span></span>|<span data-ttu-id="4e6be-144">Coleção (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="4e6be-144">Collection(string)</span></span>| <span data-ttu-id="4e6be-145">Lista de recursos habilitados para visualização privada no locatário.</span><span class="sxs-lookup"><span data-stu-id="4e6be-145">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="4e6be-146">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="4e6be-146">blockMsolPowerShell</span></span>|<span data-ttu-id="4e6be-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e6be-147">Boolean</span></span>| <span data-ttu-id="4e6be-148">Para desabilitar o uso do MSOL PowerShell, defina essa propriedade como `true` .</span><span class="sxs-lookup"><span data-stu-id="4e6be-148">To disable the use of MSOL PowerShell, set this property to `true`.</span></span> <span data-ttu-id="4e6be-149">A configuração `true` também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSol PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4e6be-149">Setting to `true` will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="4e6be-150">Isso não afeta o Azure AD Connect ou o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4e6be-150">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 

## <a name="response"></a><span data-ttu-id="4e6be-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e6be-151">Response</span></span>

<span data-ttu-id="4e6be-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e6be-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4e6be-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4e6be-154">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="4e6be-155">Exemplo 1: atualizar ou definir o nível de acesso do usuário convidado para o locatário</span><span class="sxs-lookup"><span data-stu-id="4e6be-155">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="4e6be-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e6be-156">Request</span></span>

<span data-ttu-id="4e6be-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e6be-157">The following is an example of the request.</span></span> <span data-ttu-id="4e6be-158">Neste exemplo, o nível de acesso de convidado é modificado para o usuário convidado restrito.</span><span class="sxs-lookup"><span data-stu-id="4e6be-158">In this example, guest access level is modified to Restricted Guest User.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "guestUserRole": "2af84b1e-32c8-42b7-82bc-daa82404023b"
}

```
#### <a name="response"></a><span data-ttu-id="4e6be-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e6be-159">Response</span></span>

<span data-ttu-id="4e6be-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4e6be-160">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content

```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a><span data-ttu-id="4e6be-161">Exemplo 2: habilitar novo recurso para visualização no locatário</span><span class="sxs-lookup"><span data-stu-id="4e6be-161">Example 2: Enable new feature for preview on tenant</span></span>

#### <a name="request"></a><span data-ttu-id="4e6be-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e6be-162">Request</span></span>

<span data-ttu-id="4e6be-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e6be-163">The following is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "enabledPreviewFeatures": ["assignGroupsToRoles"]
}

```
#### <a name="response"></a><span data-ttu-id="4e6be-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e6be-164">Response</span></span>

<span data-ttu-id="4e6be-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4e6be-165">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```


### <a name="example-3-block-msol-powershell-in-tenant"></a><span data-ttu-id="4e6be-166">Exemplo 3: bloquear o MSOL PowerShell no locatário</span><span class="sxs-lookup"><span data-stu-id="4e6be-166">Example 3: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="4e6be-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e6be-167">Request</span></span>

<span data-ttu-id="4e6be-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e6be-168">The following is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "blockMsolPowerShell": true
}

```
#### <a name="response"></a><span data-ttu-id="4e6be-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e6be-169">Response</span></span>

<span data-ttu-id="4e6be-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4e6be-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
