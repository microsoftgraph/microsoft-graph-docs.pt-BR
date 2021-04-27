---
title: Listar userFlows
description: Recupere uma lista de objetos userFlow.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: db3b83e151abb09f443c703eeda03daa8391560e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040704"
---
# <a name="list-userflows"></a><span data-ttu-id="ce04f-103">Listar userFlows</span><span class="sxs-lookup"><span data-stu-id="ce04f-103">List userFlows</span></span>

<span data-ttu-id="ce04f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce04f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce04f-105">Recuperar uma lista de [fluxos de usuários](../resources/identityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="ce04f-105">Retrieve a list of [userflows](../resources/identityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ce04f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce04f-106">Permissions</span></span>

<span data-ttu-id="ce04f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce04f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce04f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce04f-109">Permission type</span></span>                        | <span data-ttu-id="ce04f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce04f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ce04f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce04f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce04f-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce04f-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>  |
| <span data-ttu-id="ce04f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce04f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce04f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce04f-114">Not supported.</span></span> |
| <span data-ttu-id="ce04f-115">Application</span><span class="sxs-lookup"><span data-stu-id="ce04f-115">Application</span></span>                            | <span data-ttu-id="ce04f-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce04f-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce04f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce04f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="ce04f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce04f-118">Request headers</span></span>

| <span data-ttu-id="ce04f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ce04f-119">Name</span></span>      |<span data-ttu-id="ce04f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce04f-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce04f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce04f-121">Authorization</span></span> | <span data-ttu-id="ce04f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce04f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce04f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce04f-124">Request body</span></span>

<span data-ttu-id="ce04f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ce04f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce04f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce04f-126">Response</span></span>

<span data-ttu-id="ce04f-127">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos userFlow](../resources/identityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce04f-127">If successful, this method returns a `200 OK` response code and a collection of [userFlow](../resources/identityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce04f-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ce04f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce04f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce04f-129">Request</span></span>

<span data-ttu-id="ce04f-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce04f-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce04f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce04f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflows"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows
```
# <a name="c"></a>[<span data-ttu-id="ce04f-132">C#</span><span class="sxs-lookup"><span data-stu-id="ce04f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce04f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce04f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce04f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce04f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce04f-135">Java</span><span class="sxs-lookup"><span data-stu-id="ce04f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ce04f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce04f-136">Response</span></span>

<span data-ttu-id="ce04f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce04f-137">The following is an example of the response.</span></span>

> <span data-ttu-id="ce04f-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ce04f-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "B2C_1_UserFlow1",
      "userFlowType": "signUpOrSignIn",
      "userFlowTypeVersion": 1
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userFlows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_userflows/container/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->


