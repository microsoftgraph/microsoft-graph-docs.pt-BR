---
title: Excluir userSource
description: Exclui um objeto userSource.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 631d547aefec38258d69ccb48d325fc955e65a57
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873028"
---
# <a name="delete-usersource"></a><span data-ttu-id="95009-103">Excluir userSource</span><span class="sxs-lookup"><span data-stu-id="95009-103">Delete userSource</span></span>

<span data-ttu-id="95009-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95009-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95009-105">[Exclua um objeto userSource.](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="95009-105">Delete a [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="95009-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="95009-106">Permissions</span></span>

<span data-ttu-id="95009-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95009-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95009-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95009-109">Permission type</span></span>|<span data-ttu-id="95009-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95009-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95009-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95009-111">Delegated (work or school account)</span></span>|<span data-ttu-id="95009-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="95009-112">User.Read</span></span>|
|<span data-ttu-id="95009-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95009-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95009-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95009-114">Not supported.</span></span>|
|<span data-ttu-id="95009-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95009-115">Application</span></span>|<span data-ttu-id="95009-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95009-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95009-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95009-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources/{userSourceId}
```

## <a name="request-headers"></a><span data-ttu-id="95009-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95009-118">Request headers</span></span>

|<span data-ttu-id="95009-119">Nome</span><span class="sxs-lookup"><span data-stu-id="95009-119">Name</span></span>|<span data-ttu-id="95009-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="95009-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="95009-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="95009-121">Authorization</span></span>|<span data-ttu-id="95009-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95009-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="95009-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95009-124">Request body</span></span>

<span data-ttu-id="95009-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95009-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95009-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="95009-126">Response</span></span>

<span data-ttu-id="95009-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="95009-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="95009-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="95009-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="95009-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95009-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="95009-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="95009-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_usersource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735
```
# <a name="c"></a>[<span data-ttu-id="95009-131">C#</span><span class="sxs-lookup"><span data-stu-id="95009-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-usersource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95009-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95009-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-usersource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95009-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95009-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-usersource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="95009-134">Java</span><span class="sxs-lookup"><span data-stu-id="95009-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-usersource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="95009-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="95009-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
