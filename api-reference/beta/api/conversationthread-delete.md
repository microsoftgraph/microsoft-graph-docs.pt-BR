---
title: Excluir conversationThread
description: Exclua um conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0db360081d9d371f52bc8a40428ac293ed537e3f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437428"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="a2f9c-103">Excluir conversationThread</span><span class="sxs-lookup"><span data-stu-id="a2f9c-103">Delete conversationThread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2f9c-104">Exclua um conversationThread.</span><span class="sxs-lookup"><span data-stu-id="a2f9c-104">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="a2f9c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2f9c-105">Permissions</span></span>
<span data-ttu-id="a2f9c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2f9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2f9c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2f9c-108">Permission type</span></span>      | <span data-ttu-id="a2f9c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2f9c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2f9c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2f9c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a2f9c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2f9c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2f9c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2f9c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2f9c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2f9c-113">Not supported.</span></span>    |
|<span data-ttu-id="a2f9c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2f9c-114">Application</span></span> | <span data-ttu-id="a2f9c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2f9c-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2f9c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2f9c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="a2f9c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2f9c-117">Request headers</span></span>
| <span data-ttu-id="a2f9c-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2f9c-118">Header</span></span>       | <span data-ttu-id="a2f9c-119">Valor</span><span class="sxs-lookup"><span data-stu-id="a2f9c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a2f9c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2f9c-120">Authorization</span></span>  | <span data-ttu-id="a2f9c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2f9c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a2f9c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2f9c-123">Request body</span></span>
<span data-ttu-id="a2f9c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2f9c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2f9c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2f9c-125">Response</span></span>

<span data-ttu-id="a2f9c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2f9c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2f9c-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2f9c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2f9c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2f9c-129">Request</span></span>
<span data-ttu-id="a2f9c-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2f9c-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a2f9c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2f9c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a2f9c-132">C#</span><span class="sxs-lookup"><span data-stu-id="a2f9c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2f9c-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="a2f9c-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a2f9c-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a2f9c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a2f9c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2f9c-135">Response</span></span>
<span data-ttu-id="a2f9c-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2f9c-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
