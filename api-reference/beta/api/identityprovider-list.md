---
title: Lista identityProviders
description: Recuperar todos os identityProviders no diretório.
localization_priority: Normal
ms.openlocfilehash: c7ddabf8aef2a4d50f6ea133ecf696c8bdda922b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262661"
---
# <a name="list-identityproviders"></a><span data-ttu-id="dd634-103">Lista identityProviders</span><span class="sxs-lookup"><span data-stu-id="dd634-103">List identityProviders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd634-104">Recuperar todos os [identityProviders](../resources/identityprovider.md) no diretório.</span><span class="sxs-lookup"><span data-stu-id="dd634-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd634-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd634-105">Permissions</span></span>

<span data-ttu-id="dd634-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd634-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd634-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd634-108">Permission type</span></span>      | <span data-ttu-id="dd634-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd634-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd634-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd634-110">Delegated (work or school account)</span></span>|<span data-ttu-id="dd634-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd634-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="dd634-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd634-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="dd634-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd634-113">Not supported.</span></span>|
|<span data-ttu-id="dd634-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd634-114">Application</span></span>|<span data-ttu-id="dd634-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd634-115">Not supported.</span></span>|

<span data-ttu-id="dd634-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="dd634-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="dd634-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd634-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="dd634-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd634-118">Request headers</span></span>

|<span data-ttu-id="dd634-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dd634-119">Name</span></span>|<span data-ttu-id="dd634-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd634-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="dd634-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd634-121">Authorization</span></span>|<span data-ttu-id="dd634-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd634-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd634-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd634-124">Request body</span></span>

<span data-ttu-id="dd634-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dd634-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd634-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd634-126">Response</span></span>

<span data-ttu-id="dd634-127">Se bem-sucedido, esse método retornará `200 OK` código de resposta e um conjunto de [identityProviders](../resources/identityprovider.md) em representação JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd634-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd634-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd634-128">Example</span></span>

<span data-ttu-id="dd634-129">O exemplo a seguir recupera todos os **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="dd634-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="dd634-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd634-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```

##### <a name="response"></a><span data-ttu-id="dd634-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd634-131">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="dd634-132">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="dd634-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dd634-133">C#</span><span class="sxs-lookup"><span data-stu-id="dd634-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_identityproviders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd634-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="dd634-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_identityproviders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dd634-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dd634-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_identityproviders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/identityprovider-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/identityprovider-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
