---
title: Listar availableProviderTypes
description: Recupere todos os tipos de provedores de identidade disponíveis no diretório.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 3282ed8aff91e6fe82d62593be13efa052248abc
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921410"
---
# <a name="list-availableprovidertypes"></a><span data-ttu-id="c048b-103">Listar availableProviderTypes</span><span class="sxs-lookup"><span data-stu-id="c048b-103">List availableProviderTypes</span></span>

<span data-ttu-id="c048b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c048b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c048b-105">Recupera todos os tipos de provedor de identidade disponíveis em um diretório.</span><span class="sxs-lookup"><span data-stu-id="c048b-105">Retrieves all identity provider types available in a directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="c048b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c048b-106">Permissions</span></span>

<span data-ttu-id="c048b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c048b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c048b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c048b-109">Permission type</span></span>      | <span data-ttu-id="c048b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c048b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c048b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c048b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c048b-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c048b-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="c048b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c048b-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c048b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c048b-114">Not supported.</span></span>|
|<span data-ttu-id="c048b-115">Application</span><span class="sxs-lookup"><span data-stu-id="c048b-115">Application</span></span>|<span data-ttu-id="c048b-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c048b-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="c048b-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="c048b-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c048b-118">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="c048b-118">Global Administrator</span></span>
* <span data-ttu-id="c048b-119">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="c048b-119">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c048b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c048b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/identityProviders/availableProviderTypes
```

## <a name="request-headers"></a><span data-ttu-id="c048b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c048b-121">Request headers</span></span>

|<span data-ttu-id="c048b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c048b-122">Name</span></span>|<span data-ttu-id="c048b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c048b-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c048b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c048b-124">Authorization</span></span>|<span data-ttu-id="c048b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c048b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c048b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c048b-127">Request body</span></span>
<span data-ttu-id="c048b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c048b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c048b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c048b-129">Response</span></span>

<span data-ttu-id="c048b-130">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c048b-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c048b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c048b-131">Example</span></span>

### <a name="example-1-list-all-identityprovider-available-in-an-azure-ad-directory"></a><span data-ttu-id="c048b-132">Exemplo 1: listar **toda a identidadeProvider** disponível em um diretório do Azure AD</span><span class="sxs-lookup"><span data-stu-id="c048b-132">Example 1: List all **identityProvider** available in an Azure AD directory</span></span>

### <a name="request"></a><span data-ttu-id="c048b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c048b-133">Request</span></span>
<span data-ttu-id="c048b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c048b-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c048b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c048b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/availableProviderTypes
```
# <a name="c"></a>[<span data-ttu-id="c048b-136">C#</span><span class="sxs-lookup"><span data-stu-id="c048b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityprovider-availableprovidertypes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c048b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c048b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityprovider-availableprovidertypes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c048b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c048b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityprovider-availableprovidertypes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c048b-139">Java</span><span class="sxs-lookup"><span data-stu-id="c048b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityprovider-availableprovidertypes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="c048b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c048b-140">Response</span></span>

<span data-ttu-id="c048b-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c048b-141">The following is an example of the response.</span></span>

<span data-ttu-id="c048b-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c048b-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-identityprovider-available-in-an-azure-ad-b2c-directory"></a><span data-ttu-id="c048b-143">Exemplo 2: Listar **todos os identityProvider** disponíveis em um diretório do Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="c048b-143">Example 2: List all **identityProvider** available in an Azure AD B2C directory</span></span>

### <a name="request"></a><span data-ttu-id="c048b-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c048b-144">Request</span></span>
<span data-ttu-id="c048b-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c048b-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c048b-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="c048b-146">HTTP</span></span>](#tab/http)

# <a name="http"></a>[<span data-ttu-id="c048b-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="c048b-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes_b2c"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/availableProviderTypes
```
# <a name="c"></a>[<span data-ttu-id="c048b-148">C#</span><span class="sxs-lookup"><span data-stu-id="c048b-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityprovider-availableprovidertypes-b2c-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c048b-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c048b-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityprovider-availableprovidertypes-b2c-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c048b-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c048b-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityprovider-availableprovidertypes-b2c-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c048b-151">Java</span><span class="sxs-lookup"><span data-stu-id="c048b-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityprovider-availableprovidertypes-b2c-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="c048b-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="c048b-152">Response</span></span>

<span data-ttu-id="c048b-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c048b-153">The following is an example of the response.</span></span>

<span data-ttu-id="c048b-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c048b-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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
