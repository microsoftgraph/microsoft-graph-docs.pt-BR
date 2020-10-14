---
title: Obter b2cAuthenticationMethodsPolicy
description: Ler as propriedades de um objeto b2cAuthenticationMethodsPolicy.
localization_priority: Priority
author: namkedia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b4dd25fce2d54aaaac451dc25ddc18a410fd1f15
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457322"
---
# <a name="get-b2cauthenticationmethodspolicy"></a><span data-ttu-id="49974-103">Obter b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="49974-103">Get b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="49974-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49974-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49974-105">Ler as propriedades de um objeto [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="49974-105">Read the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="49974-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="49974-106">Permissions</span></span>

<span data-ttu-id="49974-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49974-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49974-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49974-109">Permission type</span></span>                        | <span data-ttu-id="49974-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="49974-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="49974-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49974-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="49974-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="49974-112">Policy.Read.All</span></span>|
| <span data-ttu-id="49974-113">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="49974-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49974-114">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="49974-114">Policy.Read.All</span></span>|
| <span data-ttu-id="49974-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49974-115">Application</span></span>                            | <span data-ttu-id="49974-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="49974-116">Policy.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49974-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49974-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="49974-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49974-118">Request headers</span></span>

| <span data-ttu-id="49974-119">Nome</span><span class="sxs-lookup"><span data-stu-id="49974-119">Name</span></span>      |<span data-ttu-id="49974-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="49974-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49974-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="49974-121">Authorization</span></span> | <span data-ttu-id="49974-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49974-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49974-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49974-124">Request body</span></span>

<span data-ttu-id="49974-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49974-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49974-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="49974-126">Response</span></span>

<span data-ttu-id="49974-127">Se bem-sucedido, este método retorna um `200 OK`código de resposta e um objeto [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49974-127">If successful, this method returns a `200 OK` response code and the requested [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49974-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="49974-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="49974-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49974-129">Request</span></span>

<span data-ttu-id="49974-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="49974-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="49974-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="49974-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy
```
# <a name="c"></a>[<span data-ttu-id="49974-132">C#</span><span class="sxs-lookup"><span data-stu-id="49974-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cauthenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49974-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49974-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cauthenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49974-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49974-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cauthenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="49974-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="49974-135">Response</span></span>

<span data-ttu-id="49974-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="49974-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cAuthenticationMethodsPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#b2cAuthenticationMethodsPolicy",
    "id": "b2CAuthenticationMethodsPolicy",
    "isEmailPasswordAuthenticationEnabled": true,
    "isUserNameAuthenticationEnabled": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get b2cAuthenticationMethodsPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
