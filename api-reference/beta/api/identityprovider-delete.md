---
title: Excluir identityProvider
description: Excluir um identityprovider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 08e6208cbd58a3101d995d77e7d90b47918fbce5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001684"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="6a580-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="6a580-103">Delete identityProvider</span></span>

<span data-ttu-id="6a580-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a580-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a580-105">Excluir um [identityprovider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="6a580-105">Delete an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6a580-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a580-106">Permissions</span></span>

<span data-ttu-id="6a580-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a580-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a580-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a580-109">Permission type</span></span>      | <span data-ttu-id="6a580-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a580-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a580-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a580-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a580-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a580-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="6a580-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a580-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6a580-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a580-114">Not supported.</span></span>|
|<span data-ttu-id="6a580-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a580-115">Application</span></span>|<span data-ttu-id="6a580-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a580-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="6a580-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="6a580-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="6a580-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="6a580-118">Global administrator</span></span>
* <span data-ttu-id="6a580-119">Administrador do provedor de identidade externa</span><span class="sxs-lookup"><span data-stu-id="6a580-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="6a580-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a580-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6a580-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a580-121">Request headers</span></span>

|<span data-ttu-id="6a580-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6a580-122">Name</span></span>|<span data-ttu-id="6a580-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a580-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="6a580-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a580-124">Authorization</span></span>|<span data-ttu-id="6a580-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a580-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a580-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a580-127">Request body</span></span>

<span data-ttu-id="6a580-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a580-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a580-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a580-129">Response</span></span>

<span data-ttu-id="6a580-130">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6a580-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6a580-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a580-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a580-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a580-132">Request</span></span>

<span data-ttu-id="6a580-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a580-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6a580-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a580-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="6a580-135">C#</span><span class="sxs-lookup"><span data-stu-id="6a580-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a580-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a580-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a580-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a580-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6a580-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a580-138">Response</span></span>

<span data-ttu-id="6a580-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6a580-139">The following is an example of the response.</span></span>

<span data-ttu-id="6a580-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6a580-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


