---
title: Excluir b2cIdentityUserFlow
description: Excluir um objeto b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 231166675c25f908c4afe5a74bd5ff7803ebd820
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961229"
---
# <a name="delete-b2cidentityuserflow"></a><span data-ttu-id="c5320-103">Excluir b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="c5320-103">Delete b2cIdentityUserFlow</span></span>

<span data-ttu-id="c5320-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5320-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5320-105">Excluir um objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="c5320-105">Delete a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5320-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5320-106">Permissions</span></span>

<span data-ttu-id="c5320-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5320-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5320-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5320-109">Permission type</span></span>      | <span data-ttu-id="c5320-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5320-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5320-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5320-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c5320-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5320-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c5320-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5320-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c5320-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5320-114">Not supported.</span></span>|
|<span data-ttu-id="c5320-115">Application</span><span class="sxs-lookup"><span data-stu-id="c5320-115">Application</span></span>|<span data-ttu-id="c5320-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5320-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c5320-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="c5320-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c5320-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c5320-118">Global administrator</span></span>
* <span data-ttu-id="c5320-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="c5320-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c5320-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5320-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c5320-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5320-121">Request headers</span></span>

|<span data-ttu-id="c5320-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c5320-122">Name</span></span>|<span data-ttu-id="c5320-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5320-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c5320-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5320-124">Authorization</span></span>|<span data-ttu-id="c5320-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5320-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5320-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5320-127">Request body</span></span>

<span data-ttu-id="c5320-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5320-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5320-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5320-129">Response</span></span>

<span data-ttu-id="c5320-130">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c5320-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c5320-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5320-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5320-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5320-132">Request</span></span>

<span data-ttu-id="c5320-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5320-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c5320-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5320-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2cUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="c5320-135">C#</span><span class="sxs-lookup"><span data-stu-id="c5320-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5320-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5320-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5320-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5320-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5320-138">Java</span><span class="sxs-lookup"><span data-stu-id="c5320-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c5320-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5320-139">Response</span></span>

<span data-ttu-id="c5320-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5320-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


