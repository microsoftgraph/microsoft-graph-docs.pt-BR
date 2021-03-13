---
title: Excluir sourceCollection
description: Exclua um objeto sourceCollection.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 13380114c2d2e7a1f0ff4d1f612a411d8efad6f5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772741"
---
# <a name="delete-sourcecollection"></a><span data-ttu-id="57a49-103">Excluir sourceCollection</span><span class="sxs-lookup"><span data-stu-id="57a49-103">Delete sourceCollection</span></span>

<span data-ttu-id="57a49-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="57a49-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57a49-105">Exclua [um objeto sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="57a49-105">Delete a [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="57a49-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="57a49-106">Permissions</span></span>

<span data-ttu-id="57a49-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57a49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57a49-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57a49-109">Permission type</span></span>|<span data-ttu-id="57a49-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57a49-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57a49-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57a49-111">Delegated (work or school account)</span></span>|<span data-ttu-id="57a49-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57a49-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="57a49-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57a49-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57a49-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57a49-114">Not supported.</span></span>|
|<span data-ttu-id="57a49-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57a49-115">Application</span></span>|<span data-ttu-id="57a49-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57a49-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57a49-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57a49-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

## <a name="request-headers"></a><span data-ttu-id="57a49-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57a49-118">Request headers</span></span>

|<span data-ttu-id="57a49-119">Nome</span><span class="sxs-lookup"><span data-stu-id="57a49-119">Name</span></span>|<span data-ttu-id="57a49-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="57a49-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="57a49-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="57a49-121">Authorization</span></span>|<span data-ttu-id="57a49-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57a49-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57a49-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57a49-124">Request body</span></span>

<span data-ttu-id="57a49-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57a49-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57a49-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="57a49-126">Response</span></span>

<span data-ttu-id="57a49-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="57a49-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="57a49-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="57a49-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="57a49-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57a49-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="57a49-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="57a49-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sourcecollection"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```
# <a name="c"></a>[<span data-ttu-id="57a49-131">C#</span><span class="sxs-lookup"><span data-stu-id="57a49-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sourcecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57a49-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57a49-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sourcecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57a49-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57a49-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-sourcecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57a49-134">Java</span><span class="sxs-lookup"><span data-stu-id="57a49-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-sourcecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="57a49-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="57a49-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
