---
author: swapnil1993
title: 'contentType: isPublished'
description: Verifique o status de publicação de um tipo de conteúdo em um site de hub de tipo de conteúdo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 150caec3be0740d82563e280e6425d0d3b827ecd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770565"
---
# <a name="contenttype-ispublished"></a><span data-ttu-id="478ff-103">contentType: isPublished</span><span class="sxs-lookup"><span data-stu-id="478ff-103">contentType: isPublished</span></span>
<span data-ttu-id="478ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="478ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="478ff-105">Verifique o status de publicação de um [contentType][] em um site de hub de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="478ff-105">Check the publishing status of a [contentType][] in a content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="478ff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="478ff-106">Permissions</span></span>

<span data-ttu-id="478ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="478ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="478ff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="478ff-109">Permission type</span></span>      | <span data-ttu-id="478ff-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="478ff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="478ff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="478ff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="478ff-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="478ff-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="478ff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="478ff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="478ff-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="478ff-114">Not Supported</span></span>   |
|<span data-ttu-id="478ff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="478ff-115">Application</span></span> | <span data-ttu-id="478ff-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="478ff-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="478ff-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="478ff-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
><span data-ttu-id="478ff-118">**Observação:** O siteId representa um site de hub de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="478ff-118">**Note:** The siteId represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="478ff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="478ff-119">Request headers</span></span>
|<span data-ttu-id="478ff-120">Nome</span><span class="sxs-lookup"><span data-stu-id="478ff-120">Name</span></span>|<span data-ttu-id="478ff-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="478ff-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="478ff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="478ff-122">Authorization</span></span>|<span data-ttu-id="478ff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="478ff-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="478ff-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="478ff-125">Response</span></span>
<span data-ttu-id="478ff-126">Se tiver êxito, essa chamada retornará uma resposta e um valor booleano especificando o estado `200 OK` de publicação do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="478ff-126">If successful, this call returns a `200 OK` response and a boolean value specifying the publishing state of the content type.</span></span>

## <a name="request-body"></a><span data-ttu-id="478ff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="478ff-127">Request body</span></span>
<span data-ttu-id="478ff-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="478ff-128">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="478ff-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="478ff-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="478ff-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="478ff-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="478ff-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="478ff-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_ispublished"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
# <a name="c"></a>[<span data-ttu-id="478ff-132">C#</span><span class="sxs-lookup"><span data-stu-id="478ff-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-ispublished-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="478ff-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="478ff-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-ispublished-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="478ff-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="478ff-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-ispublished-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="478ff-135">Java</span><span class="sxs-lookup"><span data-stu-id="478ff-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-ispublished-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="478ff-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="478ff-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": true 
}
```

[contentType]: ../resources/contentType.md
