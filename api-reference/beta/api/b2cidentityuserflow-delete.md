---
title: Excluir b2cIdentityUserFlow
description: Exclua um objeto b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 11ea70b285f20e281d342e808ad1a15b98041572
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438348"
---
# <a name="delete-b2cidentityuserflow"></a><span data-ttu-id="3baa9-103">Excluir b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3baa9-103">Delete b2cIdentityUserFlow</span></span>

<span data-ttu-id="3baa9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3baa9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3baa9-105">[Exclua um objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="3baa9-105">Delete a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3baa9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3baa9-106">Permissions</span></span>

<span data-ttu-id="3baa9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3baa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3baa9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3baa9-109">Permission type</span></span>      | <span data-ttu-id="3baa9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3baa9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3baa9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3baa9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3baa9-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3baa9-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3baa9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3baa9-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3baa9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3baa9-114">Not supported.</span></span>|
|<span data-ttu-id="3baa9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3baa9-115">Application</span></span>|<span data-ttu-id="3baa9-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3baa9-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="3baa9-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="3baa9-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="3baa9-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="3baa9-118">Global administrator</span></span>
* <span data-ttu-id="3baa9-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="3baa9-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3baa9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3baa9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3baa9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3baa9-121">Request headers</span></span>

|<span data-ttu-id="3baa9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3baa9-122">Name</span></span>|<span data-ttu-id="3baa9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3baa9-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3baa9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3baa9-124">Authorization</span></span>|<span data-ttu-id="3baa9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3baa9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3baa9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3baa9-127">Request body</span></span>

<span data-ttu-id="3baa9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3baa9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3baa9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3baa9-129">Response</span></span>

<span data-ttu-id="3baa9-130">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3baa9-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3baa9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3baa9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3baa9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3baa9-132">Request</span></span>

<span data-ttu-id="3baa9-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3baa9-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3baa9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3baa9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2cUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="3baa9-135">C#</span><span class="sxs-lookup"><span data-stu-id="3baa9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3baa9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3baa9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3baa9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3baa9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3baa9-138">Java</span><span class="sxs-lookup"><span data-stu-id="3baa9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3baa9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3baa9-139">Response</span></span>

<span data-ttu-id="3baa9-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3baa9-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


