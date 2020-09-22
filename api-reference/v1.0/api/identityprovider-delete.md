---
title: Excluir identityProvider
description: Excluir um identityProvider existente.
localization_priority: Priority
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7765b69536699e969fb721cc3dc7e65ff313ce77
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973201"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="d5c68-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="d5c68-103">Delete identityProvider</span></span>

<span data-ttu-id="d5c68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5c68-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5c68-105">Excluir o [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="d5c68-105">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5c68-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5c68-106">Permissions</span></span>

<span data-ttu-id="d5c68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5c68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5c68-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5c68-109">Permission type</span></span>      | <span data-ttu-id="d5c68-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5c68-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5c68-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5c68-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d5c68-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5c68-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="d5c68-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5c68-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d5c68-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5c68-114">Not supported.</span></span>|
|<span data-ttu-id="d5c68-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5c68-115">Application</span></span>|<span data-ttu-id="d5c68-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5c68-116">Not supported.</span></span>|

<span data-ttu-id="d5c68-117">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="d5c68-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="d5c68-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5c68-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d5c68-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c68-119">Request headers</span></span>

|<span data-ttu-id="d5c68-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d5c68-120">Name</span></span>|<span data-ttu-id="d5c68-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5c68-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d5c68-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5c68-122">Authorization</span></span>|<span data-ttu-id="d5c68-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5c68-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5c68-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c68-125">Request body</span></span>

<span data-ttu-id="d5c68-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d5c68-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5c68-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5c68-127">Response</span></span>

<span data-ttu-id="d5c68-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d5c68-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d5c68-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5c68-129">Example</span></span>

<span data-ttu-id="d5c68-130">O exemplo a seguir exclui um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="d5c68-130">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="d5c68-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c68-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d5c68-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5c68-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```
# <a name="c"></a>[<span data-ttu-id="d5c68-133">C#</span><span class="sxs-lookup"><span data-stu-id="d5c68-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5c68-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5c68-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5c68-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5c68-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5c68-136">Java</span><span class="sxs-lookup"><span data-stu-id="d5c68-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d5c68-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5c68-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

