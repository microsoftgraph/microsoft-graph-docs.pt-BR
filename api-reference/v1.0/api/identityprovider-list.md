---
title: Lista identityProviders
description: Recuperar todos os identityProviders
localization_priority: Priority
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fdc7e4323fa096d40d757426fd064179921c1ebc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441841"
---
# <a name="list-identityproviders"></a><span data-ttu-id="8a0b8-103">Lista identityProviders</span><span class="sxs-lookup"><span data-stu-id="8a0b8-103">List identityProviders</span></span>

<span data-ttu-id="8a0b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a0b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a0b8-105">Recuperar todos os [identityProviders](../resources/identityprovider.md) no diretório.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-105">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a0b8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a0b8-106">Permissions</span></span>

<span data-ttu-id="8a0b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a0b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a0b8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a0b8-109">Permission type</span></span>      | <span data-ttu-id="8a0b8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a0b8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a0b8-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a0b8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8a0b8-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a0b8-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="8a0b8-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a0b8-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8a0b8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-114">Not supported.</span></span>|
|<span data-ttu-id="8a0b8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a0b8-115">Application</span></span>|<span data-ttu-id="8a0b8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-116">Not supported.</span></span>|

<span data-ttu-id="8a0b8-117">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="8a0b8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a0b8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="8a0b8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a0b8-119">Request headers</span></span>

|<span data-ttu-id="8a0b8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8a0b8-120">Name</span></span>|<span data-ttu-id="8a0b8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a0b8-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="8a0b8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a0b8-122">Authorization</span></span>|<span data-ttu-id="8a0b8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a0b8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a0b8-125">Request body</span></span>

<span data-ttu-id="8a0b8-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a0b8-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a0b8-127">Response</span></span>

<span data-ttu-id="8a0b8-128">Se bem-sucedido, esse método retornará `200 OK` código de resposta e um conjunto de [identityProviders](../resources/identityprovider.md) em representação JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-128">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a0b8-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a0b8-129">Example</span></span>

<span data-ttu-id="8a0b8-130">O exemplo a seguir recupera todos os **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="8a0b8-130">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="8a0b8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a0b8-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8a0b8-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a0b8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list-identityproviders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="8a0b8-133">C#</span><span class="sxs-lookup"><span data-stu-id="8a0b8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a0b8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a0b8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a0b8-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a0b8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a0b8-136">Java</span><span class="sxs-lookup"><span data-stu-id="8a0b8-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8a0b8-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a0b8-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "Amazon-OAUTH",
        "name": "Login with Amazon",
        "type": "Amazon",
        "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
        "clientSecret": "*****"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

