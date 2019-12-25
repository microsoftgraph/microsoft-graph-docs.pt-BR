---
title: Excluir onlineMeeting
description: Excluir uma reunião online.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d6b5f0afa09bf88c9f070ef88adda2f5be20c50f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871718"
---
# <a name="delete-onlinemeeting"></a><span data-ttu-id="bc1d0-103">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="bc1d0-103">Delete onlineMeeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc1d0-104">Excluir um objeto [onlineMeeting](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="bc1d0-104">Delete an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc1d0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc1d0-105">Permissions</span></span>

| <span data-ttu-id="bc1d0-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc1d0-106">Permission type</span></span> | <span data-ttu-id="bc1d0-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc1d0-107">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="bc1d0-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc1d0-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="bc1d0-109">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc1d0-109">OnlineMeetings.ReadWrite</span></span>              |
| <span data-ttu-id="bc1d0-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc1d0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc1d0-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc1d0-111">Not Supported.</span></span>                         |
| <span data-ttu-id="bc1d0-112">Application</span><span class="sxs-lookup"><span data-stu-id="bc1d0-112">Application</span></span>                            | <span data-ttu-id="bc1d0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc1d0-113">Not Supported.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="bc1d0-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc1d0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bc1d0-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc1d0-115">Request headers</span></span>
| <span data-ttu-id="bc1d0-116">Nome</span><span class="sxs-lookup"><span data-stu-id="bc1d0-116">Name</span></span>          | <span data-ttu-id="bc1d0-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc1d0-117">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="bc1d0-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc1d0-118">Authorization</span></span> | <span data-ttu-id="bc1d0-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc1d0-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc1d0-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc1d0-121">Request body</span></span>
<span data-ttu-id="bc1d0-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc1d0-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc1d0-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc1d0-123">Response</span></span>
<span data-ttu-id="bc1d0-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc1d0-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bc1d0-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bc1d0-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bc1d0-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc1d0-127">Request</span></span>
<span data-ttu-id="bc1d0-128">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc1d0-128">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bc1d0-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc1d0-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bc1d0-130">C#</span><span class="sxs-lookup"><span data-stu-id="bc1d0-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc1d0-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc1d0-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bc1d0-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc1d0-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bc1d0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc1d0-133">Response</span></span>

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
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
