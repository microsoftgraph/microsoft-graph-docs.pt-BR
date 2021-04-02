---
title: Criar identityProvider
description: Crie um novo objeto identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 5fe99410b965f6cabae171c713a7207fc2c7ea18
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508831"
---
# <a name="create-identityprovider-deprecated"></a><span data-ttu-id="dbd11-103">Criar identityProvider (preterido)</span><span class="sxs-lookup"><span data-stu-id="dbd11-103">Create identityProvider (deprecated)</span></span>

<span data-ttu-id="dbd11-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbd11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="dbd11-105">Crie um novo [objeto identityProvider.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="dbd11-105">Create a new [identityProvider](../resources/identityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbd11-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="dbd11-106">Permissions</span></span>

<span data-ttu-id="dbd11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbd11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbd11-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbd11-109">Permission type</span></span>      | <span data-ttu-id="dbd11-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbd11-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbd11-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbd11-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dbd11-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbd11-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="dbd11-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbd11-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="dbd11-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbd11-114">Not supported.</span></span>|
|<span data-ttu-id="dbd11-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbd11-115">Application</span></span>|<span data-ttu-id="dbd11-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbd11-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="dbd11-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="dbd11-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="dbd11-118">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="dbd11-118">Global Administrator</span></span>
* <span data-ttu-id="dbd11-119">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="dbd11-119">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="dbd11-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbd11-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="dbd11-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbd11-121">Request headers</span></span>

|<span data-ttu-id="dbd11-122">Nome</span><span class="sxs-lookup"><span data-stu-id="dbd11-122">Name</span></span>|<span data-ttu-id="dbd11-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbd11-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="dbd11-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbd11-124">Authorization</span></span>|<span data-ttu-id="dbd11-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbd11-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="dbd11-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dbd11-127">Content-Type</span></span>|<span data-ttu-id="dbd11-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbd11-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbd11-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbd11-130">Request body</span></span>

<span data-ttu-id="dbd11-131">No corpo da solicitação, forneça uma representação JSON do [objeto identityProvider](../resources/identityprovider.md) ou [openIdConnectProvider](../resources/openidconnectprovider.md) (somente para o Azure AD B2C).</span><span class="sxs-lookup"><span data-stu-id="dbd11-131">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object.</span></span> <span data-ttu-id="dbd11-132">Todas as propriedades listadas na tabela a seguir são necessárias.</span><span class="sxs-lookup"><span data-stu-id="dbd11-132">All the properties listed in the following table are required.</span></span>

### <a name="identityprovider-object"></a><span data-ttu-id="dbd11-133">objeto identityProvider</span><span class="sxs-lookup"><span data-stu-id="dbd11-133">identityProvider object</span></span>

