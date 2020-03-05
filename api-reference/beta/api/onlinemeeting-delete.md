---
title: Excluir onlineMeeting
description: Excluir uma reunião online.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9998e67ff9e8ffe93d349115cfe50beb8d317073
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456520"
---
# <a name="delete-onlinemeeting"></a><span data-ttu-id="ad1f5-103">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ad1f5-103">Delete onlineMeeting</span></span>

<span data-ttu-id="ad1f5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ad1f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad1f5-105">Excluir um objeto [onlineMeeting](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="ad1f5-105">Delete an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad1f5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad1f5-106">Permissions</span></span>

| <span data-ttu-id="ad1f5-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad1f5-107">Permission type</span></span> | <span data-ttu-id="ad1f5-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad1f5-108">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="ad1f5-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad1f5-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad1f5-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad1f5-110">OnlineMeetings.ReadWrite</span></span>              |
| <span data-ttu-id="ad1f5-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad1f5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad1f5-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad1f5-112">Not Supported.</span></span>                         |
| <span data-ttu-id="ad1f5-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad1f5-113">Application</span></span>                            | <span data-ttu-id="ad1f5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad1f5-114">Not Supported.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="ad1f5-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad1f5-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ad1f5-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad1f5-116">Request headers</span></span>
| <span data-ttu-id="ad1f5-117">Nome</span><span class="sxs-lookup"><span data-stu-id="ad1f5-117">Name</span></span>          | <span data-ttu-id="ad1f5-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad1f5-118">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ad1f5-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad1f5-119">Authorization</span></span> | <span data-ttu-id="ad1f5-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad1f5-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad1f5-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad1f5-122">Request body</span></span>
<span data-ttu-id="ad1f5-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ad1f5-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad1f5-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad1f5-124">Response</span></span>
<span data-ttu-id="ad1f5-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad1f5-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ad1f5-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ad1f5-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ad1f5-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad1f5-128">Request</span></span>
<span data-ttu-id="ad1f5-129">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad1f5-129">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad1f5-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad1f5-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype
```
# <a name="c"></a>[<span data-ttu-id="ad1f5-131">C#</span><span class="sxs-lookup"><span data-stu-id="ad1f5-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad1f5-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad1f5-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad1f5-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad1f5-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad1f5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad1f5-134">Response</span></span>

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
