---
title: Lista identityProviders
description: Recuperar todos os identityProviders no diretório.
localization_priority: Normal
doc_type: apiPageType
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a2c6279a6d5c3511d6b6786f3d561d0632933e66
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199547"
---
# <a name="list-identityproviders"></a><span data-ttu-id="b33c5-103">Lista identityProviders</span><span class="sxs-lookup"><span data-stu-id="b33c5-103">List identityProviders</span></span>

<span data-ttu-id="b33c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b33c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b33c5-105">Recuperar todos os [identityProviders](../resources/identityprovider.md) no diretório.</span><span class="sxs-lookup"><span data-stu-id="b33c5-105">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="b33c5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b33c5-106">Permissions</span></span>

<span data-ttu-id="b33c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b33c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b33c5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b33c5-109">Permission type</span></span>      | <span data-ttu-id="b33c5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b33c5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b33c5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b33c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b33c5-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b33c5-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="b33c5-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b33c5-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b33c5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b33c5-114">Not supported.</span></span>|
|<span data-ttu-id="b33c5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b33c5-115">Application</span></span>|<span data-ttu-id="b33c5-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b33c5-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="b33c5-117">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="b33c5-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="b33c5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b33c5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="b33c5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b33c5-119">Request headers</span></span>

|<span data-ttu-id="b33c5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b33c5-120">Name</span></span>|<span data-ttu-id="b33c5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b33c5-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b33c5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b33c5-122">Authorization</span></span>|<span data-ttu-id="b33c5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b33c5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b33c5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b33c5-125">Request body</span></span>

<span data-ttu-id="b33c5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b33c5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b33c5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b33c5-127">Response</span></span>

<span data-ttu-id="b33c5-128">Se bem-sucedido, esse método retornará `200 OK` código de resposta e um conjunto de [identityProviders](../resources/identityprovider.md) em representação JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b33c5-128">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b33c5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b33c5-129">Example</span></span>

<span data-ttu-id="b33c5-130">O exemplo a seguir recupera todos os **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="b33c5-130">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="b33c5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b33c5-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b33c5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b33c5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="b33c5-133">C#</span><span class="sxs-lookup"><span data-stu-id="b33c5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b33c5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b33c5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b33c5-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b33c5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b33c5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b33c5-136">Response</span></span>

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
