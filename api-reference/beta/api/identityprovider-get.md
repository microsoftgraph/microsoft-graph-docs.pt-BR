---
title: Obter identityProvider
description: Recupere as propriedades de um identityprovider existente.
localization_priority: Normal
doc_type: apiPageType
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d5f42b514f1b6c72d5c301121494a5a8de4bd708
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446496"
---
# <a name="get-identityprovider"></a><span data-ttu-id="d0121-103">Obter identityProvider</span><span class="sxs-lookup"><span data-stu-id="d0121-103">Get identityProvider</span></span>

<span data-ttu-id="d0121-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d0121-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0121-105">Recuperar as propriedades de um [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="d0121-105">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d0121-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0121-106">Permissions</span></span>

<span data-ttu-id="d0121-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0121-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0121-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0121-109">Permission type</span></span>      | <span data-ttu-id="d0121-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0121-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0121-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0121-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d0121-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0121-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="d0121-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0121-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d0121-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0121-114">Not supported.</span></span>|
|<span data-ttu-id="d0121-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0121-115">Application</span></span>|<span data-ttu-id="d0121-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0121-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="d0121-117">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="d0121-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="d0121-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0121-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d0121-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0121-119">Request headers</span></span>

|<span data-ttu-id="d0121-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d0121-120">Name</span></span>|<span data-ttu-id="d0121-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0121-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d0121-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0121-122">Authorization</span></span>|<span data-ttu-id="d0121-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0121-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0121-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0121-125">Request body</span></span>

<span data-ttu-id="d0121-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0121-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0121-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0121-127">Response</span></span>

<span data-ttu-id="d0121-128">Se bem-sucedido, esse método retornará `200 OK` código de resposta e uma representação JSON do [identityProvider](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0121-128">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0121-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0121-129">Example</span></span>

<span data-ttu-id="d0121-130">O exemplo a seguir recupera uma determinada **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="d0121-130">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="d0121-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0121-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d0121-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0121-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```
# <a name="c"></a>[<span data-ttu-id="d0121-133">C#</span><span class="sxs-lookup"><span data-stu-id="d0121-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0121-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0121-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0121-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0121-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d0121-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0121-136">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
