---
title: Listar todos os identityProviders em um b2cIdentityUserFlow
description: Listar todos os identityProviders em um b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: f0d0dbf0cedb1ea267da23301614bd8944da7cdf
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625793"
---
# <a name="list-all-identityproviders-in-a-b2cidentityuserflow"></a><span data-ttu-id="20e77-103">Listar todos os identityProviders em um b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="20e77-103">List all identityProviders in a b2cIdentityUserFlow</span></span>

<span data-ttu-id="20e77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20e77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20e77-105">Obter os provedores de identidade em um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="20e77-105">Get the identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="20e77-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20e77-106">Permissions</span></span>

<span data-ttu-id="20e77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20e77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20e77-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20e77-109">Permission type</span></span>      | <span data-ttu-id="20e77-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20e77-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20e77-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20e77-111">Delegated (work or school account)</span></span>|<span data-ttu-id="20e77-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20e77-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="20e77-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20e77-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="20e77-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20e77-114">Not supported.</span></span>|
|<span data-ttu-id="20e77-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20e77-115">Application</span></span>| <span data-ttu-id="20e77-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20e77-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="20e77-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="20e77-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="20e77-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="20e77-118">Global administrator</span></span>
* <span data-ttu-id="20e77-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="20e77-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="20e77-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20e77-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="20e77-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20e77-121">Request headers</span></span>

|<span data-ttu-id="20e77-122">Nome</span><span class="sxs-lookup"><span data-stu-id="20e77-122">Name</span></span>|<span data-ttu-id="20e77-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="20e77-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="20e77-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="20e77-124">Authorization</span></span>|<span data-ttu-id="20e77-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20e77-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20e77-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20e77-127">Request body</span></span>

<span data-ttu-id="20e77-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20e77-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20e77-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="20e77-129">Response</span></span>

<span data-ttu-id="20e77-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` representação JSON dos [identityProviders](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20e77-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20e77-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20e77-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="20e77-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20e77-132">Request</span></span>

<span data-ttu-id="20e77-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="20e77-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="20e77-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="20e77-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="20e77-135">C#</span><span class="sxs-lookup"><span data-stu-id="20e77-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cuserflow-list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20e77-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20e77-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cuserflow-list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20e77-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20e77-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cuserflow-list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20e77-138">Java</span><span class="sxs-lookup"><span data-stu-id="20e77-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cuserflow-list-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="20e77-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="20e77-139">Response</span></span>

<span data-ttu-id="20e77-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20e77-140">The following is an example of the response.</span></span>

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


