---
title: Excluir onlineMeeting
description: Excluir uma reunião online.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8482e3a273d32f893a8e379c16ab3f8f98adf3e6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057196"
---
# <a name="delete-onlinemeeting"></a><span data-ttu-id="f49bf-103">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f49bf-103">Delete onlineMeeting</span></span>

<span data-ttu-id="f49bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f49bf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f49bf-105">Excluir um objeto [onlineMeeting](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="f49bf-105">Delete an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f49bf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f49bf-106">Permissions</span></span>

| <span data-ttu-id="f49bf-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f49bf-107">Permission type</span></span> | <span data-ttu-id="f49bf-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f49bf-108">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="f49bf-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f49bf-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="f49bf-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f49bf-110">OnlineMeetings.ReadWrite</span></span>              |
| <span data-ttu-id="f49bf-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f49bf-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f49bf-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f49bf-112">Not Supported.</span></span>                         |
| <span data-ttu-id="f49bf-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f49bf-113">Application</span></span>                            | <span data-ttu-id="f49bf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f49bf-114">Not Supported.</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f49bf-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f49bf-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/me/onlineMeetings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f49bf-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f49bf-116">Request headers</span></span>
| <span data-ttu-id="f49bf-117">Nome</span><span class="sxs-lookup"><span data-stu-id="f49bf-117">Name</span></span>          | <span data-ttu-id="f49bf-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="f49bf-118">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f49bf-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="f49bf-119">Authorization</span></span> | <span data-ttu-id="f49bf-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f49bf-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f49bf-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f49bf-122">Request body</span></span>
<span data-ttu-id="f49bf-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f49bf-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f49bf-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="f49bf-124">Response</span></span>
<span data-ttu-id="f49bf-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f49bf-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f49bf-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f49bf-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f49bf-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f49bf-128">Request</span></span>
<span data-ttu-id="f49bf-129">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="f49bf-129">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f49bf-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f49bf-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype
```
# <a name="c"></a>[<span data-ttu-id="f49bf-131">C#</span><span class="sxs-lookup"><span data-stu-id="f49bf-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f49bf-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f49bf-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f49bf-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f49bf-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f49bf-134">Java</span><span class="sxs-lookup"><span data-stu-id="f49bf-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f49bf-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f49bf-135">Response</span></span>

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

