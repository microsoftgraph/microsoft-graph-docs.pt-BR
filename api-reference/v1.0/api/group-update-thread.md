---
title: Atualizar thread de conversas
description: Atualize um objeto thread.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1216771a7955cc9460faeab420b8550150d55b84
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679866"
---
# <a name="update-conversation-thread"></a><span data-ttu-id="64db7-103">Atualizar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="64db7-103">Update conversation thread</span></span>

<span data-ttu-id="64db7-104">Namespace: microsoft.graph Atualizar um [objeto thread.](../resources/conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="64db7-104">Namespace: microsoft.graph Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64db7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="64db7-105">Permissions</span></span>
<span data-ttu-id="64db7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64db7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64db7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64db7-108">Permission type</span></span>      | <span data-ttu-id="64db7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64db7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64db7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64db7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="64db7-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64db7-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="64db7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64db7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64db7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64db7-113">Not supported.</span></span>    |
|<span data-ttu-id="64db7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64db7-114">Application</span></span> | <span data-ttu-id="64db7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64db7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64db7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64db7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="64db7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64db7-117">Request headers</span></span>
| <span data-ttu-id="64db7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="64db7-118">Name</span></span>       | <span data-ttu-id="64db7-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="64db7-119">Type</span></span> | <span data-ttu-id="64db7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="64db7-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="64db7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="64db7-121">Authorization</span></span>  | <span data-ttu-id="64db7-122">string</span><span class="sxs-lookup"><span data-stu-id="64db7-122">string</span></span>  | <span data-ttu-id="64db7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64db7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64db7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64db7-125">Request body</span></span>
<span data-ttu-id="64db7-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="64db7-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="64db7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="64db7-129">Response</span></span>
<span data-ttu-id="64db7-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="64db7-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="64db7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64db7-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="64db7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64db7-132">Request</span></span>
<span data-ttu-id="64db7-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64db7-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="64db7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="64db7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "update_group_thread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
Content-type: application/json
Content-length: 655

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="64db7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64db7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="64db7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="64db7-136">Response</span></span>
<span data-ttu-id="64db7-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64db7-137">The following is an example of the response.</span></span>

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
  "description": "Update group thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

