---
title: Lista identityProviders
description: Recuperar todos os identityProviders
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b0390da4e197ef2038d7e9a54801259e5b91634d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613380"
---
# <a name="list-identityproviders"></a><span data-ttu-id="ed6c5-103">Lista identityProviders</span><span class="sxs-lookup"><span data-stu-id="ed6c5-103">List identityProviders</span></span>

<span data-ttu-id="ed6c5-104">Recuperar todos os [identityProviders](../resources/identityprovider.md) no diretório.</span><span class="sxs-lookup"><span data-stu-id="ed6c5-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed6c5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed6c5-105">Permissions</span></span>

<span data-ttu-id="ed6c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed6c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed6c5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed6c5-108">Permission type</span></span>      | <span data-ttu-id="ed6c5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed6c5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed6c5-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed6c5-110">Delegated (work or school account)</span></span>|<span data-ttu-id="ed6c5-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed6c5-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="ed6c5-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed6c5-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ed6c5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed6c5-113">Not supported.</span></span>|
|<span data-ttu-id="ed6c5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed6c5-114">Application</span></span>|<span data-ttu-id="ed6c5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed6c5-115">Not supported.</span></span>|

<span data-ttu-id="ed6c5-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="ed6c5-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="ed6c5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed6c5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="ed6c5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed6c5-118">Request headers</span></span>

|<span data-ttu-id="ed6c5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ed6c5-119">Name</span></span>|<span data-ttu-id="ed6c5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed6c5-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ed6c5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed6c5-121">Authorization</span></span>|<span data-ttu-id="ed6c5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed6c5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed6c5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed6c5-124">Request body</span></span>

<span data-ttu-id="ed6c5-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed6c5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed6c5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed6c5-126">Response</span></span>

<span data-ttu-id="ed6c5-127">Se bem-sucedido, esse método retornará `200 OK` código de resposta e um conjunto de [identityProviders](../resources/identityProvider.md) em representação JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed6c5-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityProvider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed6c5-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed6c5-128">Example</span></span>

<span data-ttu-id="ed6c5-129">O exemplo a seguir recupera todos os **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="ed6c5-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="ed6c5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed6c5-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list-identityproviders"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders
```

##### <a name="response"></a><span data-ttu-id="ed6c5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed6c5-131">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ed6c5-132">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="ed6c5-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ed6c5-133">C#</span><span class="sxs-lookup"><span data-stu-id="ed6c5-133">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list-identityproviders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed6c5-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="ed6c5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-identityproviders-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/identityprovider-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/identityprovider-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
