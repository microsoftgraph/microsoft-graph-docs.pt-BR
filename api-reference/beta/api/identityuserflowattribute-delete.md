---
title: Excluir identityUserFlowAttribute
description: Excluir um identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 32758c748e532d7a8b778a5e19437f1bb6ae8c84
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953205"
---
# <a name="delete-identityuserflowattribute"></a><span data-ttu-id="c8117-103">Excluir identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="c8117-103">Delete identityUserFlowAttribute</span></span>

<span data-ttu-id="c8117-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8117-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8117-105">Excluir um [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="c8117-105">Delete an [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="c8117-106">Somente atributos de fluxo de usuário personalizados podem ser excluídos.</span><span class="sxs-lookup"><span data-stu-id="c8117-106">Only custom user flow attributes can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8117-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c8117-107">Permissions</span></span>

<span data-ttu-id="c8117-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8117-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8117-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8117-110">Permission type</span></span>      | <span data-ttu-id="c8117-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8117-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8117-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8117-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8117-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8117-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c8117-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8117-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c8117-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8117-115">Not supported.</span></span>|
|<span data-ttu-id="c8117-116">Application</span><span class="sxs-lookup"><span data-stu-id="c8117-116">Application</span></span>|<span data-ttu-id="c8117-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8117-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c8117-118">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="c8117-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c8117-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c8117-119">Global administrator</span></span>
* <span data-ttu-id="c8117-120">Administrador do atributo de fluxo do usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="c8117-120">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c8117-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8117-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c8117-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8117-122">Request headers</span></span>

|<span data-ttu-id="c8117-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c8117-123">Name</span></span>|<span data-ttu-id="c8117-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8117-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c8117-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8117-125">Authorization</span></span>|<span data-ttu-id="c8117-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8117-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8117-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8117-128">Request body</span></span>

<span data-ttu-id="c8117-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8117-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8117-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8117-130">Response</span></span>

<span data-ttu-id="c8117-131">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c8117-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c8117-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8117-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8117-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8117-133">Request</span></span>

<span data-ttu-id="c8117-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8117-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c8117-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8117-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userFlowAttributes"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/userFlowAttributes/{id}
```
# <a name="c"></a>[<span data-ttu-id="c8117-136">C#</span><span class="sxs-lookup"><span data-stu-id="c8117-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8117-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8117-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8117-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8117-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8117-139">Java</span><span class="sxs-lookup"><span data-stu-id="c8117-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c8117-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8117-140">Response</span></span>

<span data-ttu-id="c8117-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c8117-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
