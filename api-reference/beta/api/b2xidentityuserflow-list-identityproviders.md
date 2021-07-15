---
title: Listar todos os identityProviders em um b2xIdentityUserFlow (preterido)
description: Listar todos os identityProviders em um b2xIdentityUserFlow (preterido).
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 7b92da67e8969ffb54fe6a65469f6bd428d6e240
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439627"
---
# <a name="list-all-identityproviders-in-a-b2xidentityuserflow-deprecated"></a><span data-ttu-id="240c8-103">Listar todos os identityProviders em um b2xIdentityUserFlow (preterido)</span><span class="sxs-lookup"><span data-stu-id="240c8-103">List all identityProviders in a b2xIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="240c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="240c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="240c8-105">Obter os provedores de identidade em um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="240c8-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="240c8-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="240c8-106">Permissions</span></span>

<span data-ttu-id="240c8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="240c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="240c8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="240c8-109">Permission type</span></span>      | <span data-ttu-id="240c8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="240c8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="240c8-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="240c8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="240c8-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="240c8-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="240c8-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="240c8-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="240c8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="240c8-114">Not supported.</span></span>|
|<span data-ttu-id="240c8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="240c8-115">Application</span></span>| <span data-ttu-id="240c8-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="240c8-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="240c8-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="240c8-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="240c8-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="240c8-118">Global administrator</span></span>
* <span data-ttu-id="240c8-119">Administrador de identidade externa Flow usuário</span><span class="sxs-lookup"><span data-stu-id="240c8-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="240c8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="240c8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="240c8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="240c8-121">Request headers</span></span>

|<span data-ttu-id="240c8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="240c8-122">Name</span></span>|<span data-ttu-id="240c8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="240c8-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="240c8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="240c8-124">Authorization</span></span>|<span data-ttu-id="240c8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="240c8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="240c8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="240c8-127">Request body</span></span>

<span data-ttu-id="240c8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="240c8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="240c8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="240c8-129">Response</span></span>

<span data-ttu-id="240c8-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` representação JSON dos [identityProviders](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="240c8-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="240c8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="240c8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="240c8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="240c8-132">Request</span></span>

<span data-ttu-id="240c8-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="240c8-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="240c8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="240c8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="240c8-135">C#</span><span class="sxs-lookup"><span data-stu-id="240c8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflow-list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="240c8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="240c8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflow-list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="240c8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="240c8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflow-list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="240c8-138">Java</span><span class="sxs-lookup"><span data-stu-id="240c8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflow-list-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="240c8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="240c8-139">Response</span></span>

<span data-ttu-id="240c8-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="240c8-140">The following is an example of the response.</span></span>

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
