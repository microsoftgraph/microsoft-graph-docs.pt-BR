---
author: swapnil1993
title: Excluir contentType
description: Exclua um tipo de conteúdo de uma SharePoint ou de um site.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 9597f4b66a070ee40199b39f8accc8b3ab9f5c0e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439359"
---
# <a name="delete-contenttype"></a><span data-ttu-id="975d0-103">Excluir contentType</span><span class="sxs-lookup"><span data-stu-id="975d0-103">Delete contentType</span></span>
<span data-ttu-id="975d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="975d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="975d0-105">Remover um [tipo de conteúdo][contentType] de uma [lista][] ou de um [site][].</span><span class="sxs-lookup"><span data-stu-id="975d0-105">Remove a [content type][contentType] from a [list][] or a [site][].</span></span>


## <a name="permissions"></a><span data-ttu-id="975d0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="975d0-106">Permissions</span></span>
<span data-ttu-id="975d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="975d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="975d0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="975d0-109">Permission type</span></span>      | <span data-ttu-id="975d0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="975d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="975d0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="975d0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="975d0-112">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="975d0-112">Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="975d0-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="975d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="975d0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="975d0-114">Not supported.</span></span>    |
|<span data-ttu-id="975d0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="975d0-115">Application</span></span> | <span data-ttu-id="975d0-116">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="975d0-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="975d0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="975d0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/contentTypes/{contentType-id}
DELETE /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="request-headers"></a><span data-ttu-id="975d0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="975d0-118">Request headers</span></span>
|<span data-ttu-id="975d0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="975d0-119">Name</span></span>|<span data-ttu-id="975d0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="975d0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="975d0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="975d0-121">Authorization</span></span>|<span data-ttu-id="975d0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="975d0-p102">Bearer {token}. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="975d0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="975d0-124">Request body</span></span>

<span data-ttu-id="975d0-125">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="975d0-125">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="975d0-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="975d0-126">Response</span></span>

<span data-ttu-id="975d0-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="975d0-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="975d0-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="975d0-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="975d0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="975d0-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="975d0-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="975d0-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contenttype"
}
-->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
```
# <a name="c"></a>[<span data-ttu-id="975d0-131">C#</span><span class="sxs-lookup"><span data-stu-id="975d0-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="975d0-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="975d0-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="975d0-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="975d0-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="975d0-134">Java</span><span class="sxs-lookup"><span data-stu-id="975d0-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="975d0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="975d0-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
