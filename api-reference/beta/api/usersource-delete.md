---
title: Excluir usuário
description: Exclui um objeto username.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 2796137b1c0d045e81b9b1f4a052881f3541f4bf
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657197"
---
# <a name="delete-usersource"></a><span data-ttu-id="fb5d7-103">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="fb5d7-103">Delete userSource</span></span>

<span data-ttu-id="fb5d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb5d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb5d7-105">Excluir um objeto [username](../resources/usersource.md) .</span><span class="sxs-lookup"><span data-stu-id="fb5d7-105">Delete a [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb5d7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb5d7-106">Permissions</span></span>

<span data-ttu-id="fb5d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb5d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb5d7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb5d7-109">Permission type</span></span>|<span data-ttu-id="fb5d7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb5d7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb5d7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb5d7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb5d7-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="fb5d7-112">User.Read</span></span>|
|<span data-ttu-id="fb5d7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb5d7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb5d7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb5d7-114">Not supported.</span></span>|
|<span data-ttu-id="fb5d7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb5d7-115">Application</span></span>|<span data-ttu-id="fb5d7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb5d7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb5d7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb5d7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources/{userSourceId}
```

## <a name="request-headers"></a><span data-ttu-id="fb5d7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb5d7-118">Request headers</span></span>

|<span data-ttu-id="fb5d7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fb5d7-119">Name</span></span>|<span data-ttu-id="fb5d7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb5d7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fb5d7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb5d7-121">Authorization</span></span>|<span data-ttu-id="fb5d7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb5d7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb5d7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb5d7-124">Request body</span></span>

<span data-ttu-id="fb5d7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb5d7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb5d7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb5d7-126">Response</span></span>

<span data-ttu-id="fb5d7-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fb5d7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fb5d7-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fb5d7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb5d7-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb5d7-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fb5d7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb5d7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_usersource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735
```
# <a name="c"></a>[<span data-ttu-id="fb5d7-131">C#</span><span class="sxs-lookup"><span data-stu-id="fb5d7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-usersource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb5d7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb5d7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-usersource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb5d7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb5d7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-usersource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb5d7-134">Java</span><span class="sxs-lookup"><span data-stu-id="fb5d7-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-usersource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fb5d7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb5d7-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
