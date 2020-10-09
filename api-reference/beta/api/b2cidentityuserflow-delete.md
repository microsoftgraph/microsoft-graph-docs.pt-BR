---
title: Excluir b2cIdentityUserFlow
description: Excluir um objeto b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 45a3ae34057ca5d88219c9f929bc33ce081c24b9
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406250"
---
# <a name="delete-b2cidentityuserflow"></a><span data-ttu-id="362fe-103">Excluir b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="362fe-103">Delete b2cIdentityUserFlow</span></span>

<span data-ttu-id="362fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="362fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="362fe-105">Excluir um objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="362fe-105">Delete a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="362fe-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="362fe-106">Permissions</span></span>

<span data-ttu-id="362fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="362fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="362fe-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="362fe-109">Permission type</span></span>      | <span data-ttu-id="362fe-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="362fe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="362fe-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="362fe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="362fe-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="362fe-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="362fe-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="362fe-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="362fe-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="362fe-114">Not supported.</span></span>|
|<span data-ttu-id="362fe-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="362fe-115">Application</span></span>|<span data-ttu-id="362fe-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="362fe-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="362fe-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="362fe-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="362fe-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="362fe-118">Global administrator</span></span>
* <span data-ttu-id="362fe-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="362fe-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="362fe-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="362fe-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="362fe-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="362fe-121">Request headers</span></span>

|<span data-ttu-id="362fe-122">Nome</span><span class="sxs-lookup"><span data-stu-id="362fe-122">Name</span></span>|<span data-ttu-id="362fe-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="362fe-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="362fe-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="362fe-124">Authorization</span></span>|<span data-ttu-id="362fe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="362fe-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="362fe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="362fe-127">Request body</span></span>

<span data-ttu-id="362fe-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="362fe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="362fe-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="362fe-129">Response</span></span>

<span data-ttu-id="362fe-130">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="362fe-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="362fe-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="362fe-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="362fe-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="362fe-132">Request</span></span>

<span data-ttu-id="362fe-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="362fe-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="362fe-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="362fe-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2cUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="362fe-135">C#</span><span class="sxs-lookup"><span data-stu-id="362fe-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="362fe-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="362fe-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="362fe-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="362fe-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="362fe-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="362fe-138">Response</span></span>

<span data-ttu-id="362fe-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="362fe-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


