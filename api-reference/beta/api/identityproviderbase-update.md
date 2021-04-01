---
title: Atualizar identityProvider
description: Atualizar propriedades de um identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 985a6d4c80187decd5770eca150f501786222a1c
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491048"
---
# <a name="update-identityprovider"></a><span data-ttu-id="fe397-103">Atualizar identityProvider</span><span class="sxs-lookup"><span data-stu-id="fe397-103">Update identityProvider</span></span>
<span data-ttu-id="fe397-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe397-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe397-105">Atualize as propriedades de um [objeto socialIdentityProvider](../resources/socialidentityprovider.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fe397-105">Update the properties of a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="fe397-106">Para o Azure AD B2C, atualize as propriedades de [um objeto socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou [appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="fe397-106">For Azure AD B2C, update the properties  of a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe397-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe397-107">Permissions</span></span>

<span data-ttu-id="fe397-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe397-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe397-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe397-110">Permission type</span></span>      | <span data-ttu-id="fe397-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe397-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe397-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe397-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe397-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe397-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="fe397-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe397-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fe397-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe397-115">Not supported.</span></span>|
|<span data-ttu-id="fe397-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe397-116">Application</span></span>| <span data-ttu-id="fe397-117">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe397-117">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="fe397-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="fe397-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="fe397-119">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="fe397-119">Global Administrator</span></span>
* <span data-ttu-id="fe397-120">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="fe397-120">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="fe397-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe397-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fe397-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe397-122">Request headers</span></span>

|<span data-ttu-id="fe397-123">Nome</span><span class="sxs-lookup"><span data-stu-id="fe397-123">Name</span></span>|<span data-ttu-id="fe397-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe397-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fe397-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe397-125">Authorization</span></span>|<span data-ttu-id="fe397-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe397-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fe397-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe397-128">Content-Type</span></span>|<span data-ttu-id="fe397-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe397-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe397-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe397-131">Request body</span></span>

<span data-ttu-id="fe397-132">No corpo da solicitação, forneça um objeto JSON com uma ou mais propriedades que precisam ser atualizadas para um [objeto socialIdentityProvider](../resources/socialidentityprovider.md) no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fe397-132">In the request body, provide a JSON object with one or more properties that need to be updated for a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD tenant.</span></span>

<span data-ttu-id="fe397-133">No Azure AD B2C, forneça um objeto JSON com uma ou mais propriedades que precisam ser atualizadas para [um objeto socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou [um objeto appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="fe397-133">In Azure AD B2C, provide a JSON object with one or more properties that need to be updated for a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

### <a name="socialidentityprovider-object"></a><span data-ttu-id="fe397-134">Objeto socialIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="fe397-134">socialIdentityProvider object</span></span>

|<span data-ttu-id="fe397-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe397-135">Property</span></span>|<span data-ttu-id="fe397-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe397-136">Type</span></span>|<span data-ttu-id="fe397-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe397-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe397-138">clientId</span><span class="sxs-lookup"><span data-stu-id="fe397-138">clientId</span></span>|<span data-ttu-id="fe397-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-139">String</span></span>|<span data-ttu-id="fe397-140">O identificador de cliente do aplicativo obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fe397-140">The client identifier for the application obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="fe397-141">clientSecret</span><span class="sxs-lookup"><span data-stu-id="fe397-141">clientSecret</span></span>|<span data-ttu-id="fe397-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-142">String</span></span>|<span data-ttu-id="fe397-143">O segredo do cliente para o aplicativo que é obtido quando o aplicativo é registrado com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fe397-143">The client secret for the application that is obtained when the application is registered with the identity provider.</span></span> <span data-ttu-id="fe397-144">Isso é somente para gravar.</span><span class="sxs-lookup"><span data-stu-id="fe397-144">This is write-only.</span></span> <span data-ttu-id="fe397-145">Uma operação de leitura retorna " \* \* \* \* ".</span><span class="sxs-lookup"><span data-stu-id="fe397-145">A read operation returns "\*\*\*\*".</span></span>|
|<span data-ttu-id="fe397-146">displayName</span><span class="sxs-lookup"><span data-stu-id="fe397-146">displayName</span></span>|<span data-ttu-id="fe397-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-147">String</span></span>|<span data-ttu-id="fe397-148">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fe397-148">The display name of the identity provider.</span></span>|

### <a name="openidconnectidentityprovider-object"></a><span data-ttu-id="fe397-149">Objeto openIdConnectIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="fe397-149">openIdConnectIdentityProvider object</span></span>

|<span data-ttu-id="fe397-150">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe397-150">Property</span></span>|<span data-ttu-id="fe397-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe397-151">Type</span></span>|<span data-ttu-id="fe397-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe397-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe397-153">clientId</span><span class="sxs-lookup"><span data-stu-id="fe397-153">clientId</span></span>|<span data-ttu-id="fe397-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-154">String</span></span>|<span data-ttu-id="fe397-155">O identificador de cliente do aplicativo obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fe397-155">The client identifier for the application obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="fe397-156">clientSecret</span><span class="sxs-lookup"><span data-stu-id="fe397-156">clientSecret</span></span>|<span data-ttu-id="fe397-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-157">String</span></span>|<span data-ttu-id="fe397-158">O segredo do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fe397-158">The client secret for the application obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="fe397-159">O clientSecret tem uma dependência de **responseType**.</span><span class="sxs-lookup"><span data-stu-id="fe397-159">The clientSecret has a dependency on **responseType**.</span></span> <ul><li><span data-ttu-id="fe397-160">Quando **responseType** é `code` , um segredo é necessário para a troca de código de auth.</span><span class="sxs-lookup"><span data-stu-id="fe397-160">When **responseType** is `code`, a secret is required for the auth code exchange.</span></span></li><li><span data-ttu-id="fe397-161">Quando **responseType** é `id_token` o segredo não é necessário porque não há troca de código.</span><span class="sxs-lookup"><span data-stu-id="fe397-161">When **responseType** is `id_token` the secret is not required because there is no code exchange.</span></span> <span data-ttu-id="fe397-162">O id_token é retornado diretamente da resposta de autorização.</span><span class="sxs-lookup"><span data-stu-id="fe397-162">The id_token is returned directly from the authorization response.</span></span></li></ul>|
|<span data-ttu-id="fe397-163">displayName</span><span class="sxs-lookup"><span data-stu-id="fe397-163">displayName</span></span>|<span data-ttu-id="fe397-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-164">String</span></span>|<span data-ttu-id="fe397-165">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fe397-165">The display name of the identity provider.</span></span>|
|<span data-ttu-id="fe397-166">domainHint</span><span class="sxs-lookup"><span data-stu-id="fe397-166">domainHint</span></span>|<span data-ttu-id="fe397-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-167">String</span></span>|<span data-ttu-id="fe397-168">A dica de domínio pode ser usada para pular diretamente para a página de entrada do provedor de identidade especificado, em vez de fazer com que o usuário faça uma seleção entre a lista de provedores de identidade disponíveis.</span><span class="sxs-lookup"><span data-stu-id="fe397-168">The domain hint can be used to skip directly to the sign in page of the specified identity provider, instead of having the user make a selection among the list of available identity providers.</span></span>|
|<span data-ttu-id="fe397-169">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="fe397-169">claimsMapping</span></span>|[<span data-ttu-id="fe397-170">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="fe397-170">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="fe397-171">Depois que o provedor OIDC envia um token de ID de volta para o Azure AD, o Azure AD precisa ser capaz de mapear as declarações do token recebido para as declarações que o Azure AD reconhece e usa.</span><span class="sxs-lookup"><span data-stu-id="fe397-171">After the OIDC provider sends an ID token back to Azure AD, Azure AD needs to be able to map the claims from the received token to the claims that Azure AD recognizes and uses.</span></span> <span data-ttu-id="fe397-172">Esse tipo complexo captura esse mapeamento.</span><span class="sxs-lookup"><span data-stu-id="fe397-172">This complex type captures that mapping.</span></span>|
|<span data-ttu-id="fe397-173">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="fe397-173">metadataUrl</span></span>|<span data-ttu-id="fe397-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-174">String</span></span>|<span data-ttu-id="fe397-175">A URL do documento de metadados do provedor de identidade do OpenID Connect.</span><span class="sxs-lookup"><span data-stu-id="fe397-175">The URL for the metadata document of the OpenID Connect identity provider.</span></span> <span data-ttu-id="fe397-176">Cada provedor de identidade do OpenID Connect descreve um documento de metadados que contém a maioria das informações necessárias para executar a conexão.</span><span class="sxs-lookup"><span data-stu-id="fe397-176">Every OpenID Connect identity provider describes a metadata document that contains most of the information required to perform sign-in.</span></span> <span data-ttu-id="fe397-177">Isso inclui informações como as URLs a ser usadas e o local das chaves de assinatura públicas do serviço.</span><span class="sxs-lookup"><span data-stu-id="fe397-177">This includes information such as the URLs to use and the location of the service's public signing keys.</span></span> <span data-ttu-id="fe397-178">O documento de metadados do OpenID Connect está sempre localizado em um ponto de extremidade que termina em `.well-known/openid-configuration` .</span><span class="sxs-lookup"><span data-stu-id="fe397-178">The OpenID Connect metadata document is always located at an endpoint that ends in `.well-known/openid-configuration`.</span></span> <span data-ttu-id="fe397-179">Forneça a URL de metadados para o provedor de identidade do OpenID Connect que você adicionar.</span><span class="sxs-lookup"><span data-stu-id="fe397-179">Provide the metadata URL for the OpenID Connect identity provider you add.</span></span>|
|<span data-ttu-id="fe397-180">responseMode</span><span class="sxs-lookup"><span data-stu-id="fe397-180">responseMode</span></span>|<span data-ttu-id="fe397-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-181">String</span></span>|<span data-ttu-id="fe397-182">O modo de resposta define o método usado para enviar dados de volta do provedor de identidade personalizado para o Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="fe397-182">The response mode defines the method used to send data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="fe397-183">Valores possíveis: `form_post` , `query` .</span><span class="sxs-lookup"><span data-stu-id="fe397-183">Possible values: `form_post`, `query`.</span></span>|
|<span data-ttu-id="fe397-184">responseType</span><span class="sxs-lookup"><span data-stu-id="fe397-184">responseType</span></span>|<span data-ttu-id="fe397-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-185">String</span></span>|<span data-ttu-id="fe397-186">O tipo de resposta descreve o tipo de informação enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="fe397-186">The response type describes the type of information sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="fe397-187">Valores possíveis: `code` , `id_token` , `token` .</span><span class="sxs-lookup"><span data-stu-id="fe397-187">Possible values: `code` , `id_token` , `token`.</span></span>|
|<span data-ttu-id="fe397-188">escopo</span><span class="sxs-lookup"><span data-stu-id="fe397-188">scope</span></span>|<span data-ttu-id="fe397-189">String</span><span class="sxs-lookup"><span data-stu-id="fe397-189">String</span></span>|<span data-ttu-id="fe397-190">O escopo define as informações e permissões que você está procurando coletar do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="fe397-190">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

### <a name="applemanagedidentityprovider-object"></a><span data-ttu-id="fe397-191">Objeto appleManagedIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="fe397-191">appleManagedIdentityProvider object</span></span>

|<span data-ttu-id="fe397-192">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe397-192">Property</span></span>|<span data-ttu-id="fe397-193">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe397-193">Type</span></span>|<span data-ttu-id="fe397-194">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe397-194">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe397-195">displayName</span><span class="sxs-lookup"><span data-stu-id="fe397-195">displayName</span></span>|<span data-ttu-id="fe397-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-196">String</span></span>|<span data-ttu-id="fe397-197">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fe397-197">The display name of the identity provider.</span></span>|
|<span data-ttu-id="fe397-198">developerId</span><span class="sxs-lookup"><span data-stu-id="fe397-198">developerId</span></span>|<span data-ttu-id="fe397-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-199">String</span></span>|<span data-ttu-id="fe397-200">O identificador do Desenvolvedor apple.</span><span class="sxs-lookup"><span data-stu-id="fe397-200">The Apple Developer identifier.</span></span>|
|<span data-ttu-id="fe397-201">serviceId</span><span class="sxs-lookup"><span data-stu-id="fe397-201">serviceId</span></span>|<span data-ttu-id="fe397-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-202">String</span></span>|<span data-ttu-id="fe397-203">O identificador do Desenvolvedor apple.</span><span class="sxs-lookup"><span data-stu-id="fe397-203">The Apple Developer identifier.</span></span>|
|<span data-ttu-id="fe397-204">keyId</span><span class="sxs-lookup"><span data-stu-id="fe397-204">keyId</span></span>|<span data-ttu-id="fe397-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-205">String</span></span>|<span data-ttu-id="fe397-206">O identificador apple key.</span><span class="sxs-lookup"><span data-stu-id="fe397-206">The Apple Key identifier.</span></span>|
|<span data-ttu-id="fe397-207">certificateData</span><span class="sxs-lookup"><span data-stu-id="fe397-207">certificateData</span></span>|<span data-ttu-id="fe397-208">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe397-208">String</span></span>|<span data-ttu-id="fe397-209">Os dados do certificado, que é uma longa cadeia de caracteres de texto do certificado, podem ser nulos.</span><span class="sxs-lookup"><span data-stu-id="fe397-209">The certificate data which is a long string of text from the certificate, can be null.</span></span>|

## <a name="response"></a><span data-ttu-id="fe397-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe397-210">Response</span></span>

<span data-ttu-id="fe397-211">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fe397-211">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="fe397-212">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="fe397-212">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="fe397-213">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fe397-213">Examples</span></span>

### <a name="example-1-update-a-specific-social-identity-provider-azure-ad-or-azure-ad-b2c"></a><span data-ttu-id="fe397-214">Exemplo 1: Atualizar um provedor de **identidade social específico** (Azure AD ou Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="fe397-214">Example 1: Update a specific **social identity provider** (Azure AD or Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="fe397-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe397-215">Request</span></span>

<span data-ttu-id="fe397-216">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe397-216">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_socialidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/Amazon-OAUTH
Content-type: application/json
Content-length: 41

{
  "clientSecret": "1111111111111"
}
```

---

#### <a name="response"></a><span data-ttu-id="fe397-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe397-217">Response</span></span>

<span data-ttu-id="fe397-218">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fe397-218">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="fe397-219">Exemplo 2: atualizar um provedor de identidade **do OpenID Connect** específico (somente para o Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="fe397-219">Example 2: Update a specific **OpenID Connect identity provider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="fe397-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe397-220">Request</span></span>

<span data-ttu-id="fe397-221">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe397-221">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_openidconnectprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/OIDC-V1-Nam_AD_Test-3e393390-ed2d-4794-97f6-5c999ccc61f7
Content-type: application/json
Content-length: 41

{
  "responseType": "id_token"
}
```

---

#### <a name="response"></a><span data-ttu-id="fe397-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe397-222">Response</span></span>

<span data-ttu-id="fe397-223">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fe397-223">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-a-specific-apple-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="fe397-224">Exemplo 3: atualizar um provedor de **identidade específico da Apple** (somente para o Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="fe397-224">Example 3: Update a specific **Apple identity provider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="fe397-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe397-225">Request</span></span>

<span data-ttu-id="fe397-226">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe397-226">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_appleidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/Apple-Managed-OIDC
Content-type: application/json
Content-length: 41

{
  "displayName": "Apple"
}
```

---

#### <a name="response"></a><span data-ttu-id="fe397-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe397-227">Response</span></span>

<span data-ttu-id="fe397-228">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fe397-228">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
