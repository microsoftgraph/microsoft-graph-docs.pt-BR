---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Excluir uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 727c7be2303fc31a72f24e407cf9a6dd58a748cd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446210"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="fdee9-102">Excluir um item de uma lista.</span><span class="sxs-lookup"><span data-stu-id="fdee9-102">Delete an item from a list</span></span>

<span data-ttu-id="fdee9-103">Remover um item de uma [list][].</span><span class="sxs-lookup"><span data-stu-id="fdee9-103">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="fdee9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdee9-105">Permissions</span></span>

<span data-ttu-id="fdee9-106">Para excluir um item, o usuário deve ter concedido o acesso de gravação do aplicativo para o item a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="fdee9-106">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="fdee9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdee9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdee9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdee9-109">Permission type</span></span>      | <span data-ttu-id="fdee9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdee9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdee9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdee9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fdee9-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdee9-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fdee9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdee9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdee9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdee9-114">Not supported.</span></span>    |
|<span data-ttu-id="fdee9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdee9-115">Application</span></span> | <span data-ttu-id="fdee9-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdee9-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdee9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdee9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="fdee9-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="fdee9-118">Optional request headers</span></span>

| <span data-ttu-id="fdee9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fdee9-119">Name</span></span>       | <span data-ttu-id="fdee9-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fdee9-120">Value</span></span> | <span data-ttu-id="fdee9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdee9-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="fdee9-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="fdee9-122">_if-match_</span></span> | <span data-ttu-id="fdee9-123">etag</span><span class="sxs-lookup"><span data-stu-id="fdee9-123">etag</span></span>  | <span data-ttu-id="fdee9-124">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="fdee9-124">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="fdee9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdee9-125">Request body</span></span>

<span data-ttu-id="fdee9-126">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="fdee9-126">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="fdee9-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdee9-127">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fdee9-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="fdee9-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fdee9-129">C#</span><span class="sxs-lookup"><span data-stu-id="fdee9-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fdee9-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="fdee9-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fdee9-131">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fdee9-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="fdee9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdee9-132">Response</span></span>

<span data-ttu-id="fdee9-133">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="fdee9-133">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
