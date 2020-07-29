---
title: Criar identityProvider
description: Criar um novo objeto identityprovider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d5d6eb847179a062bda1c0013bafb73de38ab455
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509704"
---
# <a name="create-identityprovider"></a><span data-ttu-id="c1dbc-103">Criar identityProvider</span><span class="sxs-lookup"><span data-stu-id="c1dbc-103">Create identityProvider</span></span>

<span data-ttu-id="c1dbc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1dbc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1dbc-105">Criar um novo objeto [identityprovider](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="c1dbc-105">Create a new [identityProvider](../resources/identityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1dbc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c1dbc-106">Permissions</span></span>

<span data-ttu-id="c1dbc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1dbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1dbc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1dbc-109">Permission type</span></span>      | <span data-ttu-id="c1dbc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c1dbc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1dbc-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1dbc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c1dbc-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1dbc-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="c1dbc-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1dbc-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c1dbc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-114">Not supported.</span></span>|
|<span data-ttu-id="c1dbc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1dbc-115">Application</span></span>|<span data-ttu-id="c1dbc-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1dbc-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="c1dbc-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="c1dbc-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="c1dbc-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c1dbc-118">Global administrator</span></span>
* <span data-ttu-id="c1dbc-119">Administrador do provedor de identidade externa</span><span class="sxs-lookup"><span data-stu-id="c1dbc-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c1dbc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1dbc-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="c1dbc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1dbc-121">Request headers</span></span>

|<span data-ttu-id="c1dbc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c1dbc-122">Name</span></span>|<span data-ttu-id="c1dbc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1dbc-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c1dbc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1dbc-124">Authorization</span></span>|<span data-ttu-id="c1dbc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c1dbc-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1dbc-127">Content-Type</span></span>|<span data-ttu-id="c1dbc-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1dbc-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1dbc-130">Request body</span></span>

<span data-ttu-id="c1dbc-131">No corpo da solicitação, forneça uma representação JSON do objeto [identityprovider](../resources/identityprovider.md) ou [openIdConnectProvider](../resources/openidconnectprovider.md) (somente para o Azure ad B2C).</span><span class="sxs-lookup"><span data-stu-id="c1dbc-131">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object.</span></span> <span data-ttu-id="c1dbc-132">Todas as propriedades listadas na tabela a seguir são necessárias.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-132">All the properties listed in the following table are required.</span></span>

### <a name="identityprovider-object"></a><span data-ttu-id="c1dbc-133">objeto identityprovider</span><span class="sxs-lookup"><span data-stu-id="c1dbc-133">identityProvider object</span></span>

|<span data-ttu-id="c1dbc-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1dbc-134">Property</span></span>|<span data-ttu-id="c1dbc-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1dbc-135">Type</span></span>|<span data-ttu-id="c1dbc-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1dbc-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1dbc-137">clientId</span><span class="sxs-lookup"><span data-stu-id="c1dbc-137">clientId</span></span>|<span data-ttu-id="c1dbc-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1dbc-138">String</span></span>|<span data-ttu-id="c1dbc-139">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-139">The client ID for the application.</span></span> <span data-ttu-id="c1dbc-140">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-140">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="c1dbc-141">clientSecret</span><span class="sxs-lookup"><span data-stu-id="c1dbc-141">clientSecret</span></span>|<span data-ttu-id="c1dbc-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1dbc-142">String</span></span>|<span data-ttu-id="c1dbc-143">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-143">The client secret for the application.</span></span> <span data-ttu-id="c1dbc-144">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-144">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="c1dbc-145">nome</span><span class="sxs-lookup"><span data-stu-id="c1dbc-145">name</span></span>|<span data-ttu-id="c1dbc-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1dbc-146">String</span></span>|<span data-ttu-id="c1dbc-147">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-147">The display name of the identity provider.</span></span>|
|<span data-ttu-id="c1dbc-148">tipo</span><span class="sxs-lookup"><span data-stu-id="c1dbc-148">type</span></span>|<span data-ttu-id="c1dbc-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1dbc-149">String</span></span>|<span data-ttu-id="c1dbc-150">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-150">The identity provider type.</span></span> <ul><span data-ttu-id="c1dbc-151">Para cenário B2B:</span><span class="sxs-lookup"><span data-stu-id="c1dbc-151">For B2B scenario:</span></span><li/><span data-ttu-id="c1dbc-152">Google</span><span class="sxs-lookup"><span data-stu-id="c1dbc-152">Google</span></span><li/><span data-ttu-id="c1dbc-153">Facebook</span><span class="sxs-lookup"><span data-stu-id="c1dbc-153">Facebook</span></span></ul><ul><span data-ttu-id="c1dbc-154">Para o cenário B2C:</span><span class="sxs-lookup"><span data-stu-id="c1dbc-154">For B2C scenario:</span></span><li/><span data-ttu-id="c1dbc-155">Microsoft</span><span class="sxs-lookup"><span data-stu-id="c1dbc-155">Microsoft</span></span><li/><span data-ttu-id="c1dbc-156">Google</span><span class="sxs-lookup"><span data-stu-id="c1dbc-156">Google</span></span><li/><span data-ttu-id="c1dbc-157">Amazon</span><span class="sxs-lookup"><span data-stu-id="c1dbc-157">Amazon</span></span><li/><span data-ttu-id="c1dbc-158">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="c1dbc-158">LinkedIn</span></span><li/><span data-ttu-id="c1dbc-159">Facebook</span><span class="sxs-lookup"><span data-stu-id="c1dbc-159">Facebook</span></span><li/><span data-ttu-id="c1dbc-160">GitHub</span><span class="sxs-lookup"><span data-stu-id="c1dbc-160">GitHub</span></span><li/><span data-ttu-id="c1dbc-161">Twitter</span><span class="sxs-lookup"><span data-stu-id="c1dbc-161">Twitter</span></span><li/><span data-ttu-id="c1dbc-162">Weibo</span><span class="sxs-lookup"><span data-stu-id="c1dbc-162">Weibo</span></span><li/><span data-ttu-id="c1dbc-163">QQ</span><span class="sxs-lookup"><span data-stu-id="c1dbc-163">QQ</span></span><li/><span data-ttu-id="c1dbc-164">WeChat</span><span class="sxs-lookup"><span data-stu-id="c1dbc-164">WeChat</span></span><li/><span data-ttu-id="c1dbc-165">OpenIDConnect</span><span class="sxs-lookup"><span data-stu-id="c1dbc-165">OpenIDConnect</span></span></ul>|

### <a name="openidconnectprovider-object"></a><span data-ttu-id="c1dbc-166">objeto openIdConnectProvider</span><span class="sxs-lookup"><span data-stu-id="c1dbc-166">openIdConnectProvider object</span></span>

|<span data-ttu-id="c1dbc-167">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1dbc-167">Property</span></span>|<span data-ttu-id="c1dbc-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1dbc-168">Type</span></span>|<span data-ttu-id="c1dbc-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1dbc-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1dbc-170">clientId</span><span class="sxs-lookup"><span data-stu-id="c1dbc-170">clientId</span></span>|<span data-ttu-id="c1dbc-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1dbc-171">String</span></span>|<span data-ttu-id="c1dbc-172">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-172">The client ID for the application.</span></span> <span data-ttu-id="c1dbc-173">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-173">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="c1dbc-174">clientSecret</span><span class="sxs-lookup"><span data-stu-id="c1dbc-174">clientSecret</span></span>|<span data-ttu-id="c1dbc-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1dbc-175">String</span></span>|<span data-ttu-id="c1dbc-176">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-176">The client secret for the application.</span></span> <span data-ttu-id="c1dbc-177">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-177">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="c1dbc-178">nome</span><span class="sxs-lookup"><span data-stu-id="c1dbc-178">name</span></span>|<span data-ttu-id="c1dbc-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1dbc-179">String</span></span>|<span data-ttu-id="c1dbc-180">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-180">The display name of the identity provider.</span></span>|
|<span data-ttu-id="c1dbc-181">tipo</span><span class="sxs-lookup"><span data-stu-id="c1dbc-181">type</span></span>|<span data-ttu-id="c1dbc-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1dbc-182">String</span></span>|<span data-ttu-id="c1dbc-183">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-183">The identity provider type.</span></span> <span data-ttu-id="c1dbc-184">O valor deve ser `OpenIdConnect` .</span><span class="sxs-lookup"><span data-stu-id="c1dbc-184">The value must be `OpenIdConnect`.</span></span>|
|<span data-ttu-id="c1dbc-185">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="c1dbc-185">claimsMapping</span></span>|[<span data-ttu-id="c1dbc-186">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="c1dbc-186">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="c1dbc-187">As `userId` `displayname` Propriedades e são necessárias no objeto claimsMapping.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-187">The `userId` and `displayname` properties are required in the claimsMapping object.</span></span>|
|<span data-ttu-id="c1dbc-188">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="c1dbc-188">metadataUrl</span></span>|<span data-ttu-id="c1dbc-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1dbc-189">String</span></span>|<span data-ttu-id="c1dbc-190">A URL para o documento de metadados do provedor de identidade de conexão de Open ID.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-190">The URL for the metadata document of the Open Id Connect identity provider.</span></span>|
|<span data-ttu-id="c1dbc-191">responsemode</span><span class="sxs-lookup"><span data-stu-id="c1dbc-191">responseMode</span></span>|<span data-ttu-id="c1dbc-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1dbc-192">String</span></span>|<span data-ttu-id="c1dbc-193">Define o método que deve ser usado para enviar os dados de volta do provedor de identidade personalizado para o Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-193">Defines the method that should be used to send the data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="c1dbc-194">Os seguintes modos de resposta podem ser usados:</span><span class="sxs-lookup"><span data-stu-id="c1dbc-194">The following response modes can be used:</span></span> <ul><li/><span data-ttu-id="c1dbc-195">`form_post`: Este modo de resposta é recomendado para melhor segurança.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-195">`form_post` : This response mode is recommended for best security.</span></span> <span data-ttu-id="c1dbc-196">A resposta é transmitida por meio do método HTTP POST, com o código ou token codificado no corpo usando o formato application/x-www-form-urlencoded.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-196">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span><li/><span data-ttu-id="c1dbc-197">`query`: O código ou token é retornado como um parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-197">`query` : The code or token is returned as a query parameter.</span></span></ul>|
|<span data-ttu-id="c1dbc-198">responseType</span><span class="sxs-lookup"><span data-stu-id="c1dbc-198">responseType</span></span>|<span data-ttu-id="c1dbc-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1dbc-199">String</span></span>|<span data-ttu-id="c1dbc-200">Descreve que tipo de informação é enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-200">Describes what kind of information is sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="c1dbc-201">Os seguintes tipos de resposta podem ser usados:</span><span class="sxs-lookup"><span data-stu-id="c1dbc-201">The following response types can be used:</span></span><ul><li/> <span data-ttu-id="c1dbc-202">`code`: Conforme o fluxo do código de autorização, um código será retornado de volta para o Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-202">`code` : As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="c1dbc-203">O Azure AD B2C continua a chamar o token_endpoint para trocar o código do token.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-203">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span><li/> <span data-ttu-id="c1dbc-204">`id_token`: Um token de ID retorna de volta para o Azure AD B2C do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-204">`id_token` : An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span> <li/><span data-ttu-id="c1dbc-205">`token`: Um token de acesso retorna de volta para o Azure AD B2C do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-205">`token` : An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="c1dbc-206">(Esse valor não é suportado pelo Azure AD B2C no momento)</span><span class="sxs-lookup"><span data-stu-id="c1dbc-206">(This value is not supported by Azure AD B2C at the moment)</span></span></ul>|
|<span data-ttu-id="c1dbc-207">escopo</span><span class="sxs-lookup"><span data-stu-id="c1dbc-207">scope</span></span>|<span data-ttu-id="c1dbc-208">String</span><span class="sxs-lookup"><span data-stu-id="c1dbc-208">String</span></span>|<span data-ttu-id="c1dbc-209">Escopo define as informações e permissões que você pretende coletar de seu provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-209">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="c1dbc-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1dbc-210">Response</span></span>

<span data-ttu-id="c1dbc-211">Se tiver êxito, este método retornará um `201 Created` código de resposta e [identityprovider](../resources/identityprovider.md) ou [openIdConnectProvider](../resources/openidconnectprovider.md) (somente para o objeto do Azure ad B2C) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-211">If successful, this method returns a `201 Created` response code and [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object in the response body.</span></span> <span data-ttu-id="c1dbc-212">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-212">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="c1dbc-213">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c1dbc-213">Examples</span></span>

### <a name="example-1-create-a-specific-identityprovider"></a><span data-ttu-id="c1dbc-214">Exemplo 1: criar um **identityprovider** específico</span><span class="sxs-lookup"><span data-stu-id="c1dbc-214">Example 1: Create a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="c1dbc-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1dbc-215">Request</span></span>

<span data-ttu-id="c1dbc-216">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-216">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="c1dbc-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1dbc-217">Response</span></span>

<span data-ttu-id="c1dbc-218">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-218">The following is an example of the response.</span></span>

<span data-ttu-id="c1dbc-219">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-219">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
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
### <a name="example-2-create-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="c1dbc-220">Exemplo 2: criar um **openIDConnectProvider** específico (somente para o Azure ad B2C)</span><span class="sxs-lookup"><span data-stu-id="c1dbc-220">Example 2: Create a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="c1dbc-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1dbc-221">Request</span></span>

<span data-ttu-id="c1dbc-222">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-222">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="c1dbc-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1dbc-223">Response</span></span>

<span data-ttu-id="c1dbc-224">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-224">The following is an example of the response.</span></span>

<span data-ttu-id="c1dbc-225">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c1dbc-225">**Note:** The response object shown here might be shortened for readability.</span></span>

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
