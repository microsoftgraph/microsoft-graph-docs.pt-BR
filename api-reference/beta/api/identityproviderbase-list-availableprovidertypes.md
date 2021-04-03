---
title: Listar availableProviderTypes
description: Recupere todos os tipos de provedores de identidade disponíveis no diretório.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 0bcc55cca6117d42bf473c21e1578a4e36ef7574
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508789"
---
# <a name="list-availableprovidertypes"></a><span data-ttu-id="7f0bf-103">Listar availableProviderTypes</span><span class="sxs-lookup"><span data-stu-id="7f0bf-103">List availableProviderTypes</span></span>

<span data-ttu-id="7f0bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f0bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f0bf-105">Recupera todos os tipos de provedor de identidade disponíveis em um diretório.</span><span class="sxs-lookup"><span data-stu-id="7f0bf-105">Retrieves all identity provider types available in a directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f0bf-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7f0bf-106">Permissions</span></span>

<span data-ttu-id="7f0bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f0bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f0bf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f0bf-109">Permission type</span></span>      | <span data-ttu-id="7f0bf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f0bf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f0bf-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f0bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7f0bf-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f0bf-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="7f0bf-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f0bf-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7f0bf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f0bf-114">Not supported.</span></span>|
|<span data-ttu-id="7f0bf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f0bf-115">Application</span></span>|<span data-ttu-id="7f0bf-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f0bf-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="7f0bf-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="7f0bf-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="7f0bf-118">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="7f0bf-118">Global Administrator</span></span>
* <span data-ttu-id="7f0bf-119">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="7f0bf-119">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7f0bf-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f0bf-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/identityProviders/availableProviderTypes
```

## <a name="request-headers"></a><span data-ttu-id="7f0bf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f0bf-121">Request headers</span></span>

|<span data-ttu-id="7f0bf-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7f0bf-122">Name</span></span>|<span data-ttu-id="7f0bf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f0bf-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="7f0bf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f0bf-124">Authorization</span></span>|<span data-ttu-id="7f0bf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f0bf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f0bf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f0bf-127">Request body</span></span>
<span data-ttu-id="7f0bf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f0bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f0bf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f0bf-129">Response</span></span>

<span data-ttu-id="7f0bf-130">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f0bf-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f0bf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f0bf-131">Example</span></span>

### <a name="example-1-list-all-identityprovider-available-in-an-azure-ad-directory"></a><span data-ttu-id="7f0bf-132">Exemplo 1: listar **toda a identidadeProvider** disponível em um diretório do Azure AD</span><span class="sxs-lookup"><span data-stu-id="7f0bf-132">Example 1: List all **identityProvider** available in an Azure AD directory</span></span>

### <a name="request"></a><span data-ttu-id="7f0bf-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f0bf-133">Request</span></span>
<span data-ttu-id="7f0bf-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f0bf-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f0bf-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f0bf-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/availableProviderTypes
```
# <a name="c"></a>[<span data-ttu-id="7f0bf-136">C#</span><span class="sxs-lookup"><span data-stu-id="7f0bf-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityprovider-availableprovidertypes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f0bf-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f0bf-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityprovider-availableprovidertypes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f0bf-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f0bf-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityprovider-availableprovidertypes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f0bf-139">Java</span><span class="sxs-lookup"><span data-stu-id="7f0bf-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityprovider-availableprovidertypes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="7f0bf-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f0bf-140">Response</span></span>

<span data-ttu-id="7f0bf-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f0bf-141">The following is an example of the response.</span></span>

<span data-ttu-id="7f0bf-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7f0bf-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
    "value": [
        "MicrosoftAccount",
        "EmailOTP",
        "Facebook",
        "Google"
    ]
}
```

### <a name="example-2-list-all-identityprovider-available-in-an-azure-ad-b2c-directory"></a><span data-ttu-id="7f0bf-143">Exemplo 2: Listar **todos os identityProvider** disponíveis em um diretório do Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="7f0bf-143">Example 2: List all **identityProvider** available in an Azure AD B2C directory</span></span>

### <a name="request"></a><span data-ttu-id="7f0bf-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f0bf-144">Request</span></span>
<span data-ttu-id="7f0bf-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f0bf-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f0bf-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f0bf-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes_b2c"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/availableProviderTypes
```

---

### <a name="response"></a><span data-ttu-id="7f0bf-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f0bf-147">Response</span></span>

<span data-ttu-id="7f0bf-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f0bf-148">The following is an example of the response.</span></span>

<span data-ttu-id="7f0bf-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7f0bf-149">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
 "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
  "value": [
        "Microsoft",
        "Google",
        "Facebook",
        "Amazon",
        "LinkedIn",
        "Weibo",
        "QQ",
        "WeChat",
        "Twitter",
        "GitHub",
        "AppleManaged",
        "OpenIdConnect"
  ]
}
```
