---
title: Excluir b2xIdentityUserFlow
description: Exclua um objeto b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: e9a5b0b0ff28c452bbb74e14d9efbf55949a5a65
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438166"
---
# <a name="delete-b2xidentityuserflow"></a><span data-ttu-id="41772-103">Excluir b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="41772-103">Delete b2xIdentityUserFlow</span></span>

<span data-ttu-id="41772-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41772-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41772-105">[Exclua um objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="41772-105">Delete a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="41772-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="41772-106">Permissions</span></span>

<span data-ttu-id="41772-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41772-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41772-109">Permission type</span></span>      | <span data-ttu-id="41772-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41772-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41772-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41772-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41772-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41772-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="41772-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41772-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="41772-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41772-114">Not supported.</span></span>|
|<span data-ttu-id="41772-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41772-115">Application</span></span>|<span data-ttu-id="41772-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41772-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="41772-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="41772-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="41772-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="41772-118">Global administrator</span></span>
* <span data-ttu-id="41772-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="41772-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="41772-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41772-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2xUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="41772-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41772-121">Request headers</span></span>

|<span data-ttu-id="41772-122">Nome</span><span class="sxs-lookup"><span data-stu-id="41772-122">Name</span></span>|<span data-ttu-id="41772-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="41772-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="41772-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="41772-124">Authorization</span></span>|<span data-ttu-id="41772-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41772-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="41772-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41772-127">Request body</span></span>

<span data-ttu-id="41772-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41772-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41772-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="41772-129">Response</span></span>

<span data-ttu-id="41772-130">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="41772-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="41772-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41772-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="41772-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41772-132">Request</span></span>

<span data-ttu-id="41772-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41772-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="41772-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="41772-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="41772-135">C#</span><span class="sxs-lookup"><span data-stu-id="41772-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41772-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41772-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41772-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41772-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41772-138">Java</span><span class="sxs-lookup"><span data-stu-id="41772-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="41772-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="41772-139">Response</span></span>

<span data-ttu-id="41772-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41772-140">The following is an example of the response.</span></span>

<span data-ttu-id="41772-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="41772-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