|<span data-ttu-id="dbd11-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbd11-134">Property</span></span>|<span data-ttu-id="dbd11-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbd11-135">Type</span></span>|<span data-ttu-id="dbd11-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbd11-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbd11-137">clientId</span><span class="sxs-lookup"><span data-stu-id="dbd11-137">clientId</span></span>|<span data-ttu-id="dbd11-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbd11-138">String</span></span>|<span data-ttu-id="dbd11-139">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dbd11-139">The client ID for the application.</span></span> <span data-ttu-id="dbd11-140">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="dbd11-140">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="dbd11-141">clientSecret</span><span class="sxs-lookup"><span data-stu-id="dbd11-141">clientSecret</span></span>|<span data-ttu-id="dbd11-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbd11-142">String</span></span>|<span data-ttu-id="dbd11-143">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dbd11-143">The client secret for the application.</span></span> <span data-ttu-id="dbd11-144">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="dbd11-144">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="dbd11-145">nome</span><span class="sxs-lookup"><span data-stu-id="dbd11-145">name</span></span>|<span data-ttu-id="dbd11-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbd11-146">String</span></span>|<span data-ttu-id="dbd11-147">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="dbd11-147">The display name of the identity provider.</span></span>|
|<span data-ttu-id="dbd11-148">tipo</span><span class="sxs-lookup"><span data-stu-id="dbd11-148">type</span></span>|<span data-ttu-id="dbd11-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbd11-149">String</span></span>|<span data-ttu-id="dbd11-150">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="dbd11-150">The identity provider type.</span></span> <ul><span data-ttu-id="dbd11-151">Para o cenário B2B:</span><span class="sxs-lookup"><span data-stu-id="dbd11-151">For B2B scenario:</span></span><li/><span data-ttu-id="dbd11-152">Google</span><span class="sxs-lookup"><span data-stu-id="dbd11-152">Google</span></span><li/><span data-ttu-id="dbd11-153">Facebook</span><span class="sxs-lookup"><span data-stu-id="dbd11-153">Facebook</span></span></ul><ul><span data-ttu-id="dbd11-154">Para o cenário B2C:</span><span class="sxs-lookup"><span data-stu-id="dbd11-154">For B2C scenario:</span></span><li/><span data-ttu-id="dbd11-155">Microsoft</span><span class="sxs-lookup"><span data-stu-id="dbd11-155">Microsoft</span></span><li/><span data-ttu-id="dbd11-156">Google</span><span class="sxs-lookup"><span data-stu-id="dbd11-156">Google</span></span><li/><span data-ttu-id="dbd11-157">Amazon</span><span class="sxs-lookup"><span data-stu-id="dbd11-157">Amazon</span></span><li/><span data-ttu-id="dbd11-158">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="dbd11-158">LinkedIn</span></span><li/><span data-ttu-id="dbd11-159">Facebook</span><span class="sxs-lookup"><span data-stu-id="dbd11-159">Facebook</span></span><li/><span data-ttu-id="dbd11-160">GitHub</span><span class="sxs-lookup"><span data-stu-id="dbd11-160">GitHub</span></span><li/><span data-ttu-id="dbd11-161">Twitter</span><span class="sxs-lookup"><span data-stu-id="dbd11-161">Twitter</span></span><li/><span data-ttu-id="dbd11-162">Weibo</span><span class="sxs-lookup"><span data-stu-id="dbd11-162">Weibo</span></span><li/><span data-ttu-id="dbd11-163">QQ</span><span class="sxs-lookup"><span data-stu-id="dbd11-163">QQ</span></span><li/><span data-ttu-id="dbd11-164">WeChat</span><span class="sxs-lookup"><span data-stu-id="dbd11-164">WeChat</span></span><li/><span data-ttu-id="dbd11-165">OpenIDConnect</span><span class="sxs-lookup"><span data-stu-id="dbd11-165">OpenIDConnect</span></span></ul>|

### <a name="openidconnectprovider-object"></a><span data-ttu-id="dbd11-166">Objeto openIdConnectProvider</span><span class="sxs-lookup"><span data-stu-id="dbd11-166">openIdConnectProvider object</span></span>

