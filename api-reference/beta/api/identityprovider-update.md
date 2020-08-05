---
title: Atualizar identityProvider
description: Atualizar propriedades de um identityprovider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: be8c24c1c34dca1803bd1c527e043a5c52ac5e10
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566667"
---
# <a name="update-identityprovider"></a><span data-ttu-id="fba42-103">Atualizar identityProvider</span><span class="sxs-lookup"><span data-stu-id="fba42-103">Update identityProvider</span></span>

<span data-ttu-id="fba42-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fba42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fba42-105">Atualiza as propriedades de um objeto [identityprovider](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="fba42-105">Update the properties of an [identityProvider](../resources/identityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fba42-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fba42-106">Permissions</span></span>

<span data-ttu-id="fba42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fba42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fba42-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fba42-109">Permission type</span></span>      | <span data-ttu-id="fba42-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fba42-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fba42-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fba42-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fba42-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fba42-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="fba42-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fba42-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fba42-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fba42-114">Not supported.</span></span>|
|<span data-ttu-id="fba42-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fba42-115">Application</span></span>| <span data-ttu-id="fba42-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fba42-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="fba42-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="fba42-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="fba42-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="fba42-118">Global administrator</span></span>
* <span data-ttu-id="fba42-119">Administrador do provedor de identidade externa</span><span class="sxs-lookup"><span data-stu-id="fba42-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="fba42-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fba42-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fba42-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fba42-121">Request headers</span></span>

|<span data-ttu-id="fba42-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fba42-122">Name</span></span>|<span data-ttu-id="fba42-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fba42-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fba42-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fba42-124">Authorization</span></span>|<span data-ttu-id="fba42-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fba42-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fba42-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fba42-127">Content-Type</span></span>|<span data-ttu-id="fba42-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fba42-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fba42-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fba42-130">Request body</span></span>

<span data-ttu-id="fba42-131">No corpo da solicitação, forneça um objeto JSON com uma ou mais propriedades que precisam ser atualizadas para um objeto [identityprovider](../resources/identityprovider.md) ou [openIdConnectProvider](../resources/openidconnectprovider.md) (somente para o Azure ad B2C).</span><span class="sxs-lookup"><span data-stu-id="fba42-131">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object.</span></span>

### <a name="identityprovider-object"></a><span data-ttu-id="fba42-132">objeto identityprovider</span><span class="sxs-lookup"><span data-stu-id="fba42-132">identityProvider object</span></span>

|<span data-ttu-id="fba42-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fba42-133">Property</span></span>|<span data-ttu-id="fba42-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="fba42-134">Type</span></span>|<span data-ttu-id="fba42-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="fba42-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fba42-136">clientId</span><span class="sxs-lookup"><span data-stu-id="fba42-136">clientId</span></span>|<span data-ttu-id="fba42-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fba42-137">String</span></span>|<span data-ttu-id="fba42-138">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fba42-138">The client ID for the application.</span></span> <span data-ttu-id="fba42-139">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fba42-139">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="fba42-140">clientSecret</span><span class="sxs-lookup"><span data-stu-id="fba42-140">clientSecret</span></span>|<span data-ttu-id="fba42-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fba42-141">String</span></span>|<span data-ttu-id="fba42-142">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fba42-142">The client secret for the application.</span></span> <span data-ttu-id="fba42-143">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fba42-143">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="fba42-144">nome</span><span class="sxs-lookup"><span data-stu-id="fba42-144">name</span></span>|<span data-ttu-id="fba42-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fba42-145">String</span></span>|<span data-ttu-id="fba42-146">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fba42-146">The display name of the identity provider.</span></span>|
|<span data-ttu-id="fba42-147">tipo</span><span class="sxs-lookup"><span data-stu-id="fba42-147">type</span></span>|<span data-ttu-id="fba42-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fba42-148">String</span></span>|<span data-ttu-id="fba42-149">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fba42-149">The identity provider type.</span></span><ul><span data-ttu-id="fba42-150">Para o cenário B2B:</span><span class="sxs-lookup"><span data-stu-id="fba42-150">For B2B scenario:</span></span><li/><span data-ttu-id="fba42-151">Google</span><span class="sxs-lookup"><span data-stu-id="fba42-151">Google</span></span><li/><span data-ttu-id="fba42-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="fba42-152">Facebook</span></span></ul><ul><span data-ttu-id="fba42-153">Para o cenário B2C:</span><span class="sxs-lookup"><span data-stu-id="fba42-153">For B2C scenario:</span></span><li/><span data-ttu-id="fba42-154">Microsoft</span><span class="sxs-lookup"><span data-stu-id="fba42-154">Microsoft</span></span><li/><span data-ttu-id="fba42-155">Google</span><span class="sxs-lookup"><span data-stu-id="fba42-155">Google</span></span><li/><span data-ttu-id="fba42-156">Amazon</span><span class="sxs-lookup"><span data-stu-id="fba42-156">Amazon</span></span><li/><span data-ttu-id="fba42-157">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="fba42-157">LinkedIn</span></span><li/><span data-ttu-id="fba42-158">Facebook</span><span class="sxs-lookup"><span data-stu-id="fba42-158">Facebook</span></span><li/><span data-ttu-id="fba42-159">GitHub</span><span class="sxs-lookup"><span data-stu-id="fba42-159">GitHub</span></span><li/><span data-ttu-id="fba42-160">Twitter</span><span class="sxs-lookup"><span data-stu-id="fba42-160">Twitter</span></span><li/><span data-ttu-id="fba42-161">Weibo</span><span class="sxs-lookup"><span data-stu-id="fba42-161">Weibo</span></span><li/><span data-ttu-id="fba42-162">QQ</span><span class="sxs-lookup"><span data-stu-id="fba42-162">QQ</span></span><li/><span data-ttu-id="fba42-163">WeChat</span><span class="sxs-lookup"><span data-stu-id="fba42-163">WeChat</span></span><li/><span data-ttu-id="fba42-164">OpenIDConnect</span><span class="sxs-lookup"><span data-stu-id="fba42-164">OpenIDConnect</span></span></ul>|

### <a name="openidconnectprovider-object"></a><span data-ttu-id="fba42-165">objeto openIdConnectProvider</span><span class="sxs-lookup"><span data-stu-id="fba42-165">openIdConnectProvider object</span></span>

|<span data-ttu-id="fba42-166">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fba42-166">Property</span></span>|<span data-ttu-id="fba42-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="fba42-167">Type</span></span>|<span data-ttu-id="fba42-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="fba42-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fba42-169">clientId</span><span class="sxs-lookup"><span data-stu-id="fba42-169">clientId</span></span>|<span data-ttu-id="fba42-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fba42-170">String</span></span>|<span data-ttu-id="fba42-171">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fba42-171">The client ID for the application.</span></span> <span data-ttu-id="fba42-172">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fba42-172">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="fba42-173">clientSecret</span><span class="sxs-lookup"><span data-stu-id="fba42-173">clientSecret</span></span>|<span data-ttu-id="fba42-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fba42-174">String</span></span>|<span data-ttu-id="fba42-175">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fba42-175">The client secret for the application.</span></span> <span data-ttu-id="fba42-176">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fba42-176">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="fba42-177">nome</span><span class="sxs-lookup"><span data-stu-id="fba42-177">name</span></span>|<span data-ttu-id="fba42-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fba42-178">String</span></span>|<span data-ttu-id="fba42-179">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fba42-179">The display name of the identity provider.</span></span>|
|<span data-ttu-id="fba42-180">tipo</span><span class="sxs-lookup"><span data-stu-id="fba42-180">type</span></span>|<span data-ttu-id="fba42-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fba42-181">String</span></span>|<span data-ttu-id="fba42-182">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fba42-182">The identity provider type.</span></span> <span data-ttu-id="fba42-183">O valor deve ser `OpenIdConnect` .</span><span class="sxs-lookup"><span data-stu-id="fba42-183">The value must be `OpenIdConnect`.</span></span>|
|<span data-ttu-id="fba42-184">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="fba42-184">claimsMapping</span></span>|[<span data-ttu-id="fba42-185">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="fba42-185">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="fba42-186">Depois que o provedor OIDC envia um token de ID de volta para o Azure AD, o Azure AD precisa ser capaz de mapear as declarações do token recebido para as declarações que o Azure AD reconhece e usa.</span><span class="sxs-lookup"><span data-stu-id="fba42-186">After the OIDC provider sends an ID token back to Azure AD, Azure AD needs to be able to map the claims from the received token to the claims that Azure AD recognizes and uses.</span></span> <span data-ttu-id="fba42-187">Esse tipo complexo captura esse mapeamento.</span><span class="sxs-lookup"><span data-stu-id="fba42-187">This complex type captures that mapping.</span></span>|
|<span data-ttu-id="fba42-188">domainHint</span><span class="sxs-lookup"><span data-stu-id="fba42-188">domainHint</span></span>|<span data-ttu-id="fba42-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fba42-189">String</span></span>|<span data-ttu-id="fba42-190">A dica de domínio pode ser usada para saltar diretamente para a página de entrada do provedor de identidade especificado, em vez de fazer com que o usuário faça uma seleção entre a lista de provedores de identidade disponíveis.</span><span class="sxs-lookup"><span data-stu-id="fba42-190">The domain hint can be used to skip directly to the sign in page of the specified identity provider, instead of having the user make a selection among the list of available identity providers.</span></span>|
|<span data-ttu-id="fba42-191">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="fba42-191">metadataUrl</span></span>|<span data-ttu-id="fba42-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fba42-192">String</span></span>|<span data-ttu-id="fba42-193">A URL para o documento de metadados do provedor de identidade de conexão de Open ID.</span><span class="sxs-lookup"><span data-stu-id="fba42-193">The URL for the metadata document of the Open Id Connect identity provider.</span></span>|
|<span data-ttu-id="fba42-194">responsemode</span><span class="sxs-lookup"><span data-stu-id="fba42-194">responseMode</span></span>|<span data-ttu-id="fba42-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fba42-195">String</span></span>|<span data-ttu-id="fba42-196">Define o método que deve ser usado para enviar os dados de volta do provedor de identidade personalizado para o Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="fba42-196">Defines the method that should be used to send the data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="fba42-197">Os seguintes modos de resposta podem ser usados:</span><span class="sxs-lookup"><span data-stu-id="fba42-197">The following response modes can be used:</span></span> <ul><li/><span data-ttu-id="fba42-198">`form_post`: Este modo de resposta é recomendado para melhor segurança.</span><span class="sxs-lookup"><span data-stu-id="fba42-198">`form_post` : This response mode is recommended for best security.</span></span> <span data-ttu-id="fba42-199">A resposta é transmitida por meio do método HTTP POST, com o código ou token codificado no corpo usando o formato application/x-www-form-urlencoded.</span><span class="sxs-lookup"><span data-stu-id="fba42-199">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span><li/><span data-ttu-id="fba42-200">`query`: O código ou token é retornado como um parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="fba42-200">`query` : The code or token is returned as a query parameter.</span></span></ul>|
|<span data-ttu-id="fba42-201">responseType</span><span class="sxs-lookup"><span data-stu-id="fba42-201">responseType</span></span>|<span data-ttu-id="fba42-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fba42-202">String</span></span>|<span data-ttu-id="fba42-203">Descreve que tipo de informação é enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="fba42-203">Describes what kind of information is sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="fba42-204">Os seguintes tipos de resposta podem ser usados:</span><span class="sxs-lookup"><span data-stu-id="fba42-204">The following response types can be used:</span></span><ul><li/> <span data-ttu-id="fba42-205">`code`: Conforme o fluxo do código de autorização, um código será retornado de volta para o Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="fba42-205">`code` : As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="fba42-206">O Azure AD B2C continua a chamar o token_endpoint para trocar o código do token.</span><span class="sxs-lookup"><span data-stu-id="fba42-206">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span><li/> <span data-ttu-id="fba42-207">`id_token`: Um token de ID retorna de volta para o Azure AD B2C do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="fba42-207">`id_token` : An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span> <li/><span data-ttu-id="fba42-208">`token`: Um token de acesso retorna de volta para o Azure AD B2C do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="fba42-208">`token` : An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="fba42-209">(Esse valor não é suportado pelo Azure AD B2C no momento)</span><span class="sxs-lookup"><span data-stu-id="fba42-209">(This value is not supported by Azure AD B2C at the moment)</span></span></ul>|
|<span data-ttu-id="fba42-210">escopo</span><span class="sxs-lookup"><span data-stu-id="fba42-210">scope</span></span>|<span data-ttu-id="fba42-211">String</span><span class="sxs-lookup"><span data-stu-id="fba42-211">String</span></span>|<span data-ttu-id="fba42-212">Escopo define as informações e permissões que você pretende coletar de seu provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="fba42-212">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="fba42-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="fba42-213">Response</span></span>

<span data-ttu-id="fba42-214">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fba42-214">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="fba42-215">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="fba42-215">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="fba42-216">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fba42-216">Examples</span></span>

### <a name="example-1-update-a-specific-identityprovider"></a><span data-ttu-id="fba42-217">Exemplo 1: atualizar um **identityprovider** específico</span><span class="sxs-lookup"><span data-stu-id="fba42-217">Example 1: Update a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="fba42-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fba42-218">Request</span></span>

<span data-ttu-id="fba42-219">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fba42-219">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fba42-220">HTTP</span><span class="sxs-lookup"><span data-stu-id="fba42-220">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
  "clientSecret": "1111111111111"
}
```
# <a name="c"></a>[<span data-ttu-id="fba42-221">C#</span><span class="sxs-lookup"><span data-stu-id="fba42-221">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fba42-222">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fba42-222">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fba42-223">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fba42-223">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fba42-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="fba42-224">Response</span></span>

<span data-ttu-id="fba42-225">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fba42-225">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-update-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="fba42-226">Exemplo 2: atualizar um **openIDConnectProvider** específico (somente para o Azure ad B2C)</span><span class="sxs-lookup"><span data-stu-id="fba42-226">Example 2: Update a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="fba42-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fba42-227">Request</span></span>

<span data-ttu-id="fba42-228">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fba42-228">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fba42-229">HTTP</span><span class="sxs-lookup"><span data-stu-id="fba42-229">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_openidconnectprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identityProviders/OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a
Content-type: application/json
Content-length: 41

{
  "responseType": "id_token"
}
```
# <a name="c"></a>[<span data-ttu-id="fba42-230">C#</span><span class="sxs-lookup"><span data-stu-id="fba42-230">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openidconnectprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fba42-231">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fba42-231">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openidconnectprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fba42-232">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fba42-232">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openidconnectprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fba42-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="fba42-233">Response</span></span>

<span data-ttu-id="fba42-234">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fba42-234">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
