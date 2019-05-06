---
title: Excluir conversationThread
description: Exclua um conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a89176839875d4b5ecd3edd6e4d83242d29be567
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591108"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="e4433-103">Excluir conversationThread</span><span class="sxs-lookup"><span data-stu-id="e4433-103">Delete conversationThread</span></span>

<span data-ttu-id="e4433-104">Exclua um conversationThread.</span><span class="sxs-lookup"><span data-stu-id="e4433-104">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="e4433-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4433-105">Permissions</span></span>
<span data-ttu-id="e4433-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4433-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4433-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4433-108">Permission type</span></span>      | <span data-ttu-id="e4433-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4433-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4433-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4433-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e4433-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4433-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4433-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4433-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4433-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4433-113">Not supported.</span></span>    |
|<span data-ttu-id="e4433-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4433-114">Application</span></span> | <span data-ttu-id="e4433-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4433-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4433-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4433-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e4433-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4433-117">Request headers</span></span>
| <span data-ttu-id="e4433-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4433-118">Header</span></span>       | <span data-ttu-id="e4433-119">Valor</span><span class="sxs-lookup"><span data-stu-id="e4433-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e4433-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4433-120">Authorization</span></span>  | <span data-ttu-id="e4433-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4433-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e4433-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4433-123">Request body</span></span>
<span data-ttu-id="e4433-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4433-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4433-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4433-125">Response</span></span>

<span data-ttu-id="e4433-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4433-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4433-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4433-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4433-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4433-129">Request</span></span>
<span data-ttu-id="e4433-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4433-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="e4433-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4433-131">Response</span></span>
<span data-ttu-id="e4433-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4433-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e4433-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e4433-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e4433-134">Basic</span><span class="sxs-lookup"><span data-stu-id="e4433-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_conversationthread-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e4433-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4433-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_conversationthread-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/conversationthread-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/conversationthread-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
