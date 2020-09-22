---
title: Excluir b2cUserFlow
description: Excluir um objeto b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 26e4b244128a8dbd61179197d82d9d83a920b91f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991499"
---
# <a name="delete-b2cuserflow"></a><span data-ttu-id="25990-103">Excluir b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="25990-103">Delete b2cUserFlow</span></span>

<span data-ttu-id="25990-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25990-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25990-105">Excluir um objeto [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="25990-105">Delete a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="25990-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="25990-106">Permissions</span></span>

<span data-ttu-id="25990-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25990-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25990-109">Permission type</span></span>      | <span data-ttu-id="25990-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25990-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25990-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25990-111">Delegated (work or school account)</span></span>|<span data-ttu-id="25990-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="25990-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="25990-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25990-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="25990-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25990-114">Not supported.</span></span>|
|<span data-ttu-id="25990-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25990-115">Application</span></span>|<span data-ttu-id="25990-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="25990-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="25990-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="25990-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="25990-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="25990-118">Global administrator</span></span>
* <span data-ttu-id="25990-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="25990-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="25990-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25990-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="25990-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25990-121">Request headers</span></span>

|<span data-ttu-id="25990-122">Nome</span><span class="sxs-lookup"><span data-stu-id="25990-122">Name</span></span>|<span data-ttu-id="25990-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="25990-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="25990-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="25990-124">Authorization</span></span>|<span data-ttu-id="25990-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25990-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="25990-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25990-127">Request body</span></span>

<span data-ttu-id="25990-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25990-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25990-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="25990-129">Response</span></span>

<span data-ttu-id="25990-130">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="25990-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="25990-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25990-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="25990-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25990-132">Request</span></span>

<span data-ttu-id="25990-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="25990-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="25990-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="25990-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2cUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="25990-135">C#</span><span class="sxs-lookup"><span data-stu-id="25990-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25990-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25990-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25990-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25990-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="25990-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="25990-138">Response</span></span>

<span data-ttu-id="25990-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="25990-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


