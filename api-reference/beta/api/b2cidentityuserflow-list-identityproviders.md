---
title: Listar todos os identityProviders em um b2cIdentityUserFlow
description: Listar todos os identityProviders em um b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: e908159c657016f7b36d1886e3d3b501503b295b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438299"
---
# <a name="list-all-identityproviders-in-a-b2cidentityuserflow"></a><span data-ttu-id="c68a7-103">Listar todos os identityProviders em um b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="c68a7-103">List all identityProviders in a b2cIdentityUserFlow</span></span>

<span data-ttu-id="c68a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c68a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c68a7-105">Obter os provedores de identidade em um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="c68a7-105">Get the identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c68a7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c68a7-106">Permissions</span></span>

<span data-ttu-id="c68a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c68a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c68a7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c68a7-109">Permission type</span></span>      | <span data-ttu-id="c68a7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c68a7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c68a7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c68a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c68a7-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c68a7-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c68a7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c68a7-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c68a7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c68a7-114">Not supported.</span></span>|
|<span data-ttu-id="c68a7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c68a7-115">Application</span></span>| <span data-ttu-id="c68a7-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c68a7-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c68a7-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="c68a7-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c68a7-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c68a7-118">Global administrator</span></span>
* <span data-ttu-id="c68a7-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="c68a7-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c68a7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c68a7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /b2cUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="c68a7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c68a7-121">Request headers</span></span>

|<span data-ttu-id="c68a7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c68a7-122">Name</span></span>|<span data-ttu-id="c68a7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c68a7-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c68a7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c68a7-124">Authorization</span></span>|<span data-ttu-id="c68a7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c68a7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c68a7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c68a7-127">Request body</span></span>

<span data-ttu-id="c68a7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c68a7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c68a7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c68a7-129">Response</span></span>

<span data-ttu-id="c68a7-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` representação JSON dos [identityProviders](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c68a7-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c68a7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c68a7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c68a7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c68a7-132">Request</span></span>

<span data-ttu-id="c68a7-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c68a7-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c68a7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c68a7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="c68a7-135">C#</span><span class="sxs-lookup"><span data-stu-id="c68a7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cuserflow-list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c68a7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c68a7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cuserflow-list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c68a7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c68a7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cuserflow-list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c68a7-138">Java</span><span class="sxs-lookup"><span data-stu-id="c68a7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cuserflow-list-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c68a7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c68a7-139">Response</span></span>

<span data-ttu-id="c68a7-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c68a7-140">The following is an example of the response.</span></span>

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


