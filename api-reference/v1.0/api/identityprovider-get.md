---
title: Obter identityProvider
description: Recuperar as propriedades de um identityProvider existente
localization_priority: Priority
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5d45ab0b1c315793bffd376d90fb22dc175886e5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434276"
---
# <a name="get-identityprovider"></a><span data-ttu-id="0fd88-103">Obter identityProvider</span><span class="sxs-lookup"><span data-stu-id="0fd88-103">Get identityProvider</span></span>

<span data-ttu-id="0fd88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fd88-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0fd88-105">Recuperar as propriedades de um [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="0fd88-105">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0fd88-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0fd88-106">Permissions</span></span>

<span data-ttu-id="0fd88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fd88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fd88-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fd88-109">Permission type</span></span>      | <span data-ttu-id="0fd88-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0fd88-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fd88-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fd88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0fd88-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fd88-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="0fd88-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fd88-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0fd88-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fd88-114">Not supported.</span></span>|
|<span data-ttu-id="0fd88-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fd88-115">Application</span></span>|<span data-ttu-id="0fd88-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fd88-116">Not supported.</span></span>|

<span data-ttu-id="0fd88-117">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="0fd88-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="0fd88-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fd88-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0fd88-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fd88-119">Request headers</span></span>

|<span data-ttu-id="0fd88-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0fd88-120">Name</span></span>|<span data-ttu-id="0fd88-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fd88-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="0fd88-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fd88-122">Authorization</span></span>|<span data-ttu-id="0fd88-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fd88-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fd88-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fd88-125">Request body</span></span>

<span data-ttu-id="0fd88-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0fd88-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fd88-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fd88-127">Response</span></span>

<span data-ttu-id="0fd88-128">Se bem-sucedido, esse método retornará `200 OK` código de resposta e uma representação JSON do [identityProvider](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fd88-128">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fd88-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fd88-129">Example</span></span>

<span data-ttu-id="0fd88-130">O exemplo a seguir recupera uma determinada **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="0fd88-130">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="0fd88-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fd88-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0fd88-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fd88-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-identityprovider"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```
# <a name="c"></a>[<span data-ttu-id="0fd88-133">C#</span><span class="sxs-lookup"><span data-stu-id="0fd88-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fd88-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fd88-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fd88-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fd88-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fd88-136">Java</span><span class="sxs-lookup"><span data-stu-id="0fd88-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0fd88-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fd88-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

