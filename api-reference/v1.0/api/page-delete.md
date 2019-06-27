---
title: Excluir página
description: Excluir uma página do OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: f8dea5fcd299426545510c6f2d024e51617c243e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274274"
---
# <a name="delete-page"></a><span data-ttu-id="ec40c-103">Excluir página</span><span class="sxs-lookup"><span data-stu-id="ec40c-103">Delete page</span></span>

<span data-ttu-id="ec40c-104">Excluir uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="ec40c-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec40c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec40c-105">Permissions</span></span>
<span data-ttu-id="ec40c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec40c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec40c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec40c-108">Permission type</span></span>      | <span data-ttu-id="ec40c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec40c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec40c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec40c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ec40c-111">Notes. ReadWrite, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ec40c-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ec40c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec40c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec40c-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec40c-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ec40c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec40c-114">Application</span></span> | <span data-ttu-id="ec40c-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec40c-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec40c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec40c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ec40c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec40c-117">Request headers</span></span>
| <span data-ttu-id="ec40c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ec40c-118">Name</span></span>       | <span data-ttu-id="ec40c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec40c-119">Type</span></span> | <span data-ttu-id="ec40c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec40c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ec40c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec40c-121">Authorization</span></span>  | <span data-ttu-id="ec40c-122">string</span><span class="sxs-lookup"><span data-stu-id="ec40c-122">string</span></span>  | <span data-ttu-id="ec40c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec40c-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ec40c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec40c-125">Response</span></span>

<span data-ttu-id="ec40c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec40c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec40c-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec40c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec40c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec40c-129">Request</span></span>
<span data-ttu-id="ec40c-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec40c-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="ec40c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec40c-131">Response</span></span>
<span data-ttu-id="ec40c-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec40c-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ec40c-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ec40c-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ec40c-134">C#</span><span class="sxs-lookup"><span data-stu-id="ec40c-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_page-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ec40c-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="ec40c-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_page-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ec40c-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ec40c-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_page-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/page-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/page-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/page-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
