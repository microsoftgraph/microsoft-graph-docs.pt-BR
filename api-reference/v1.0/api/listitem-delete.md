---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Excluir uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
description: Remove um item de uma lista.
doc_type: apiPageType
ms.openlocfilehash: ac07e03892476ad160f76dd49ced3b2bcb63ace6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373992"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="4e4c3-103">Excluir um item de uma lista.</span><span class="sxs-lookup"><span data-stu-id="4e4c3-103">Delete an item from a list</span></span>

<span data-ttu-id="4e4c3-104">Remover um item de uma [list][].</span><span class="sxs-lookup"><span data-stu-id="4e4c3-104">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="4e4c3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4e4c3-106">Permissions</span></span>

<span data-ttu-id="4e4c3-107">Para excluir um item, o usuário deve ter concedido o acesso de gravação do aplicativo para o item a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="4e4c3-107">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="4e4c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e4c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e4c3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e4c3-110">Permission type</span></span>      | <span data-ttu-id="4e4c3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e4c3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e4c3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e4c3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4e4c3-113">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e4c3-113">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4e4c3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e4c3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e4c3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e4c3-115">Not supported.</span></span>    |
|<span data-ttu-id="4e4c3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e4c3-116">Application</span></span> | <span data-ttu-id="4e4c3-117">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e4c3-117">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e4c3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e4c3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="4e4c3-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="4e4c3-119">Optional request headers</span></span>

| <span data-ttu-id="4e4c3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4e4c3-120">Name</span></span>       | <span data-ttu-id="4e4c3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4e4c3-121">Value</span></span> | <span data-ttu-id="4e4c3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e4c3-122">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="4e4c3-123">_if-match_</span><span class="sxs-lookup"><span data-stu-id="4e4c3-123">_if-match_</span></span> | <span data-ttu-id="4e4c3-124">etag</span><span class="sxs-lookup"><span data-stu-id="4e4c3-124">etag</span></span>  | <span data-ttu-id="4e4c3-125">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="4e4c3-125">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="4e4c3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e4c3-126">Request body</span></span>

<span data-ttu-id="4e4c3-127">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="4e4c3-127">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="4e4c3-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e4c3-128">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4e4c3-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e4c3-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4e4c3-130">C#</span><span class="sxs-lookup"><span data-stu-id="4e4c3-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4e4c3-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e4c3-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4e4c3-132">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4e4c3-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4e4c3-133">Java</span><span class="sxs-lookup"><span data-stu-id="4e4c3-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-item-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="4e4c3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e4c3-134">Response</span></span>

<span data-ttu-id="4e4c3-135">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="4e4c3-135">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": [
  ]
} -->