|<span data-ttu-id="dbd11-167">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbd11-167">Property</span></span>|<span data-ttu-id="dbd11-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbd11-168">Type</span></span>|<span data-ttu-id="dbd11-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbd11-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbd11-170">clientId</span><span class="sxs-lookup"><span data-stu-id="dbd11-170">clientId</span></span>|<span data-ttu-id="dbd11-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbd11-171">String</span></span>|<span data-ttu-id="dbd11-172">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dbd11-172">The client ID for the application.</span></span> <span data-ttu-id="dbd11-173">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="dbd11-173">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="dbd11-174">clientSecret</span><span class="sxs-lookup"><span data-stu-id="dbd11-174">clientSecret</span></span>|<span data-ttu-id="dbd11-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbd11-175">String</span></span>|<span data-ttu-id="dbd11-176">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dbd11-176">The client secret for the application.</span></span> <span data-ttu-id="dbd11-177">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="dbd11-177">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="dbd11-178">nome</span><span class="sxs-lookup"><span data-stu-id="dbd11-178">name</span></span>|<span data-ttu-id="dbd11-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbd11-179">String</span></span>|<span data-ttu-id="dbd11-180">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="dbd11-180">The display name of the identity provider.</span></span>|
|<span data-ttu-id="dbd11-181">tipo</span><span class="sxs-lookup"><span data-stu-id="dbd11-181">type</span></span>|<span data-ttu-id="dbd11-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbd11-182">String</span></span>|<span data-ttu-id="dbd11-183">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="dbd11-183">The identity provider type.</span></span> <span data-ttu-id="dbd11-184">O valor deve ser `OpenIdConnect` .</span><span class="sxs-lookup"><span data-stu-id="dbd11-184">The value must be `OpenIdConnect`.</span></span>|
|<span data-ttu-id="dbd11-185">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="dbd11-185">claimsMapping</span></span>|[<span data-ttu-id="dbd11-186">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="dbd11-186">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="dbd11-187">As `userId` propriedades e são necessárias no objeto `displayname` claimsMapping.</span><span class="sxs-lookup"><span data-stu-id="dbd11-187">The `userId` and `displayname` properties are required in the claimsMapping object.</span></span>|
|<span data-ttu-id="dbd11-188">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="dbd11-188">metadataUrl</span></span>|<span data-ttu-id="dbd11-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbd11-189">String</span></span>|<span data-ttu-id="dbd11-190">A URL do documento de metadados do provedor de identidade do Open Id Connect.</span><span class="sxs-lookup"><span data-stu-id="dbd11-190">The URL for the metadata document of the Open Id Connect identity provider.</span></span>|
|<span data-ttu-id="dbd11-191">responseMode</span><span class="sxs-lookup"><span data-stu-id="dbd11-191">responseMode</span></span>|<span data-ttu-id="dbd11-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbd11-192">String</span></span>|<span data-ttu-id="dbd11-193">Define o método que deve ser usado para enviar os dados de volta do provedor de identidade personalizado para o Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="dbd11-193">Defines the method that should be used to send the data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="dbd11-194">Os seguintes modos de resposta podem ser usados:</span><span class="sxs-lookup"><span data-stu-id="dbd11-194">The following response modes can be used:</span></span> <ul><li/><span data-ttu-id="dbd11-195">`form_post` : Este modo de resposta é recomendado para melhor segurança.</span><span class="sxs-lookup"><span data-stu-id="dbd11-195">`form_post` : This response mode is recommended for best security.</span></span> <span data-ttu-id="dbd11-196">A resposta é transmitida por meio do método HTTP POST, com o código ou token sendo codificado no corpo usando o formato application/x-www-form-urlencoded.</span><span class="sxs-lookup"><span data-stu-id="dbd11-196">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span><li/><span data-ttu-id="dbd11-197">`query` : O código ou token é retornado como um parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="dbd11-197">`query` : The code or token is returned as a query parameter.</span></span></ul>|
|<span data-ttu-id="dbd11-198">responseType</span><span class="sxs-lookup"><span data-stu-id="dbd11-198">responseType</span></span>|<span data-ttu-id="dbd11-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbd11-199">String</span></span>|<span data-ttu-id="dbd11-200">Descreve que tipo de informação é enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="dbd11-200">Describes what kind of information is sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="dbd11-201">Os seguintes tipos de resposta podem ser usados:</span><span class="sxs-lookup"><span data-stu-id="dbd11-201">The following response types can be used:</span></span><ul><li/> <span data-ttu-id="dbd11-202">`code` : De acordo com o fluxo de código de autorização, um código será retornado para o Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="dbd11-202">`code` : As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="dbd11-203">O Azure AD B2C continua a chamar o token_endpoint para trocar o código pelo token.</span><span class="sxs-lookup"><span data-stu-id="dbd11-203">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span><li/> <span data-ttu-id="dbd11-204">`id_token` : Um token de ID é retornado ao Azure AD B2C do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="dbd11-204">`id_token` : An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span> <li/><span data-ttu-id="dbd11-205">`token` : Um token de acesso é retornado ao Azure AD B2C do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="dbd11-205">`token` : An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="dbd11-206">(Esse valor não é suportado pelo Azure AD B2C no momento)</span><span class="sxs-lookup"><span data-stu-id="dbd11-206">(This value is not supported by Azure AD B2C at the moment)</span></span></ul>|
|<span data-ttu-id="dbd11-207">escopo</span><span class="sxs-lookup"><span data-stu-id="dbd11-207">scope</span></span>|<span data-ttu-id="dbd11-208">String</span><span class="sxs-lookup"><span data-stu-id="dbd11-208">String</span></span>|<span data-ttu-id="dbd11-209">O escopo define as informações e permissões que você está procurando coletar do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="dbd11-209">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="dbd11-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbd11-210">Response</span></span>

<span data-ttu-id="dbd11-211">Se tiver êxito, este método retornará um código de resposta e `201 Created` [um objeto identityProvider](../resources/identityprovider.md) ou [openIdConnectProvider](../resources/openidconnectprovider.md) (somente para o Azure AD B2C) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbd11-211">If successful, this method returns a `201 Created` response code and [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object in the response body.</span></span> <span data-ttu-id="dbd11-212">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="dbd11-212">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="dbd11-213">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dbd11-213">Examples</span></span>

### <a name="example-1-create-a-specific-identityprovider"></a><span data-ttu-id="dbd11-214">Exemplo 1: Criar uma **identidade específicaProvider**</span><span class="sxs-lookup"><span data-stu-id="dbd11-214">Example 1: Create a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="dbd11-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbd11-215">Request</span></span>

<span data-ttu-id="dbd11-216">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbd11-216">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json
Content-length: 154

{
  "@odata.type": "microsoft.graph.identityProvider",
  "name": "Login with Amazon",
  "type": "Amazon",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "000000000000"
}
```

# <a name="java"></a>[<span data-ttu-id="dbd11-217">Java</span><span class="sxs-lookup"><span data-stu-id="dbd11-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityprovider-from-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="dbd11-218">C#</span><span class="sxs-lookup"><span data-stu-id="dbd11-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbd11-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbd11-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbd11-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbd11-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="dbd11-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbd11-221">Response</span></span>

<span data-ttu-id="dbd11-222">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dbd11-222">The following is an example of the response.</span></span>

<span data-ttu-id="dbd11-223">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dbd11-223">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "@odata.type": "microsoft.graph.identityProvider",
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

### <a name="example-2-create-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="dbd11-224">Exemplo 2: Criar um **openIDConnectProvider específico** (somente para o Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="dbd11-224">Example 2: Create a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="dbd11-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbd11-225">Request</span></span>

<span data-ttu-id="dbd11-226">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbd11-226">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_openidconnectprovider_from_identityproviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
    "name": "Login with the Contoso identity provider",
    "type": "OpenIDConnect",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "12345",
    "claimsMapping": {
        "userId": "myUserId",
        "givenName": "myGivenName",
        "surname": "mySurname",
        "email": "myEmail",
        "displayName": "myDisplayName"
    },
    "domainHint": "mycustomoidc",
    "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
    "responseMode": "form_post",
    "responseType": "code",
    "scope": "openid"
}

```

# <a name="java"></a>[<span data-ttu-id="dbd11-227">Java</span><span class="sxs-lookup"><span data-stu-id="dbd11-227">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-openidconnectprovider-from-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="dbd11-228">C#</span><span class="sxs-lookup"><span data-stu-id="dbd11-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-openidconnectprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbd11-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbd11-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-openidconnectprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbd11-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbd11-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-openidconnectprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="dbd11-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbd11-231">Response</span></span>

<span data-ttu-id="dbd11-232">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dbd11-232">The following is an example of the response.</span></span>

<span data-ttu-id="dbd11-233">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dbd11-233">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
  "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
  "name": "Login with the Contoso identity provider",
  "type": "OpenIDConnect",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "12345",
  "claimsMapping": {
      "userId": "myUserId",
      "givenName": "myGivenName",
      "surname": "mySurname",
      "email": "myEmail",
      "displayName": "myDisplayName"
  },
  "domainHint": "mycustomoidc",
  "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
  "responseMode": "form_post",
  "responseType": "code",
  "scope": "openid"
}
```
