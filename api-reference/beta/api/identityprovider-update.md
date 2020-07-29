---
title: Atualizar identityProvider
description: Atualizar propriedades de um identityprovider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6bd2944211312c1b5440390f7a1c7a84de205e9f
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509697"
---
# <a name="update-identityprovider"></a><span data-ttu-id="391cb-103">Atualizar identityProvider</span><span class="sxs-lookup"><span data-stu-id="391cb-103">Update identityProvider</span></span>

<span data-ttu-id="391cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="391cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="391cb-105">Atualiza as propriedades de um objeto [identityprovider](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="391cb-105">Update the properties of an [identityProvider](../resources/identityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="391cb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="391cb-106">Permissions</span></span>

<span data-ttu-id="391cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="391cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="391cb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="391cb-109">Permission type</span></span>      | <span data-ttu-id="391cb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="391cb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="391cb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="391cb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="391cb-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="391cb-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="391cb-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="391cb-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="391cb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="391cb-114">Not supported.</span></span>|
|<span data-ttu-id="391cb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="391cb-115">Application</span></span>| <span data-ttu-id="391cb-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="391cb-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="391cb-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="391cb-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="391cb-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="391cb-118">Global administrator</span></span>
* <span data-ttu-id="391cb-119">Administrador do provedor de identidade externa</span><span class="sxs-lookup"><span data-stu-id="391cb-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="391cb-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="391cb-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="391cb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="391cb-121">Request headers</span></span>

|<span data-ttu-id="391cb-122">Nome</span><span class="sxs-lookup"><span data-stu-id="391cb-122">Name</span></span>|<span data-ttu-id="391cb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="391cb-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="391cb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="391cb-124">Authorization</span></span>|<span data-ttu-id="391cb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="391cb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="391cb-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="391cb-127">Content-Type</span></span>|<span data-ttu-id="391cb-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="391cb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="391cb-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="391cb-130">Request body</span></span>

<span data-ttu-id="391cb-131">No corpo da solicitação, forneça um objeto JSON com uma ou mais propriedades que precisam ser atualizadas para um objeto [identityprovider](../resources/identityprovider.md) ou [openIdConnectProvider](../resources/openidconnectprovider.md) (somente para o Azure ad B2C).</span><span class="sxs-lookup"><span data-stu-id="391cb-131">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object.</span></span>

### <a name="identityprovider-object"></a><span data-ttu-id="391cb-132">objeto identityprovider</span><span class="sxs-lookup"><span data-stu-id="391cb-132">identityProvider object</span></span>

|<span data-ttu-id="391cb-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="391cb-133">Property</span></span>|<span data-ttu-id="391cb-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="391cb-134">Type</span></span>|<span data-ttu-id="391cb-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="391cb-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="391cb-136">clientId</span><span class="sxs-lookup"><span data-stu-id="391cb-136">clientId</span></span>|<span data-ttu-id="391cb-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="391cb-137">String</span></span>|<span data-ttu-id="391cb-138">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="391cb-138">The client ID for the application.</span></span> <span data-ttu-id="391cb-139">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="391cb-139">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="391cb-140">clientSecret</span><span class="sxs-lookup"><span data-stu-id="391cb-140">clientSecret</span></span>|<span data-ttu-id="391cb-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="391cb-141">String</span></span>|<span data-ttu-id="391cb-142">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="391cb-142">The client secret for the application.</span></span> <span data-ttu-id="391cb-143">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="391cb-143">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="391cb-144">nome</span><span class="sxs-lookup"><span data-stu-id="391cb-144">name</span></span>|<span data-ttu-id="391cb-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="391cb-145">String</span></span>|<span data-ttu-id="391cb-146">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="391cb-146">The display name of the identity provider.</span></span>|
|<span data-ttu-id="391cb-147">tipo</span><span class="sxs-lookup"><span data-stu-id="391cb-147">type</span></span>|<span data-ttu-id="391cb-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="391cb-148">String</span></span>|<span data-ttu-id="391cb-149">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="391cb-149">The identity provider type.</span></span><ul><span data-ttu-id="391cb-150">Para cenário B2B:</span><span class="sxs-lookup"><span data-stu-id="391cb-150">For B2B scenario:</span></span><li/><span data-ttu-id="391cb-151">Google</span><span class="sxs-lookup"><span data-stu-id="391cb-151">Google</span></span><li/><span data-ttu-id="391cb-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="391cb-152">Facebook</span></span></ul><ul><span data-ttu-id="391cb-153">Para o cenário B2C:</span><span class="sxs-lookup"><span data-stu-id="391cb-153">For B2C scenario:</span></span><li/><span data-ttu-id="391cb-154">Microsoft</span><span class="sxs-lookup"><span data-stu-id="391cb-154">Microsoft</span></span><li/><span data-ttu-id="391cb-155">Google</span><span class="sxs-lookup"><span data-stu-id="391cb-155">Google</span></span><li/><span data-ttu-id="391cb-156">Amazon</span><span class="sxs-lookup"><span data-stu-id="391cb-156">Amazon</span></span><li/><span data-ttu-id="391cb-157">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="391cb-157">LinkedIn</span></span><li/><span data-ttu-id="391cb-158">Facebook</span><span class="sxs-lookup"><span data-stu-id="391cb-158">Facebook</span></span><li/><span data-ttu-id="391cb-159">GitHub</span><span class="sxs-lookup"><span data-stu-id="391cb-159">GitHub</span></span><li/><span data-ttu-id="391cb-160">Twitter</span><span class="sxs-lookup"><span data-stu-id="391cb-160">Twitter</span></span><li/><span data-ttu-id="391cb-161">Weibo</span><span class="sxs-lookup"><span data-stu-id="391cb-161">Weibo</span></span><li/><span data-ttu-id="391cb-162">QQ</span><span class="sxs-lookup"><span data-stu-id="391cb-162">QQ</span></span><li/><span data-ttu-id="391cb-163">WeChat</span><span class="sxs-lookup"><span data-stu-id="391cb-163">WeChat</span></span><li/><span data-ttu-id="391cb-164">OpenIDConnect</span><span class="sxs-lookup"><span data-stu-id="391cb-164">OpenIDConnect</span></span></ul>|

### <a name="openidconnectprovider-object"></a><span data-ttu-id="391cb-165">objeto openIdConnectProvider</span><span class="sxs-lookup"><span data-stu-id="391cb-165">openIdConnectProvider object</span></span>

|<span data-ttu-id="391cb-166">Propriedade</span><span class="sxs-lookup"><span data-stu-id="391cb-166">Property</span></span>|<span data-ttu-id="391cb-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="391cb-167">Type</span></span>|<span data-ttu-id="391cb-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="391cb-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="391cb-169">clientId</span><span class="sxs-lookup"><span data-stu-id="391cb-169">clientId</span></span>|<span data-ttu-id="391cb-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="391cb-170">String</span></span>|<span data-ttu-id="391cb-171">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="391cb-171">The client ID for the application.</span></span> <span data-ttu-id="391cb-172">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="391cb-172">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="391cb-173">clientSecret</span><span class="sxs-lookup"><span data-stu-id="391cb-173">clientSecret</span></span>|<span data-ttu-id="391cb-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="391cb-174">String</span></span>|<span data-ttu-id="391cb-175">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="391cb-175">The client secret for the application.</span></span> <span data-ttu-id="391cb-176">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="391cb-176">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="391cb-177">nome</span><span class="sxs-lookup"><span data-stu-id="391cb-177">name</span></span>|<span data-ttu-id="391cb-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="391cb-178">String</span></span>|<span data-ttu-id="391cb-179">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="391cb-179">The display name of the identity provider.</span></span>|
|<span data-ttu-id="391cb-180">tipo</span><span class="sxs-lookup"><span data-stu-id="391cb-180">type</span></span>|<span data-ttu-id="391cb-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="391cb-181">String</span></span>|<span data-ttu-id="391cb-182">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="391cb-182">The identity provider type.</span></span> <span data-ttu-id="391cb-183">O valor deve ser `OpenIdConnect` .</span><span class="sxs-lookup"><span data-stu-id="391cb-183">The value must be `OpenIdConnect`.</span></span>|
|<span data-ttu-id="391cb-184">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="391cb-184">claimsMapping</span></span>|[<span data-ttu-id="391cb-185">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="391cb-185">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="391cb-186">Depois que o provedor OIDC envia um token de ID de volta para o Azure AD, o Azure AD precisa ser capaz de mapear as declarações do token recebido para as declarações que o Azure AD reconhece e usa.</span><span class="sxs-lookup"><span data-stu-id="391cb-186">After the OIDC provider sends an ID token back to Azure AD, Azure AD needs to be able to map the claims from the received token to the claims that Azure AD recognizes and uses.</span></span> <span data-ttu-id="391cb-187">Esse tipo complexo captura esse mapeamento.</span><span class="sxs-lookup"><span data-stu-id="391cb-187">This complex type captures that mapping.</span></span>|
|<span data-ttu-id="391cb-188">domainHint</span><span class="sxs-lookup"><span data-stu-id="391cb-188">domainHint</span></span>|<span data-ttu-id="391cb-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="391cb-189">String</span></span>|<span data-ttu-id="391cb-190">A dica de domínio pode ser usada para saltar diretamente para a página de entrada do provedor de identidade especificado, em vez de fazer com que o usuário faça uma seleção entre a lista de provedores de identidade disponíveis.</span><span class="sxs-lookup"><span data-stu-id="391cb-190">The domain hint can be used to skip directly to the sign in page of the specified identity provider, instead of having the user make a selection among the list of available identity providers.</span></span>|
|<span data-ttu-id="391cb-191">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="391cb-191">metadataUrl</span></span>|<span data-ttu-id="391cb-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="391cb-192">String</span></span>|<span data-ttu-id="391cb-193">A URL para o documento de metadados do provedor de identidade de conexão de Open ID.</span><span class="sxs-lookup"><span data-stu-id="391cb-193">The URL for the metadata document of the Open Id Connect identity provider.</span></span>|
|<span data-ttu-id="391cb-194">responsemode</span><span class="sxs-lookup"><span data-stu-id="391cb-194">responseMode</span></span>|<span data-ttu-id="391cb-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="391cb-195">String</span></span>|<span data-ttu-id="391cb-196">Define o método que deve ser usado para enviar os dados de volta do provedor de identidade personalizado para o Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="391cb-196">Defines the method that should be used to send the data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="391cb-197">Os seguintes modos de resposta podem ser usados:</span><span class="sxs-lookup"><span data-stu-id="391cb-197">The following response modes can be used:</span></span> <ul><li/><span data-ttu-id="391cb-198">`form_post`: Este modo de resposta é recomendado para melhor segurança.</span><span class="sxs-lookup"><span data-stu-id="391cb-198">`form_post` : This response mode is recommended for best security.</span></span> <span data-ttu-id="391cb-199">A resposta é transmitida por meio do método HTTP POST, com o código ou token codificado no corpo usando o formato application/x-www-form-urlencoded.</span><span class="sxs-lookup"><span data-stu-id="391cb-199">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span><li/><span data-ttu-id="391cb-200">`query`: O código ou token é retornado como um parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="391cb-200">`query` : The code or token is returned as a query parameter.</span></span></ul>|
|<span data-ttu-id="391cb-201">responseType</span><span class="sxs-lookup"><span data-stu-id="391cb-201">responseType</span></span>|<span data-ttu-id="391cb-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="391cb-202">String</span></span>|<span data-ttu-id="391cb-203">Descreve que tipo de informação é enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="391cb-203">Describes what kind of information is sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="391cb-204">Os seguintes tipos de resposta podem ser usados:</span><span class="sxs-lookup"><span data-stu-id="391cb-204">The following response types can be used:</span></span><ul><li/> <span data-ttu-id="391cb-205">`code`: Conforme o fluxo do código de autorização, um código será retornado de volta para o Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="391cb-205">`code` : As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="391cb-206">O Azure AD B2C continua a chamar o token_endpoint para trocar o código do token.</span><span class="sxs-lookup"><span data-stu-id="391cb-206">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span><li/> <span data-ttu-id="391cb-207">`id_token`: Um token de ID retorna de volta para o Azure AD B2C do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="391cb-207">`id_token` : An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span> <li/><span data-ttu-id="391cb-208">`token`: Um token de acesso retorna de volta para o Azure AD B2C do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="391cb-208">`token` : An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="391cb-209">(Esse valor não é suportado pelo Azure AD B2C no momento)</span><span class="sxs-lookup"><span data-stu-id="391cb-209">(This value is not supported by Azure AD B2C at the moment)</span></span></ul>|
|<span data-ttu-id="391cb-210">escopo</span><span class="sxs-lookup"><span data-stu-id="391cb-210">scope</span></span>|<span data-ttu-id="391cb-211">String</span><span class="sxs-lookup"><span data-stu-id="391cb-211">String</span></span>|<span data-ttu-id="391cb-212">Escopo define as informações e permissões que você pretende coletar de seu provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="391cb-212">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="391cb-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="391cb-213">Response</span></span>

<span data-ttu-id="391cb-214">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="391cb-214">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="391cb-215">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="391cb-215">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="391cb-216">Exemplos</span><span class="sxs-lookup"><span data-stu-id="391cb-216">Examples</span></span>

### <a name="example-1-update-a-specific-identityprovider"></a><span data-ttu-id="391cb-217">Exemplo 1: atualizar um **identityprovider** específico</span><span class="sxs-lookup"><span data-stu-id="391cb-217">Example 1: Update a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="391cb-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="391cb-218">Request</span></span>

<span data-ttu-id="391cb-219">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="391cb-219">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="391cb-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="391cb-220">Response</span></span>

<span data-ttu-id="391cb-221">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="391cb-221">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-update-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="391cb-222">Exemplo 2: atualizar um **openIDConnectProvider** específico (somente para o Azure ad B2C)</span><span class="sxs-lookup"><span data-stu-id="391cb-222">Example 2: Update a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="391cb-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="391cb-223">Request</span></span>

<span data-ttu-id="391cb-224">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="391cb-224">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="391cb-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="391cb-225">Response</span></span>

<span data-ttu-id="391cb-226">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="391cb-226">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
