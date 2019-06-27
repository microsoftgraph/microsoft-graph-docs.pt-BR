---
title: Obter identityProvider
description: Recuperar as propriedades de um identityProvider existente
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 90c9cec4d7a3a0dff47de37b461e087103ed7081
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277130"
---
# <a name="get-identityprovider"></a><span data-ttu-id="e12ac-103">Obter identityProvider</span><span class="sxs-lookup"><span data-stu-id="e12ac-103">Get identityProvider</span></span>

<span data-ttu-id="e12ac-104">Recuperar as propriedades de um [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="e12ac-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e12ac-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e12ac-105">Permissions</span></span>

<span data-ttu-id="e12ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e12ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e12ac-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e12ac-108">Permission type</span></span>      | <span data-ttu-id="e12ac-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e12ac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e12ac-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e12ac-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e12ac-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e12ac-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e12ac-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e12ac-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e12ac-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e12ac-113">Not supported.</span></span>|
|<span data-ttu-id="e12ac-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e12ac-114">Application</span></span>|<span data-ttu-id="e12ac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e12ac-115">Not supported.</span></span>|

<span data-ttu-id="e12ac-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="e12ac-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e12ac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e12ac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e12ac-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e12ac-118">Request headers</span></span>

|<span data-ttu-id="e12ac-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e12ac-119">Name</span></span>|<span data-ttu-id="e12ac-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e12ac-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e12ac-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e12ac-121">Authorization</span></span>|<span data-ttu-id="e12ac-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e12ac-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e12ac-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e12ac-124">Request body</span></span>

<span data-ttu-id="e12ac-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e12ac-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e12ac-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e12ac-126">Response</span></span>

<span data-ttu-id="e12ac-127">Se bem-sucedido, esse método retornará `200 OK` código de resposta e uma representação JSON do [identityProvider](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e12ac-127">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e12ac-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e12ac-128">Example</span></span>

<span data-ttu-id="e12ac-129">O exemplo a seguir recupera uma determinada **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="e12ac-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="e12ac-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e12ac-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-identityprovider"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="e12ac-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e12ac-131">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e12ac-132">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="e12ac-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e12ac-133">C#</span><span class="sxs-lookup"><span data-stu-id="e12ac-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-identityprovider-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e12ac-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="e12ac-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-identityprovider-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e12ac-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e12ac-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-identityprovider-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/identityprovider-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/identityprovider-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/identityprovider-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
