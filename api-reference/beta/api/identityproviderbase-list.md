---
title: Lista identityProviders
description: Recupere uma lista de objetos identityProviderbase.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: a61ccdc32cc83c5e2a520e72b30a61d1478f7cd2
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491053"
---
# <a name="list-identityproviders"></a><span data-ttu-id="1eb77-103">Lista identityProviders</span><span class="sxs-lookup"><span data-stu-id="1eb77-103">List identityProviders</span></span>
<span data-ttu-id="1eb77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1eb77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1eb77-105">Recuperar uma lista de conjunto de objetos herdados  [de identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="1eb77-105">Retrieve a list of collection of object inherited from  [identityProviderBase](../resources/identityproviderbase.md).</span></span>

<span data-ttu-id="1eb77-106">Para um locatário do Azure AD, ele pode ser [socialIdentityProviders](../resources/socialidentityprovider.md) e/ou [objetos builtinIdentityProviders.](../resources/builtinidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="1eb77-106">For an Azure AD tenant it can be [socialIdentityProviders](../resources/socialidentityprovider.md) and/or [builtinIdentityProviders](../resources/builtinidentityprovider.md) objects.</span></span>

<span data-ttu-id="1eb77-107">Para um locatário do Azure AD B2C, pode ser [socialIdentityProviders,](../resources/socialidentityprovider.md) [objetos openIdConnectIdentityProviders](../resources/openidconnectidentityprovider.md) e/ou [appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="1eb77-107">For an Azure AD B2C tenant it can be [socialIdentityProviders](../resources/socialidentityprovider.md), [openIdConnectIdentityProviders](../resources/openidconnectidentityprovider.md) and/or [appleIdentityProvider](../resources/appleidentityprovider.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1eb77-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1eb77-108">Permissions</span></span>

<span data-ttu-id="1eb77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1eb77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1eb77-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1eb77-111">Permission type</span></span>      | <span data-ttu-id="1eb77-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1eb77-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1eb77-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1eb77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1eb77-114">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1eb77-114">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="1eb77-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1eb77-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1eb77-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1eb77-116">Not supported.</span></span>|
|<span data-ttu-id="1eb77-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1eb77-117">Application</span></span>|<span data-ttu-id="1eb77-118">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1eb77-118">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="1eb77-119">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="1eb77-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="1eb77-120">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="1eb77-120">Global Administrator</span></span>
* <span data-ttu-id="1eb77-121">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="1eb77-121">External Identity Provider Administrator</span></span>
* <span data-ttu-id="1eb77-122">Administrador de fluxo de usuário de ID externa</span><span class="sxs-lookup"><span data-stu-id="1eb77-122">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1eb77-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1eb77-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="1eb77-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb77-124">Request headers</span></span>

|<span data-ttu-id="1eb77-125">Nome</span><span class="sxs-lookup"><span data-stu-id="1eb77-125">Name</span></span>|<span data-ttu-id="1eb77-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="1eb77-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1eb77-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="1eb77-127">Authorization</span></span>|<span data-ttu-id="1eb77-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1eb77-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1eb77-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb77-130">Request body</span></span>

<span data-ttu-id="1eb77-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1eb77-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1eb77-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eb77-132">Response</span></span>

<span data-ttu-id="1eb77-133">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [socialIdentityProvider](../resources/socialidentityprovider.md) e/ou [builtinIdentityProvider](../resources/builtinidentityprovider.md) no corpo da resposta para um locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1eb77-133">If successful, this method returns a `200 OK` response code and a collection of [socialIdentityProvider](../resources/socialidentityprovider.md) and/or [builtinIdentityProvider](../resources/builtinidentityprovider.md) objects in the response body for an Azure AD tenant.</span></span>

<span data-ttu-id="1eb77-134">Para um locatário do Azure AD B2C, este método retorna um código de resposta e uma coleção de objetos `200 OK` [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) e/ou [appleIdentityProvider](../resources/appleidentityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1eb77-134">For an Azure AD B2C tenant this method returns a `200 OK` response code and a collection of [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) and/or [appleIdentityProvider](../resources/appleidentityprovider.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1eb77-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1eb77-135">Example</span></span>

### <a name="example-1-list-all-identityprovider-configured-in-an-azure-ad-tenant"></a><span data-ttu-id="1eb77-136">Exemplo 1: listar **toda a identidadeProvider** configurada em um locatário do Azure AD</span><span class="sxs-lookup"><span data-stu-id="1eb77-136">Example 1: List all **identityProvider** configured in an Azure AD tenant</span></span>

### <a name="request"></a><span data-ttu-id="1eb77-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb77-137">Request</span></span>
<span data-ttu-id="1eb77-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1eb77-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders
```

### <a name="response"></a><span data-ttu-id="1eb77-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eb77-139">Response</span></span>
<span data-ttu-id="1eb77-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1eb77-140">The following is an example of the response.</span></span>

<span data-ttu-id="1eb77-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1eb77-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase",
  "isCollection": true
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/identityProviders",
   "value":[
      {
         "@odata.type": "microsoft.graph.builtInIdentityProvider",
         "id": "MSASignup-OAUTH",
         "identityProviderType": "MicrosoftAccount",
         "displayName": "MicrosoftAccount"
      },
      {
         "@odata.type": "#microsoft.graph.socialIdentityProvider",
         "id": "Facebook-OAUTH",
         "displayName": "Facebook",
         "identityProviderType": "Facebook",
         "clientId": "test",
         "clientSecret": "******"
      }
   ]
}
```

### <a name="example-2-list-all-identityprovider-configured-in-an-azure-ad-b2c-tenant"></a><span data-ttu-id="1eb77-142">Exemplo 2: listar **toda a identidadeProvider** configurada em um locatário do Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="1eb77-142">Example 2: List all **identityProvider** configured in an Azure AD B2C tenant</span></span>

### <a name="request"></a><span data-ttu-id="1eb77-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb77-143">Request</span></span>
<span data-ttu-id="1eb77-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1eb77-144">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders
```

### <a name="response"></a><span data-ttu-id="1eb77-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eb77-145">Response</span></span>
<span data-ttu-id="1eb77-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1eb77-146">The following is an example of the response.</span></span>

<span data-ttu-id="1eb77-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1eb77-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/identityProviders",
    "value": [
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "LinkedIn-OAUTH",
            "displayName": "linkedin",
            "identityProviderType": "LinkedIn",
            "clientId": "866xc0qtyy00ih",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.openIdConnectIdentityProvider",
            "id": "OIDC-V1-rtt_AD_Test-3e393390-ed2d-4794-97f6-5c1a1ccc61f7",
            "displayName": "OIDC AD Test",
            "clientId": "fe1b3476-rdca-4bef-b321-076fde19750b",
            "clientSecret": "******",
            "scope": "openid",
            "metadataUrl": "https://login.microsoftonline.com/sashawho.onmicrosoft.com/.well-known/openid-configuration",
            "domainHint": "",
            "responseType": "code",
            "responseMode": "form_post",
            "claimsMapping": {
                "userId": "oid",
                "displayName": "name",
                "givenName": "given_name",
                "surname": "family_name",
                "email": "unique_email"
            }
        },
        {
            "@odata.type": "#microsoft.graph.appleManagedIdentityProvider",
            "id": "Apple-Managed-OIDC",
            "displayName": "Sign in with Apple",
            "developerId": "UBF8T346G9",
            "serviceId": "com.microsoft.aad.b2c.iuyt.client",
            "keyId": "99P6DD87C4",
            "certificateData": "******"
        }
    ]
}

```
