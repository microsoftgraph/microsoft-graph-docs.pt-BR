---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Excluir uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
description: Remove um item de uma lista.
doc_type: apiPageType
ms.openlocfilehash: f62360dec348e80cc2f54bc2d06afdc20abf19c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511709"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="0461c-103">Excluir um item de uma lista.</span><span class="sxs-lookup"><span data-stu-id="0461c-103">Delete an item from a list</span></span>

<span data-ttu-id="0461c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0461c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0461c-105">Remover um item de uma [list][].</span><span class="sxs-lookup"><span data-stu-id="0461c-105">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="0461c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0461c-107">Permissions</span></span>

<span data-ttu-id="0461c-108">Para excluir um item, o usuário deve ter concedido o acesso de gravação do aplicativo para o item a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="0461c-108">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="0461c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0461c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0461c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0461c-111">Permission type</span></span>      | <span data-ttu-id="0461c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0461c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0461c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0461c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0461c-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0461c-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0461c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0461c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0461c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0461c-116">Not supported.</span></span>    |
|<span data-ttu-id="0461c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0461c-117">Application</span></span> | <span data-ttu-id="0461c-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0461c-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0461c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0461c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="0461c-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="0461c-120">Optional request headers</span></span>

| <span data-ttu-id="0461c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0461c-121">Name</span></span>       | <span data-ttu-id="0461c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0461c-122">Value</span></span> | <span data-ttu-id="0461c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0461c-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="0461c-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="0461c-124">_if-match_</span></span> | <span data-ttu-id="0461c-125">etag</span><span class="sxs-lookup"><span data-stu-id="0461c-125">etag</span></span>  | <span data-ttu-id="0461c-126">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="0461c-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="0461c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0461c-127">Request body</span></span>

<span data-ttu-id="0461c-128">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="0461c-128">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="0461c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0461c-129">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="0461c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0461c-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="c"></a>[<span data-ttu-id="0461c-131">C#</span><span class="sxs-lookup"><span data-stu-id="0461c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0461c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0461c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0461c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0461c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0461c-134">Java</span><span class="sxs-lookup"><span data-stu-id="0461c-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-item-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="0461c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0461c-135">Response</span></span>

<span data-ttu-id="0461c-136">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="0461c-136">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
