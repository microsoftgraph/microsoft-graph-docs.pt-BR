---
title: Lista identityProviders
description: Listar todos os identityProviders em um b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: f7bc5bea06e7fd6f659d0c5567079b04d3b2f3c8
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919925"
---
# <a name="list-identityproviders"></a><span data-ttu-id="fcf27-103">Lista identityProviders</span><span class="sxs-lookup"><span data-stu-id="fcf27-103">List identityProviders</span></span>

<span data-ttu-id="fcf27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcf27-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fcf27-105">Obter os provedores de identidade em um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="fcf27-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcf27-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fcf27-106">Permissions</span></span>

<span data-ttu-id="fcf27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcf27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcf27-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcf27-109">Permission type</span></span>      | <span data-ttu-id="fcf27-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fcf27-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcf27-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcf27-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fcf27-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcf27-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="fcf27-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcf27-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fcf27-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcf27-114">Not supported.</span></span>|
|<span data-ttu-id="fcf27-115">Application</span><span class="sxs-lookup"><span data-stu-id="fcf27-115">Application</span></span>| <span data-ttu-id="fcf27-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcf27-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="fcf27-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="fcf27-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="fcf27-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="fcf27-118">Global administrator</span></span>
* <span data-ttu-id="fcf27-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="fcf27-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="fcf27-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcf27-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="fcf27-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf27-121">Request headers</span></span>

|<span data-ttu-id="fcf27-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fcf27-122">Name</span></span>|<span data-ttu-id="fcf27-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcf27-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fcf27-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcf27-124">Authorization</span></span>|<span data-ttu-id="fcf27-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcf27-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcf27-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf27-127">Request body</span></span>

<span data-ttu-id="fcf27-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fcf27-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcf27-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcf27-129">Response</span></span>

<span data-ttu-id="fcf27-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` representação JSON dos [identityProviders](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fcf27-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcf27-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fcf27-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcf27-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf27-132">Request</span></span>

<span data-ttu-id="fcf27-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcf27-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fcf27-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fcf27-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="fcf27-135">C#</span><span class="sxs-lookup"><span data-stu-id="fcf27-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflow-list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fcf27-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fcf27-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflow-list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fcf27-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fcf27-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflow-list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fcf27-138">Java</span><span class="sxs-lookup"><span data-stu-id="fcf27-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflow-list-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fcf27-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcf27-139">Response</span></span>

<span data-ttu-id="fcf27-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fcf27-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "Facebook-OAuth",
            "type": "Facebook",
            "name": "Facebook",
            "clientId": "clientIdFromFacebook",
            "clientSecret": "*****"
        },
        {
            "id": "Google-OAuth",
            "type": "Google",
            "name": "Google",
            "clientId": "clientIdFromGoogle",
            "clientSecret": "*****"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
 "description": "get_b2xuserflow_list_identityproviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
