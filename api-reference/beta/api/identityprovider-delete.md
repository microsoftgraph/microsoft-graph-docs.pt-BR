---
title: Excluir identityProvider
description: Excluir o identityProvider existente.
localization_priority: Normal
doc_type: apiPageType
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8d63e828ac78ce376c78a484402f44e7584bc331
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446503"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="1399c-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="1399c-103">Delete identityProvider</span></span>

<span data-ttu-id="1399c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1399c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1399c-105">Excluir o [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="1399c-105">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1399c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1399c-106">Permissions</span></span>

<span data-ttu-id="1399c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1399c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1399c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1399c-109">Permission type</span></span>      | <span data-ttu-id="1399c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1399c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1399c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1399c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1399c-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1399c-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="1399c-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1399c-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1399c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1399c-114">Not supported.</span></span>|
|<span data-ttu-id="1399c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1399c-115">Application</span></span>|<span data-ttu-id="1399c-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1399c-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="1399c-117">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="1399c-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="1399c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1399c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1399c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1399c-119">Request headers</span></span>

|<span data-ttu-id="1399c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1399c-120">Name</span></span>|<span data-ttu-id="1399c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1399c-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1399c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1399c-122">Authorization</span></span>|<span data-ttu-id="1399c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1399c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1399c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1399c-125">Request body</span></span>

<span data-ttu-id="1399c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1399c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1399c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1399c-127">Response</span></span>

<span data-ttu-id="1399c-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1399c-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1399c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1399c-129">Example</span></span>

<span data-ttu-id="1399c-130">O exemplo a seguir exclui um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="1399c-130">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="1399c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1399c-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1399c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1399c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```
# <a name="c"></a>[<span data-ttu-id="1399c-133">C#</span><span class="sxs-lookup"><span data-stu-id="1399c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1399c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1399c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1399c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1399c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1399c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1399c-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
