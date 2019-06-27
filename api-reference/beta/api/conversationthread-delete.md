---
title: Excluir conversationThread
description: Exclua um conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7709728b64772450540f04d9780aff523f1bc64e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261093"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="63bed-103">Excluir conversationThread</span><span class="sxs-lookup"><span data-stu-id="63bed-103">Delete conversationThread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63bed-104">Exclua um conversationThread.</span><span class="sxs-lookup"><span data-stu-id="63bed-104">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="63bed-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="63bed-105">Permissions</span></span>
<span data-ttu-id="63bed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63bed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63bed-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63bed-108">Permission type</span></span>      | <span data-ttu-id="63bed-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63bed-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63bed-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63bed-110">Delegated (work or school account)</span></span> | <span data-ttu-id="63bed-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63bed-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="63bed-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63bed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63bed-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63bed-113">Not supported.</span></span>    |
|<span data-ttu-id="63bed-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63bed-114">Application</span></span> | <span data-ttu-id="63bed-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63bed-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63bed-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63bed-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="63bed-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63bed-117">Request headers</span></span>
| <span data-ttu-id="63bed-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63bed-118">Header</span></span>       | <span data-ttu-id="63bed-119">Valor</span><span class="sxs-lookup"><span data-stu-id="63bed-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="63bed-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="63bed-120">Authorization</span></span>  | <span data-ttu-id="63bed-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63bed-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63bed-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63bed-123">Request body</span></span>
<span data-ttu-id="63bed-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63bed-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63bed-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="63bed-125">Response</span></span>

<span data-ttu-id="63bed-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63bed-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63bed-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63bed-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63bed-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63bed-129">Request</span></span>
<span data-ttu-id="63bed-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63bed-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="63bed-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="63bed-131">Response</span></span>
<span data-ttu-id="63bed-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63bed-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="63bed-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="63bed-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="63bed-134">C#</span><span class="sxs-lookup"><span data-stu-id="63bed-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_conversationthread-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63bed-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="63bed-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_conversationthread-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="63bed-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="63bed-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_conversationthread-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversationthread-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/conversationthread-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/conversationthread-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
