---
title: Listar todos os identityProviders em um b2xIdentityUserFlow
description: Listar todos os identityProviders em um b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c741e8251ec5ce0de6d169580687346fbf4e0502
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961075"
---
# <a name="list-all-identityproviders-in-a-b2xidentityuserflow"></a><span data-ttu-id="c8f0d-103">Listar todos os identityProviders em um b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="c8f0d-103">List all identityProviders in a b2xIdentityUserFlow</span></span>

<span data-ttu-id="c8f0d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8f0d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8f0d-105">Obtenha os provedores de identidade em um objeto [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="c8f0d-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8f0d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c8f0d-106">Permissions</span></span>

<span data-ttu-id="c8f0d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8f0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8f0d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8f0d-109">Permission type</span></span>      | <span data-ttu-id="c8f0d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8f0d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8f0d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8f0d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c8f0d-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8f0d-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c8f0d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8f0d-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c8f0d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8f0d-114">Not supported.</span></span>|
|<span data-ttu-id="c8f0d-115">Application</span><span class="sxs-lookup"><span data-stu-id="c8f0d-115">Application</span></span>| <span data-ttu-id="c8f0d-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8f0d-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c8f0d-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="c8f0d-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c8f0d-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c8f0d-118">Global administrator</span></span>
* <span data-ttu-id="c8f0d-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="c8f0d-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c8f0d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8f0d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /b2xUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="c8f0d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8f0d-121">Request headers</span></span>

|<span data-ttu-id="c8f0d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c8f0d-122">Name</span></span>|<span data-ttu-id="c8f0d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8f0d-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c8f0d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8f0d-124">Authorization</span></span>|<span data-ttu-id="c8f0d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8f0d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8f0d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8f0d-127">Request body</span></span>

<span data-ttu-id="c8f0d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8f0d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8f0d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8f0d-129">Response</span></span>

<span data-ttu-id="c8f0d-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma representação JSON do [identityProviders](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8f0d-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8f0d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8f0d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8f0d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8f0d-132">Request</span></span>

<span data-ttu-id="c8f0d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8f0d-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c8f0d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8f0d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="c8f0d-135">C#</span><span class="sxs-lookup"><span data-stu-id="c8f0d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflow-list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8f0d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8f0d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflow-list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8f0d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8f0d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflow-list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8f0d-138">Java</span><span class="sxs-lookup"><span data-stu-id="c8f0d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflow-list-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c8f0d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8f0d-139">Response</span></span>

<span data-ttu-id="c8f0d-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c8f0d-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
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


