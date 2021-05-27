---
title: Atualizar thread de conversas
description: Atualize um objeto thread.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 26eab98dc2d734e76905c458c7730d6f6237bc93
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681225"
---
# <a name="update-conversation-thread"></a><span data-ttu-id="4c14d-103">Atualizar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="4c14d-103">Update conversation thread</span></span>

<span data-ttu-id="4c14d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c14d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c14d-105">Atualize um objeto [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="4c14d-105">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c14d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c14d-106">Permissions</span></span>
<span data-ttu-id="4c14d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c14d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c14d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c14d-109">Permission type</span></span>      | <span data-ttu-id="4c14d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c14d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c14d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c14d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4c14d-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c14d-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c14d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c14d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c14d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c14d-114">Not supported.</span></span>    |
|<span data-ttu-id="4c14d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c14d-115">Application</span></span> | <span data-ttu-id="4c14d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c14d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c14d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c14d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4c14d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c14d-118">Request headers</span></span>
| <span data-ttu-id="4c14d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4c14d-119">Name</span></span>       | <span data-ttu-id="4c14d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c14d-120">Type</span></span> | <span data-ttu-id="4c14d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c14d-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4c14d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c14d-122">Authorization</span></span>  | <span data-ttu-id="4c14d-123">string</span><span class="sxs-lookup"><span data-stu-id="4c14d-123">string</span></span>  | <span data-ttu-id="4c14d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c14d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c14d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c14d-126">Request body</span></span>
<span data-ttu-id="4c14d-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4c14d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="4c14d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c14d-130">Response</span></span>
<span data-ttu-id="4c14d-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4c14d-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4c14d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c14d-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4c14d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c14d-133">Request</span></span>
<span data-ttu-id="4c14d-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c14d-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4c14d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c14d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_thread"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
Content-type: application/json
Content-length: 655

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="4c14d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c14d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4c14d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c14d-137">Response</span></span>
<span data-ttu-id="4c14d-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c14d-138">The following is an example of the response.</span></span>

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
  "description": "Update group thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


