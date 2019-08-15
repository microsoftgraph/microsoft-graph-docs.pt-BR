---
title: Lista identityProviders
description: Recuperar todos os identityProviders no diretório.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 4000be4ce44ed38c40b739313a80ad84aa880feb
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420533"
---
# <a name="list-identityproviders"></a><span data-ttu-id="9e1d7-103">Lista identityProviders</span><span class="sxs-lookup"><span data-stu-id="9e1d7-103">List identityProviders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e1d7-104">Recuperar todos os [identityProviders](../resources/identityprovider.md) no diretório.</span><span class="sxs-lookup"><span data-stu-id="9e1d7-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e1d7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e1d7-105">Permissions</span></span>

<span data-ttu-id="9e1d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e1d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e1d7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e1d7-108">Permission type</span></span>      | <span data-ttu-id="9e1d7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e1d7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e1d7-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e1d7-110">Delegated (work or school account)</span></span>|<span data-ttu-id="9e1d7-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e1d7-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="9e1d7-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e1d7-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9e1d7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e1d7-113">Not supported.</span></span>|
|<span data-ttu-id="9e1d7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e1d7-114">Application</span></span>|<span data-ttu-id="9e1d7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e1d7-115">Not supported.</span></span>|

<span data-ttu-id="9e1d7-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="9e1d7-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="9e1d7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e1d7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="9e1d7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e1d7-118">Request headers</span></span>

|<span data-ttu-id="9e1d7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9e1d7-119">Name</span></span>|<span data-ttu-id="9e1d7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e1d7-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9e1d7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e1d7-121">Authorization</span></span>|<span data-ttu-id="9e1d7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e1d7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e1d7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e1d7-124">Request body</span></span>

<span data-ttu-id="9e1d7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e1d7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e1d7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e1d7-126">Response</span></span>

<span data-ttu-id="9e1d7-127">Se bem-sucedido, esse método retornará `200 OK` código de resposta e um conjunto de [identityProviders](../resources/identityprovider.md) em representação JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e1d7-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e1d7-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e1d7-128">Example</span></span>

<span data-ttu-id="9e1d7-129">O exemplo a seguir recupera todos os **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="9e1d7-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="9e1d7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e1d7-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9e1d7-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e1d7-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9e1d7-132">C#</span><span class="sxs-lookup"><span data-stu-id="9e1d7-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9e1d7-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e1d7-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9e1d7-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9e1d7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9e1d7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e1d7-135">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
