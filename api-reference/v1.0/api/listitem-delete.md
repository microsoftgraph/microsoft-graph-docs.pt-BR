---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Excluir uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 80ecd3a9079e52ee9908f0211d0e283d993869b2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612962"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="cc7a4-102">Excluir um item de uma lista.</span><span class="sxs-lookup"><span data-stu-id="cc7a4-102">Delete an item from a list</span></span>

<span data-ttu-id="cc7a4-103">Remover um item de uma [list][].</span><span class="sxs-lookup"><span data-stu-id="cc7a4-103">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="cc7a4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc7a4-105">Permissions</span></span>

<span data-ttu-id="cc7a4-106">Para excluir um item, o usuário deve ter concedido o acesso de gravação do aplicativo para o item a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="cc7a4-106">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="cc7a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc7a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc7a4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc7a4-109">Permission type</span></span>      | <span data-ttu-id="cc7a4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc7a4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc7a4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc7a4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cc7a4-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc7a4-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc7a4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc7a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc7a4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc7a4-114">Not supported.</span></span>    |
|<span data-ttu-id="cc7a4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc7a4-115">Application</span></span> | <span data-ttu-id="cc7a4-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc7a4-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc7a4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc7a4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="cc7a4-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="cc7a4-118">Optional request headers</span></span>

| <span data-ttu-id="cc7a4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cc7a4-119">Name</span></span>       | <span data-ttu-id="cc7a4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cc7a4-120">Value</span></span> | <span data-ttu-id="cc7a4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc7a4-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="cc7a4-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="cc7a4-122">_if-match_</span></span> | <span data-ttu-id="cc7a4-123">etag</span><span class="sxs-lookup"><span data-stu-id="cc7a4-123">etag</span></span>  | <span data-ttu-id="cc7a4-124">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="cc7a4-124">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="cc7a4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc7a4-125">Request body</span></span>

<span data-ttu-id="cc7a4-126">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="cc7a4-126">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="cc7a4-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc7a4-127">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="cc7a4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc7a4-128">Response</span></span>

<span data-ttu-id="cc7a4-129">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="cc7a4-129">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cc7a4-130">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="cc7a4-130">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cc7a4-131">C#</span><span class="sxs-lookup"><span data-stu-id="cc7a4-131">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete-item-site-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc7a4-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="cc7a4-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete-item-site-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
