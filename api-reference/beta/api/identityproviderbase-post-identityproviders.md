---
title: Criar identityProvider
description: Crie um novo objeto identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 3ec9797ea97a34d3ab6de3098ba60f52bb48770e
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546228"
---
# <a name="create-identityprovider"></a><span data-ttu-id="73dcb-103">Criar identityProvider</span><span class="sxs-lookup"><span data-stu-id="73dcb-103">Create identityProvider</span></span>

<span data-ttu-id="73dcb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73dcb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73dcb-105">Crie um novo [objeto socialIdentityProvider](../resources/socialidentityprovider.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="73dcb-105">Create a new [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="73dcb-106">No Azure AD B2C, crie um [novo objeto socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou [appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="73dcb-106">In Azure AD B2C create a new [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="73dcb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="73dcb-107">Permissions</span></span>

<span data-ttu-id="73dcb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73dcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73dcb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73dcb-110">Permission type</span></span>      | <span data-ttu-id="73dcb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73dcb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73dcb-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73dcb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73dcb-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73dcb-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="73dcb-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73dcb-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="73dcb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73dcb-115">Not supported.</span></span>|
|<span data-ttu-id="73dcb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73dcb-116">Application</span></span>|<span data-ttu-id="73dcb-117">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73dcb-117">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="73dcb-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="73dcb-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="73dcb-119">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="73dcb-119">Global Administrator</span></span>
* <span data-ttu-id="73dcb-120">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="73dcb-120">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="73dcb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73dcb-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="73dcb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73dcb-122">Request headers</span></span>

|<span data-ttu-id="73dcb-123">Nome</span><span class="sxs-lookup"><span data-stu-id="73dcb-123">Name</span></span>|<span data-ttu-id="73dcb-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="73dcb-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="73dcb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="73dcb-125">Authorization</span></span>|<span data-ttu-id="73dcb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73dcb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="73dcb-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73dcb-128">Content-Type</span></span>|<span data-ttu-id="73dcb-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73dcb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73dcb-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73dcb-131">Request body</span></span>

<span data-ttu-id="73dcb-132">No corpo da solicitação, forneça uma representação JSON do [objeto socialIdentityProvider](../resources/socialidentityprovider.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="73dcb-132">In the request body, provide a JSON representation of [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="73dcb-133">No Azure AD B2C, forneça uma representação JSON [de socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou [um objeto appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="73dcb-133">In Azure AD B2C provide a JSON representation of [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

<span data-ttu-id="73dcb-134">Todas as propriedades listadas na tabela a seguir são necessárias.</span><span class="sxs-lookup"><span data-stu-id="73dcb-134">All the properties listed in the following table are required.</span></span>

### <a name="socialidentityprovider-object"></a><span data-ttu-id="73dcb-135">Objeto socialIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="73dcb-135">socialIdentityProvider object</span></span>

|<span data-ttu-id="73dcb-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73dcb-136">Property</span></span>|<span data-ttu-id="73dcb-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="73dcb-137">Type</span></span>|<span data-ttu-id="73dcb-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="73dcb-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73dcb-139">clientId</span><span class="sxs-lookup"><span data-stu-id="73dcb-139">clientId</span></span>|<span data-ttu-id="73dcb-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dcb-140">String</span></span>|<span data-ttu-id="73dcb-141">O identificador do cliente para o aplicativo obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="73dcb-141">The client identifier for the application obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="73dcb-142">clientSecret</span><span class="sxs-lookup"><span data-stu-id="73dcb-142">clientSecret</span></span>|<span data-ttu-id="73dcb-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dcb-143">String</span></span>|<span data-ttu-id="73dcb-144">O segredo do cliente para o aplicativo obtido quando o aplicativo é registrado com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="73dcb-144">The client secret for the application that is obtained when the application is registered with the identity provider.</span></span> <span data-ttu-id="73dcb-145">Isso é somente gravação.</span><span class="sxs-lookup"><span data-stu-id="73dcb-145">This is write-only.</span></span> <span data-ttu-id="73dcb-146">Uma operação de leitura retorna "\*\*\*\*".</span><span class="sxs-lookup"><span data-stu-id="73dcb-146">A read operation returns "\*\*\*\*".</span></span>|
|<span data-ttu-id="73dcb-147">displayName</span><span class="sxs-lookup"><span data-stu-id="73dcb-147">displayName</span></span>|<span data-ttu-id="73dcb-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dcb-148">String</span></span>|<span data-ttu-id="73dcb-149">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="73dcb-149">The display name of the identity provider.</span></span>|
|<span data-ttu-id="73dcb-150">identityProviderType</span><span class="sxs-lookup"><span data-stu-id="73dcb-150">identityProviderType</span></span>|<span data-ttu-id="73dcb-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dcb-151">String</span></span>|<span data-ttu-id="73dcb-152">Para um cenário B2B, valores possíveis: `Google`, `Facebook`.</span><span class="sxs-lookup"><span data-stu-id="73dcb-152">For a B2B scenario, possible values: `Google`, `Facebook`.</span></span> <span data-ttu-id="73dcb-153">Para um cenário B2C, valores possíveis: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`.</span><span class="sxs-lookup"><span data-stu-id="73dcb-153">For a B2C scenario, possible values: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`.</span></span>|

### <a name="openidconnectidentityprovider-object"></a><span data-ttu-id="73dcb-154">Objeto openIdConnectIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="73dcb-154">openIdConnectIdentityProvider object</span></span>

|<span data-ttu-id="73dcb-155">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73dcb-155">Property</span></span>|<span data-ttu-id="73dcb-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="73dcb-156">Type</span></span>|<span data-ttu-id="73dcb-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="73dcb-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73dcb-158">clientId</span><span class="sxs-lookup"><span data-stu-id="73dcb-158">clientId</span></span>|<span data-ttu-id="73dcb-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dcb-159">String</span></span>|<span data-ttu-id="73dcb-160">A ID do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="73dcb-160">The client ID for the application obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="73dcb-161">clientSecret</span><span class="sxs-lookup"><span data-stu-id="73dcb-161">clientSecret</span></span>|<span data-ttu-id="73dcb-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dcb-162">String</span></span>|<span data-ttu-id="73dcb-163">O segredo do cliente para o aplicativo obtido ao registrar o aplicativo no provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="73dcb-163">The client secret for the application obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="73dcb-164">O clientSecret tem uma dependência de **responseType**.</span><span class="sxs-lookup"><span data-stu-id="73dcb-164">The clientSecret has a dependency on **responseType**.</span></span> <ul><li><span data-ttu-id="73dcb-165">Quando **responseType** é `code` , um segredo é necessário para a troca de código de auth.</span><span class="sxs-lookup"><span data-stu-id="73dcb-165">When **responseType** is `code`, a secret is required for the auth code exchange.</span></span></li><li><span data-ttu-id="73dcb-166">Quando **responseType** é o segredo não é necessário porque não há troca de código, o id_token é retornado `id_token` diretamente da resposta de autorização.</span><span class="sxs-lookup"><span data-stu-id="73dcb-166">When **responseType** is `id_token` the secret is not required because there is no code exchange—the id_token is returned directly from the authorization response.</span></span></li></ul>|
|<span data-ttu-id="73dcb-167">displayName</span><span class="sxs-lookup"><span data-stu-id="73dcb-167">displayName</span></span>|<span data-ttu-id="73dcb-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dcb-168">String</span></span>|<span data-ttu-id="73dcb-169">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="73dcb-169">The display name of the identity provider.</span></span>|
|<span data-ttu-id="73dcb-170">domainHint</span><span class="sxs-lookup"><span data-stu-id="73dcb-170">domainHint</span></span>|<span data-ttu-id="73dcb-171">String</span><span class="sxs-lookup"><span data-stu-id="73dcb-171">String</span></span>|<span data-ttu-id="73dcb-172">A dica de domínio pode ser usada para pular diretamente para a página de entrada do provedor de identidade especificado, em vez de fazer com que o usuário faça uma seleção entre a lista de provedores de identidade disponíveis.</span><span class="sxs-lookup"><span data-stu-id="73dcb-172">The domain hint can be used to skip directly to the sign in page of the specified identity provider, instead of having the user make a selection among the list of available identity providers.</span></span>|
|<span data-ttu-id="73dcb-173">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="73dcb-173">claimsMapping</span></span>|[<span data-ttu-id="73dcb-174">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="73dcb-174">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="73dcb-175">Depois que o provedor OIDC envia um token de ID de volta para o Azure AD, o Azure AD precisa ser capaz de mapear as declarações do token recebido para as declarações que o Azure AD reconhece e usa.</span><span class="sxs-lookup"><span data-stu-id="73dcb-175">After the OIDC provider sends an ID token back to Azure AD, Azure AD needs to be able to map the claims from the received token to the claims that Azure AD recognizes and uses.</span></span> <span data-ttu-id="73dcb-176">Esse tipo complexo captura esse mapeamento.</span><span class="sxs-lookup"><span data-stu-id="73dcb-176">This complex type captures that mapping.</span></span>|
|<span data-ttu-id="73dcb-177">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="73dcb-177">metadataUrl</span></span>|<span data-ttu-id="73dcb-178">String</span><span class="sxs-lookup"><span data-stu-id="73dcb-178">String</span></span>|<span data-ttu-id="73dcb-179">A URL do documento de metadados do provedor de Conexão OpenID.</span><span class="sxs-lookup"><span data-stu-id="73dcb-179">The URL for the metadata document of the OpenID Connect identity provider.</span></span> <span data-ttu-id="73dcb-180">Cada provedor Conexão de identidade OpenID descreve um documento de metadados que contém a maioria das informações necessárias para executar a login.</span><span class="sxs-lookup"><span data-stu-id="73dcb-180">Every OpenID Connect identity provider describes a metadata document that contains most of the information required to perform sign-in.</span></span> <span data-ttu-id="73dcb-181">Isso inclui informações como as URLs a ser usadas e o local das chaves de assinatura públicas do serviço.</span><span class="sxs-lookup"><span data-stu-id="73dcb-181">This includes information such as the URLs to use and the location of the service's public signing keys.</span></span> <span data-ttu-id="73dcb-182">O documento Conexão de metadados do OpenID está sempre localizado em um ponto de extremidade que termina em `.well-known/openid-configuration` .</span><span class="sxs-lookup"><span data-stu-id="73dcb-182">The OpenID Connect metadata document is always located at an endpoint that ends in `.well-known/openid-configuration`.</span></span> <span data-ttu-id="73dcb-183">Forneça a URL de metadados para o provedor Conexão de identidade openid que você adicionar.</span><span class="sxs-lookup"><span data-stu-id="73dcb-183">Provide the metadata URL for the OpenID Connect identity provider you add.</span></span>|
|<span data-ttu-id="73dcb-184">responseMode</span><span class="sxs-lookup"><span data-stu-id="73dcb-184">responseMode</span></span>|<span data-ttu-id="73dcb-185">String</span><span class="sxs-lookup"><span data-stu-id="73dcb-185">String</span></span>|<span data-ttu-id="73dcb-186">O modo de resposta define o método usado para enviar dados de volta do provedor de identidade personalizado para o Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="73dcb-186">The response mode defines the method used to send data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="73dcb-187">Valores possíveis: `form_post` , `query` .</span><span class="sxs-lookup"><span data-stu-id="73dcb-187">Possible values: `form_post`, `query`.</span></span>|
|<span data-ttu-id="73dcb-188">responseType</span><span class="sxs-lookup"><span data-stu-id="73dcb-188">responseType</span></span>|<span data-ttu-id="73dcb-189">String</span><span class="sxs-lookup"><span data-stu-id="73dcb-189">String</span></span>|<span data-ttu-id="73dcb-190">O tipo de resposta descreve o tipo de informação enviada de volta na chamada inicial para o authorization_endpoint do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="73dcb-190">The response type describes the type of information sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="73dcb-191">Valores possíveis: `code` , `id_token` , `token` .</span><span class="sxs-lookup"><span data-stu-id="73dcb-191">Possible values: `code` , `id_token` , `token`.</span></span>|
|<span data-ttu-id="73dcb-192">escopo</span><span class="sxs-lookup"><span data-stu-id="73dcb-192">scope</span></span>|<span data-ttu-id="73dcb-193">String</span><span class="sxs-lookup"><span data-stu-id="73dcb-193">String</span></span>|<span data-ttu-id="73dcb-194">O escopo define as informações e permissões que você está procurando coletar do provedor de identidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="73dcb-194">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

### <a name="appleidentityprovider-object"></a><span data-ttu-id="73dcb-195">Objeto appleIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="73dcb-195">appleIdentityProvider object</span></span>

|<span data-ttu-id="73dcb-196">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73dcb-196">Property</span></span>|<span data-ttu-id="73dcb-197">Tipo</span><span class="sxs-lookup"><span data-stu-id="73dcb-197">Type</span></span>|<span data-ttu-id="73dcb-198">Descrição</span><span class="sxs-lookup"><span data-stu-id="73dcb-198">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73dcb-199">displayName</span><span class="sxs-lookup"><span data-stu-id="73dcb-199">displayName</span></span>|<span data-ttu-id="73dcb-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dcb-200">String</span></span>|<span data-ttu-id="73dcb-201">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="73dcb-201">The display name of the identity provider.</span></span>|
|<span data-ttu-id="73dcb-202">developerId</span><span class="sxs-lookup"><span data-stu-id="73dcb-202">developerId</span></span>|<span data-ttu-id="73dcb-203">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dcb-203">String</span></span>|<span data-ttu-id="73dcb-204">O identificador do Desenvolvedor apple.</span><span class="sxs-lookup"><span data-stu-id="73dcb-204">The Apple Developer identifier.</span></span>|
|<span data-ttu-id="73dcb-205">serviceId</span><span class="sxs-lookup"><span data-stu-id="73dcb-205">serviceId</span></span>|<span data-ttu-id="73dcb-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dcb-206">String</span></span>|<span data-ttu-id="73dcb-207">O identificador do Desenvolvedor apple.</span><span class="sxs-lookup"><span data-stu-id="73dcb-207">The Apple Developer identifier.</span></span>|
|<span data-ttu-id="73dcb-208">keyId</span><span class="sxs-lookup"><span data-stu-id="73dcb-208">keyId</span></span>|<span data-ttu-id="73dcb-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dcb-209">String</span></span>|<span data-ttu-id="73dcb-210">O identificador apple key.</span><span class="sxs-lookup"><span data-stu-id="73dcb-210">The Apple Key identifier.</span></span>|
|<span data-ttu-id="73dcb-211">certificateData</span><span class="sxs-lookup"><span data-stu-id="73dcb-211">certificateData</span></span>|<span data-ttu-id="73dcb-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dcb-212">String</span></span>|<span data-ttu-id="73dcb-213">Os dados do certificado, que são uma longa sequência de texto do certificado, podem ser nulos.</span><span class="sxs-lookup"><span data-stu-id="73dcb-213">The certificate data which is a long string of text from the certificate, can be null.</span></span>|

## <a name="response"></a><span data-ttu-id="73dcb-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="73dcb-214">Response</span></span>

<span data-ttu-id="73dcb-215">Se tiver êxito, este método retornará um código de resposta e uma representação JSON de um `201 Created` [objeto socialIdentityProvider](../resources/socialidentityprovider.md) no corpo da resposta para um locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="73dcb-215">If successful, this method returns a `201 Created` response code and a JSON representation of a [socialIdentityProvider](../resources/socialidentityprovider.md) object in the response body for an Azure AD tenant.</span></span>

<span data-ttu-id="73dcb-216">Para um locatário do Azure AD B2C, este método retorna um código de resposta e uma representação JSON de `201 Created` [um socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou um [objeto appleIdentityProvider](../resources/appleidentityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73dcb-216">For an Azure AD B2C tenant, this method returns a `201 Created` response code and a JSON representation of a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object in the response body.</span></span>

<span data-ttu-id="73dcb-217">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="73dcb-217">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="73dcb-218">Exemplos</span><span class="sxs-lookup"><span data-stu-id="73dcb-218">Examples</span></span>

### <a name="example-1-create-a-specific-social-identity-provider-azure-ad-and-azure-ad-b2c"></a><span data-ttu-id="73dcb-219">Exemplo 1: Criar um provedor de **identidade social específico** (Azure AD e Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="73dcb-219">Example 1: Create a specific **social identity provider** (Azure AD and Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="73dcb-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73dcb-220">Request</span></span>

<span data-ttu-id="73dcb-221">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="73dcb-221">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="73dcb-222">HTTP</span><span class="sxs-lookup"><span data-stu-id="73dcb-222">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_socialidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json
Content-length: 154

{
  "@odata.type": "microsoft.graph.socialIdentityProvider",
  "displayName": "Login with Amazon",
  "identityProviderType": "Amazon",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="73dcb-223">C#</span><span class="sxs-lookup"><span data-stu-id="73dcb-223">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-socialidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73dcb-224">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73dcb-224">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-socialidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73dcb-225">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73dcb-225">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-socialidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73dcb-226">Java</span><span class="sxs-lookup"><span data-stu-id="73dcb-226">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-socialidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="73dcb-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="73dcb-227">Response</span></span>

<span data-ttu-id="73dcb-228">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="73dcb-228">The following is an example of the response.</span></span>

<span data-ttu-id="73dcb-229">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="73dcb-229">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.socialIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.type": "microsoft.graph.socialIdentityProvider",
    "id": "Amazon-OAUTH",
    "displayName": "Login with Amazon",
    "identityProviderType": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

### <a name="example-2-create-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="73dcb-230">Exemplo 2: Criar um provedor de identidade **Conexão OpenID específico** (somente para o Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="73dcb-230">Example 2: Create a specific **OpenID Connect identity provider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="73dcb-231">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73dcb-231">Request</span></span>

<span data-ttu-id="73dcb-232">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="73dcb-232">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="73dcb-233">HTTP</span><span class="sxs-lookup"><span data-stu-id="73dcb-233">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_openidconnectidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
    "displayName": "Login with the Contoso identity provider",
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
# <a name="c"></a>[<span data-ttu-id="73dcb-234">C#</span><span class="sxs-lookup"><span data-stu-id="73dcb-234">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-openidconnectidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73dcb-235">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73dcb-235">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-openidconnectidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73dcb-236">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73dcb-236">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-openidconnectidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73dcb-237">Java</span><span class="sxs-lookup"><span data-stu-id="73dcb-237">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-openidconnectidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="73dcb-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="73dcb-238">Response</span></span>

<span data-ttu-id="73dcb-239">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="73dcb-239">The following is an example of the response.</span></span>

<span data-ttu-id="73dcb-240">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="73dcb-240">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
  "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
  "displayName": "Login with the Contoso identity provider",
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

### <a name="example-3-retrieves-apple-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="73dcb-241">Exemplo 3: recupera o provedor de identidade da Apple (somente para o Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="73dcb-241">Example 3: Retrieves Apple identity provider (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="73dcb-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73dcb-242">Request</span></span>

<span data-ttu-id="73dcb-243">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="73dcb-243">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_applemanagedidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json
Content-length: 154

{
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider",
  "displayName": "Sign in with Apple",
  "developerId": "UBF8T346G9",
  "serviceId": "com.microsoft.rts.b2c.test.client",
  "keyId": "99P6D879C4",
  "certificateData": "******"
}
```

#### <a name="response"></a><span data-ttu-id="73dcb-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="73dcb-244">Response</span></span>

<span data-ttu-id="73dcb-245">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="73dcb-245">The following is an example of the response.</span></span>

<span data-ttu-id="73dcb-246">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="73dcb-246">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider",
  "id": "Apple-Managed-OIDC",
  "displayName": "Sign in with Apple",
  "developerId": "UBF8T346G9",
  "serviceId": "com.microsoft.rts.b2c.test.client",
  "keyId": "99P6D879C4",
  "certificateData": "******"
}
```
