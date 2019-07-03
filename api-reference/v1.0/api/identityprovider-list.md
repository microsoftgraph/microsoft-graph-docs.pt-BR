---
title: Lista identityProviders
description: Recuperar todos os identityProviders
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 756578bd61e034972f9b500091ab54c0c7a7dd5f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444643"
---
# <a name="list-identityproviders"></a><span data-ttu-id="d898f-103">Lista identityProviders</span><span class="sxs-lookup"><span data-stu-id="d898f-103">List identityProviders</span></span>

<span data-ttu-id="d898f-104">Recuperar todos os [identityProviders](../resources/identityprovider.md) no diretório.</span><span class="sxs-lookup"><span data-stu-id="d898f-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="d898f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d898f-105">Permissions</span></span>

<span data-ttu-id="d898f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d898f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d898f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d898f-108">Permission type</span></span>      | <span data-ttu-id="d898f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d898f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d898f-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d898f-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d898f-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d898f-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="d898f-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d898f-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d898f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d898f-113">Not supported.</span></span>|
|<span data-ttu-id="d898f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d898f-114">Application</span></span>|<span data-ttu-id="d898f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d898f-115">Not supported.</span></span>|

<span data-ttu-id="d898f-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="d898f-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="d898f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d898f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="d898f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d898f-118">Request headers</span></span>

|<span data-ttu-id="d898f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d898f-119">Name</span></span>|<span data-ttu-id="d898f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d898f-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d898f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d898f-121">Authorization</span></span>|<span data-ttu-id="d898f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d898f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d898f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d898f-124">Request body</span></span>

<span data-ttu-id="d898f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d898f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d898f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d898f-126">Response</span></span>

<span data-ttu-id="d898f-127">Se bem-sucedido, esse método retornará `200 OK` código de resposta e um conjunto de [identityProviders](../resources/identityprovider.md) em representação JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d898f-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d898f-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d898f-128">Example</span></span>

<span data-ttu-id="d898f-129">O exemplo a seguir recupera todos os **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="d898f-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="d898f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d898f-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d898f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d898f-131">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list-identityproviders"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d898f-132">C#</span><span class="sxs-lookup"><span data-stu-id="d898f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d898f-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="d898f-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d898f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d898f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d898f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d898f-135">Response</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
