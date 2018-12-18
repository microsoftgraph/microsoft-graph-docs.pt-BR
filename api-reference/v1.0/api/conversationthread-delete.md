---
title: Excluir conversationThread
description: Exclua um conversationThread.
author: dkershaw10
ms.openlocfilehash: 37ddcd5c08af3afb0e997af24163754d61a99ff6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304883"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="8fb0a-103">Excluir conversationThread</span><span class="sxs-lookup"><span data-stu-id="8fb0a-103">Delete conversationThread</span></span>

<span data-ttu-id="8fb0a-104">Exclua um conversationThread.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-104">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="8fb0a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8fb0a-105">Permissions</span></span>
<span data-ttu-id="8fb0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fb0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fb0a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fb0a-108">Permission type</span></span>      | <span data-ttu-id="8fb0a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8fb0a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fb0a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fb0a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8fb0a-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fb0a-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8fb0a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fb0a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fb0a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-113">Not supported.</span></span>    |
|<span data-ttu-id="8fb0a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fb0a-114">Application</span></span> | <span data-ttu-id="8fb0a-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fb0a-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fb0a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fb0a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="8fb0a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8fb0a-117">Request headers</span></span>
| <span data-ttu-id="8fb0a-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8fb0a-118">Header</span></span>       | <span data-ttu-id="8fb0a-119">Valor</span><span class="sxs-lookup"><span data-stu-id="8fb0a-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8fb0a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fb0a-120">Authorization</span></span>  | <span data-ttu-id="8fb0a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8fb0a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fb0a-123">Request body</span></span>
<span data-ttu-id="8fb0a-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fb0a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fb0a-125">Response</span></span>

<span data-ttu-id="8fb0a-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fb0a-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8fb0a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8fb0a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fb0a-129">Request</span></span>
<span data-ttu-id="8fb0a-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="8fb0a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fb0a-131">Response</span></span>
<span data-ttu-id="8fb0a-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8fb0a-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->