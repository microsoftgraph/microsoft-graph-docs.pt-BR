---
title: Atualizar identityProvider
description: Atualizar propriedades de um identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 4056229ecb748ff9c99a3b332298d32e67fdaf66
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921211"
---
# <a name="update-identityprovider"></a><span data-ttu-id="a6e4e-103">Atualizar identityProvider</span><span class="sxs-lookup"><span data-stu-id="a6e4e-103">Update identityProvider</span></span>
<span data-ttu-id="a6e4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6e4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6e4e-105">Atualize as propriedades de um [objeto socialIdentityProvider](../resources/socialidentityprovider.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-105">Update the properties of a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="a6e4e-106">Para o Azure AD B2C, atualize as propriedades de [um objeto socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou [appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="a6e4e-106">For Azure AD B2C, update the properties  of a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6e4e-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="a6e4e-107">Permissions</span></span>

<span data-ttu-id="a6e4e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6e4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6e4e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6e4e-110">Permission type</span></span>      | <span data-ttu-id="a6e4e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6e4e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6e4e-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6e4e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6e4e-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6e4e-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="a6e4e-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6e4e-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a6e4e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-115">Not supported.</span></span>|
|<span data-ttu-id="a6e4e-116">Application</span><span class="sxs-lookup"><span data-stu-id="a6e4e-116">Application</span></span>| <span data-ttu-id="a6e4e-117">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6e4e-117">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="a6e4e-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="a6e4e-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="a6e4e-119">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="a6e4e-119">Global Administrator</span></span>
* <span data-ttu-id="a6e4e-120">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="a6e4e-120">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a6e4e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6e4e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a6e4e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6e4e-122">Request headers</span></span>

|<span data-ttu-id="a6e4e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="a6e4e-123">Name</span></span>|<span data-ttu-id="a6e4e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6e4e-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a6e4e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6e4e-125">Authorization</span></span>|<span data-ttu-id="a6e4e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a6e4e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6e4e-128">Content-Type</span></span>|<span data-ttu-id="a6e4e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6e4e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6e4e-131">Request body</span></span>

<span data-ttu-id="a6e4e-132">No corpo da solicitação, forneça um objeto JSON com uma ou mais propriedades que precisam ser atualizadas para um [objeto socialIdentityProvider](../resources/socialidentityprovider.md) no locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-132">In the request body, provide a JSON object with one or more properties that need to be updated for a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD tenant.</span></span>

<span data-ttu-id="a6e4e-133">No Azure AD B2C, forneça um objeto JSON com uma ou mais propriedades que precisam ser atualizadas para [um objeto socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou [um objeto appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="a6e4e-133">In Azure AD B2C, provide a JSON object with one or more properties that need to be updated for a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

### <a name="socialidentityprovider-object"></a><span data-ttu-id="a6e4e-134">Objeto socialIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="a6e4e-134">socialIdentityProvider object</span></span>

|<span data-ttu-id="a6e4e-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6e4e-135">Property</span></span>|<span data-ttu-id="a6e4e-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6e4e-136">Type</span></span>|<span data-ttu-id="a6e4e-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6e4e-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6e4e-138">clientId</span><span class="sxs-lookup"><span data-stu-id="a6e4e-138">clientId</span></span>|<span data-ttu-id="a6e4e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6e4e-139">String</span></span>|<span data-ttu-id="a6e4e-140">O identificador do cliente para o aplicativo obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-140">The client identifier for the application obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="a6e4e-141">clientSecret</span><span class="sxs-lookup"><span data-stu-id="a6e4e-141">clientSecret</span></span>|<span data-ttu-id="a6e4e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6e4e-142">String</span></span>|<span data-ttu-id="a6e4e-143">O segredo do cliente para o aplicativo obtido quando o aplicativo é registrado com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-143">The client secret for the application that is obtained when the application is registered with the identity provider.</span></span> <span data-ttu-id="a6e4e-144">Isso é somente gravação.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-144">This is write-only.</span></span> <span data-ttu-id="a6e4e-145">Uma operação de leitura retorna "\*\*\*\*".</span><span class="sxs-lookup"><span data-stu-id="a6e4e-145">A read operation returns "\*\*\*\*".</span></span>|
|<span data-ttu-id="a6e4e-146">displayName</span><span class="sxs-lookup"><span data-stu-id="a6e4e-146">displayName</span></span>|<span data-ttu-id="a6e4e-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6e4e-147">String</span></span>|<span data-ttu-id="a6e4e-148">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-148">The display name of the identity provider.</span></span>|

### <a name="openidconnectidentityprovider-object"></a><span data-ttu-id="a6e4e-149">Objeto openIdConnectIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="a6e4e-149">openIdConnectIdentityProvider object</span></span>

|<span data-ttu-id="a6e4e-150">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6e4e-150">Property</span></span>|<span data-ttu-id="a6e4e-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6e4e-151">Type</span></span>|<span data-ttu-id="a6e4e-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6e4e-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6e4e-153">clientId</span><span class="sxs-lookup"><span data-stu-id="a6e4e-153">clientId</span></span>|<span data-ttu-id="a6e4e-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6e4e-154">String</span></span>|<span data-ttu-id="a6e4e-155">O identificador do cliente para o aplicativo obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-155">The client identifier for the application obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="a6e4e-156">clientSecret</span><span class="sxs-lookup"><span data-stu-id="a6e4e-156">clientSecret</span></span>|<span data-ttu-id="a6e4e-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6e4e-157">String</span></span>|<span data-ttu-id="a6e4e-158">O segredo do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-158">The client secret for the application obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="a6e4e-159">O clientSecret tem uma dependência de **responseType**.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-159">The clientSecret has a dependency on **responseType**.</span></span> <ul><li><span data-ttu-id="a6e4e-160">Quando **responseType** é `code` , um segredo é necessário para a troca de código de auth.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-160">When **responseType** is `code`, a secret is required for the auth code exchange.</span></span></li><li><span data-ttu-id="a6e4e-161">Quando **responseType** é `id_token` o segredo não é necessário porque não há troca de código.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-161">When **responseType** is `id_token` the secret is not required because there is no code exchange.</span></span> <span data-ttu-id="a6e4e-162">O id_token é retornado diretamente da resposta de autorização.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-162">The id_token is returned directly from the authorization response.</span></span></li></ul>|
|<span data-ttu-id="a6e4e-163">displayName</span><span class="sxs-lookup"><span data-stu-id="a6e4e-163">displayName</span></span>|<span data-ttu-id="a6e4e-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6e4e-164">String</span></span>|<span data-ttu-id="a6e4e-165">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-165">The display name of the identity provider.</span></span>|
|<span data-ttu-id="a6e4e-166">domainHint</span><span class="sxs-lookup"><span data-stu-id="a6e4e-166">domainHint</span></span>|<span data-ttu-id="a6e4e-167">String</span><span class="sxs-lookup"><span data-stu-id="a6e4e-167">String</span></span>|<span data-ttu-id="a6e4e-168">A dica de domínio pode ser usada para pular diretamente para a página de entrada do provedor de identidade especificado, em vez de fazer com que o usuário faça uma seleção entre a lista de provedores de identidade disponíveis.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-168">The domain hint can be used to skip directly to the sign in page of the specified identity provider, instead of having the user make a selection among the list of available identity providers.</span></span>|
|<span data-ttu-id="a6e4e-169">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="a6e4e-169">claimsMapping</span></span>|[<span data-ttu-id="a6e4e-170">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="a6e4e-170">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="a6e4e-171">Depois que o provedor OIDC envia um token de ID de volta para o Azure AD, o Azure AD precisa ser capaz de mapear as declarações do token recebido para as declarações que o Azure AD reconhece e usa.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-171">After the OIDC provider sends an ID token back to Azure AD, Azure AD needs to be able to map the claims from the received token to the claims that Azure AD recognizes and uses.</span></span> <span data-ttu-id="a6e4e-172">Esse tipo complexo captura esse mapeamento.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-172">This complex type captures that mapping.</span></span>|
|<span data-ttu-id="a6e4e-173">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="a6e4e-173">metadataUrl</span></span>|<span data-ttu-id="a6e4e-174">String</span><span class="sxs-lookup"><span data-stu-id="a6e4e-174">String</span></span>|<span data-ttu-id="a6e4e-175">A URL do documento de metadados do provedor de identidade do OpenID Connect.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-175">The URL for the metadata document of the OpenID Connect identity provider.</span></span> <span data-ttu-id="a6e4e-176">Cada provedor de identidade do OpenID Connect descreve um documento de metadados que contém a maioria das informações necessárias para executar a conexão.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-176">Every OpenID Connect identity provider describes a metadata document that contains most of the information required to perform sign-in.</span></span> <span data-ttu-id="a6e4e-177">Isso inclui informações como as URLs a ser usadas e o local das chaves de assinatura públicas do serviço.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-177">This includes information such as the URLs to use and the location of the service's public signing keys.</span></span> <span data-ttu-id="a6e4e-178">O documento de metadados do OpenID Connect está sempre localizado em um ponto de extremidade que termina em `.well-known/openid-configuration` .</span><span class="sxs-lookup"><span data-stu-id="a6e4e-178">The OpenID Connect metadata document is always located at an endpoint that ends in `.well-known/openid-configuration`.</span></span> <span data-ttu-id="a6e4e-179">Forneça a URL de metadados para o provedor de identidade do OpenID Connect que você adicionar.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-179">Provide the metadata URL for the OpenID Connect identity provider you add.</span></span>|
|<span data-ttu-id="a6e4e-180">responseMode</span><span class="sxs-lookup"><span data-stu-id="a6e4e-180">responseMode</span></span>|<span data-ttu-id="a6e4e-181">String</span><span class="sxs-lookup"><span data-stu-id="a6e4e-181">String</span></span>|<span data-ttu-id="a6e4e-182">O modo de resposta define o método usado para enviar dados de volta do provedor de identidade personalizado para o Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-182">The response mode defines the method used to send data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="a6e4e-183">Valores possíveis: `form_post` , `query` .</span><span class="sxs-lookup"><span data-stu-id="a6e4e-183">Possible values: `form_post`, `query`.</span></span>|
|<span data-ttu-id="a6e4e-184">responseType</span><span class="sxs-lookup"><span data-stu-id="a6e4e-184">responseType</span></span>|<span data-ttu-id="a6e4e-185">String</span><span class="sxs-lookup"><span data-stu-id="a6e4e-185">String</span></span>|<span data-ttu-id="a6e4e-186">O tipo de resposta descreve o tipo de informação enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-186">The response type describes the type of information sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="a6e4e-187">Valores possíveis: `code` , `id_token` , `token` .</span><span class="sxs-lookup"><span data-stu-id="a6e4e-187">Possible values: `code` , `id_token` , `token`.</span></span>|
|<span data-ttu-id="a6e4e-188">escopo</span><span class="sxs-lookup"><span data-stu-id="a6e4e-188">scope</span></span>|<span data-ttu-id="a6e4e-189">String</span><span class="sxs-lookup"><span data-stu-id="a6e4e-189">String</span></span>|<span data-ttu-id="a6e4e-190">O escopo define as informações e permissões que você está procurando coletar do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-190">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

### <a name="applemanagedidentityprovider-object"></a><span data-ttu-id="a6e4e-191">Objeto appleManagedIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="a6e4e-191">appleManagedIdentityProvider object</span></span>

|<span data-ttu-id="a6e4e-192">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6e4e-192">Property</span></span>|<span data-ttu-id="a6e4e-193">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6e4e-193">Type</span></span>|<span data-ttu-id="a6e4e-194">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6e4e-194">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6e4e-195">displayName</span><span class="sxs-lookup"><span data-stu-id="a6e4e-195">displayName</span></span>|<span data-ttu-id="a6e4e-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6e4e-196">String</span></span>|<span data-ttu-id="a6e4e-197">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-197">The display name of the identity provider.</span></span>|
|<span data-ttu-id="a6e4e-198">developerId</span><span class="sxs-lookup"><span data-stu-id="a6e4e-198">developerId</span></span>|<span data-ttu-id="a6e4e-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6e4e-199">String</span></span>|<span data-ttu-id="a6e4e-200">O identificador do Desenvolvedor apple.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-200">The Apple Developer identifier.</span></span>|
|<span data-ttu-id="a6e4e-201">serviceId</span><span class="sxs-lookup"><span data-stu-id="a6e4e-201">serviceId</span></span>|<span data-ttu-id="a6e4e-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6e4e-202">String</span></span>|<span data-ttu-id="a6e4e-203">O identificador do Desenvolvedor apple.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-203">The Apple Developer identifier.</span></span>|
|<span data-ttu-id="a6e4e-204">keyId</span><span class="sxs-lookup"><span data-stu-id="a6e4e-204">keyId</span></span>|<span data-ttu-id="a6e4e-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6e4e-205">String</span></span>|<span data-ttu-id="a6e4e-206">O identificador apple key.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-206">The Apple Key identifier.</span></span>|
|<span data-ttu-id="a6e4e-207">certificateData</span><span class="sxs-lookup"><span data-stu-id="a6e4e-207">certificateData</span></span>|<span data-ttu-id="a6e4e-208">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6e4e-208">String</span></span>|<span data-ttu-id="a6e4e-209">Os dados do certificado, que são uma longa sequência de texto do certificado, podem ser nulos.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-209">The certificate data which is a long string of text from the certificate, can be null.</span></span>|

## <a name="response"></a><span data-ttu-id="a6e4e-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6e4e-210">Response</span></span>

<span data-ttu-id="a6e4e-211">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-211">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="a6e4e-212">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-212">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="a6e4e-213">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a6e4e-213">Examples</span></span>

### <a name="example-1-update-a-specific-social-identity-provider-azure-ad-or-azure-ad-b2c"></a><span data-ttu-id="a6e4e-214">Exemplo 1: Atualizar um provedor de **identidade social específico** (Azure AD ou Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="a6e4e-214">Example 1: Update a specific **social identity provider** (Azure AD or Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="a6e4e-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6e4e-215">Request</span></span>

<span data-ttu-id="a6e4e-216">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-216">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a6e4e-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6e4e-217">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a6e4e-218">C#</span><span class="sxs-lookup"><span data-stu-id="a6e4e-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-socialidentityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6e4e-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6e4e-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-socialidentityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6e4e-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6e4e-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-socialidentityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6e4e-221">Java</span><span class="sxs-lookup"><span data-stu-id="a6e4e-221">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-socialidentityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="a6e4e-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6e4e-222">Response</span></span>

<span data-ttu-id="a6e4e-223">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-223">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="a6e4e-224">Exemplo 2: atualizar um provedor de identidade **do OpenID Connect** específico (somente para o Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="a6e4e-224">Example 2: Update a specific **OpenID Connect identity provider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="a6e4e-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6e4e-225">Request</span></span>

<span data-ttu-id="a6e4e-226">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-226">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a6e4e-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6e4e-227">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a6e4e-228">C#</span><span class="sxs-lookup"><span data-stu-id="a6e4e-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openidconnectprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6e4e-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6e4e-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openidconnectprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6e4e-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6e4e-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openidconnectprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6e4e-231">Java</span><span class="sxs-lookup"><span data-stu-id="a6e4e-231">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openidconnectprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="a6e4e-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6e4e-232">Response</span></span>

<span data-ttu-id="a6e4e-233">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-233">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-a-specific-apple-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="a6e4e-234">Exemplo 3: atualizar um provedor de **identidade específico da Apple** (somente para o Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="a6e4e-234">Example 3: Update a specific **Apple identity provider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="a6e4e-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6e4e-235">Request</span></span>

<span data-ttu-id="a6e4e-236">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-236">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a6e4e-237">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6e4e-237">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a6e4e-238">C#</span><span class="sxs-lookup"><span data-stu-id="a6e4e-238">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-appleidentityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6e4e-239">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6e4e-239">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-appleidentityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6e4e-240">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6e4e-240">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-appleidentityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6e4e-241">Java</span><span class="sxs-lookup"><span data-stu-id="a6e4e-241">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-appleidentityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="a6e4e-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6e4e-242">Response</span></span>

<span data-ttu-id="a6e4e-243">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a6e4e-243">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
