---
author: swapnil1993
title: 'contentType: unpublish'
description: Não publice um tipo de conteúdo de um site de hub de tipo de conteúdo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8b7e8c63c6d92390731b670f8d95821fe5334b0d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773379"
---
# <a name="contenttype-unpublish"></a><span data-ttu-id="7b71c-103">contentType: unpublish</span><span class="sxs-lookup"><span data-stu-id="7b71c-103">contentType: unpublish</span></span>
<span data-ttu-id="7b71c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b71c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="7b71c-105">Não publice um [contentType de][] um site de hub de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7b71c-105">Unpublish a [contentType][] from a content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b71c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7b71c-106">Permissions</span></span>

<span data-ttu-id="7b71c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b71c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="7b71c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b71c-109">Permission type</span></span>      | <span data-ttu-id="7b71c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b71c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b71c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b71c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7b71c-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7b71c-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="7b71c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b71c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b71c-114">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7b71c-114">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="7b71c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b71c-115">Application</span></span> | <span data-ttu-id="7b71c-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7b71c-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b71c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b71c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/unpublish
```

><span data-ttu-id="7b71c-118">**Observação:** O siteId representa um site de hub de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7b71c-118">**Note:** The siteId represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b71c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b71c-119">Request headers</span></span>
|<span data-ttu-id="7b71c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7b71c-120">Name</span></span>|<span data-ttu-id="7b71c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b71c-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7b71c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b71c-122">Authorization</span></span>|<span data-ttu-id="7b71c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b71c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b71c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b71c-125">Request body</span></span>
<span data-ttu-id="7b71c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b71c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b71c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b71c-127">Response</span></span>

<span data-ttu-id="7b71c-128">Se tiver êxito, este método retornará uma `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="7b71c-128">If successful, this method returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="7b71c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b71c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b71c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b71c-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7b71c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b71c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_unpublish"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/unpublish
```
# <a name="c"></a>[<span data-ttu-id="7b71c-132">C#</span><span class="sxs-lookup"><span data-stu-id="7b71c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-unpublish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b71c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b71c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-unpublish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b71c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b71c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-unpublish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b71c-135">Java</span><span class="sxs-lookup"><span data-stu-id="7b71c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-unpublish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7b71c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b71c-136">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[contentType]: ../resources/contentType.md
