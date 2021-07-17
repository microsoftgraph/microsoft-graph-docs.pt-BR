---
author: swapnil1993
title: 'contentType: publish'
description: Publique um tipo de conteúdo presente no site do hub de tipo de conteúdo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: d69cbdabbb82612945dc6df85617e50bc2ca5b2c
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467082"
---
# <a name="contenttype-publish"></a><span data-ttu-id="bedd6-103">contentType: publish</span><span class="sxs-lookup"><span data-stu-id="bedd6-103">contentType: publish</span></span>
<span data-ttu-id="bedd6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bedd6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="bedd6-105">Publica um [contentType][] presente em um site de hub de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="bedd6-105">Publishes a [contentType][] present in a content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="bedd6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bedd6-106">Permissions</span></span>

<span data-ttu-id="bedd6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bedd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="bedd6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bedd6-109">Permission type</span></span>      | <span data-ttu-id="bedd6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bedd6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bedd6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bedd6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bedd6-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="bedd6-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="bedd6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bedd6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bedd6-114">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="bedd6-114">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="bedd6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bedd6-115">Application</span></span> | <span data-ttu-id="bedd6-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="bedd6-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bedd6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bedd6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/publish
```

><span data-ttu-id="bedd6-118">**Observação:** `siteId` representa um site de hub de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="bedd6-118">**Note:** `siteId` represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bedd6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bedd6-119">Request headers</span></span>
|<span data-ttu-id="bedd6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bedd6-120">Name</span></span>|<span data-ttu-id="bedd6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bedd6-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bedd6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bedd6-122">Authorization</span></span>|<span data-ttu-id="bedd6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bedd6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bedd6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bedd6-125">Request body</span></span>
<span data-ttu-id="bedd6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bedd6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bedd6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bedd6-127">Response</span></span>
<span data-ttu-id="bedd6-128">Se tiver êxito, essa chamada retornará uma `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="bedd6-128">If successful, this call returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="bedd6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bedd6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="bedd6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bedd6-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bedd6-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="bedd6-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_publish"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/publish
```
# <a name="c"></a>[<span data-ttu-id="bedd6-132">C#</span><span class="sxs-lookup"><span data-stu-id="bedd6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bedd6-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bedd6-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bedd6-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bedd6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bedd6-135">Java</span><span class="sxs-lookup"><span data-stu-id="bedd6-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-publish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bedd6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bedd6-136">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[contentType]: ../resources/contentType.md
