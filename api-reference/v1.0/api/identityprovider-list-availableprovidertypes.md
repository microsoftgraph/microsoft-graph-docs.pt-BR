---
title: Listar availableProviderTypes
description: Recupere todos os tipos de provedores de identidade disponíveis no diretório.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 38c2b393596c112fb6b533ac5ba2052cd9ac0b7d
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920227"
---
# <a name="list-availableprovidertypes"></a><span data-ttu-id="4fc61-103">Listar availableProviderTypes</span><span class="sxs-lookup"><span data-stu-id="4fc61-103">List availableProviderTypes</span></span>

<span data-ttu-id="4fc61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fc61-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4fc61-105">Recupera todos os tipos de provedor de identidade disponíveis em um diretório.</span><span class="sxs-lookup"><span data-stu-id="4fc61-105">Retrieves all identity provider types available in a directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fc61-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4fc61-106">Permissions</span></span>

<span data-ttu-id="4fc61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fc61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fc61-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4fc61-109">Permission type</span></span>      | <span data-ttu-id="4fc61-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4fc61-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fc61-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4fc61-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4fc61-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fc61-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="4fc61-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4fc61-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4fc61-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4fc61-114">Not supported.</span></span>|
|<span data-ttu-id="4fc61-115">Application</span><span class="sxs-lookup"><span data-stu-id="4fc61-115">Application</span></span>|<span data-ttu-id="4fc61-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fc61-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="4fc61-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="4fc61-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="4fc61-118">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="4fc61-118">Global Administrator</span></span>
* <span data-ttu-id="4fc61-119">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="4fc61-119">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="4fc61-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4fc61-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/availableProviderTypes
```

## <a name="request-headers"></a><span data-ttu-id="4fc61-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fc61-121">Request headers</span></span>

|<span data-ttu-id="4fc61-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4fc61-122">Name</span></span>|<span data-ttu-id="4fc61-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fc61-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="4fc61-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4fc61-124">Authorization</span></span>|<span data-ttu-id="4fc61-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fc61-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fc61-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4fc61-127">Request body</span></span>

<span data-ttu-id="4fc61-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4fc61-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fc61-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fc61-129">Response</span></span>

<span data-ttu-id="4fc61-130">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4fc61-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fc61-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4fc61-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fc61-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4fc61-132">Request</span></span>

<span data-ttu-id="4fc61-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4fc61-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4fc61-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fc61-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identityProviders/availableProviderTypes
```
# <a name="c"></a>[<span data-ttu-id="4fc61-135">C#</span><span class="sxs-lookup"><span data-stu-id="4fc61-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityprovider-availableprovidertypes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4fc61-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fc61-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityprovider-availableprovidertypes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4fc61-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4fc61-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityprovider-availableprovidertypes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4fc61-138">Java</span><span class="sxs-lookup"><span data-stu-id="4fc61-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityprovider-availableprovidertypes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4fc61-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fc61-139">Response</span></span>

<span data-ttu-id="4fc61-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4fc61-140">The following is an example of the response.</span></span>

<span data-ttu-id="4fc61-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4fc61-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "value": [
      "Google",
      "Facebook",
      "MicrosoftAccount",
      "EmailOTP"
  ]
}
```
