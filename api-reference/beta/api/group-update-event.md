---
title: Atualizar evento
description: Atualize um objeto event.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 575a449460f9f3da8edcdf17b63fb075a975e3e5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953764"
---
# <a name="update-event"></a><span data-ttu-id="a5f08-103">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="a5f08-103">Update event</span></span>

<span data-ttu-id="a5f08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5f08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5f08-105">Atualize um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="a5f08-105">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5f08-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5f08-106">Permissions</span></span>
<span data-ttu-id="a5f08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5f08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5f08-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5f08-109">Permission type</span></span>      | <span data-ttu-id="a5f08-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5f08-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5f08-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5f08-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a5f08-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5f08-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5f08-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5f08-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5f08-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5f08-114">Not supported.</span></span>    |
|<span data-ttu-id="a5f08-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5f08-115">Application</span></span> | <span data-ttu-id="a5f08-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5f08-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5f08-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5f08-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a5f08-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5f08-118">Request headers</span></span>
| <span data-ttu-id="a5f08-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a5f08-119">Name</span></span>       | <span data-ttu-id="a5f08-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5f08-120">Type</span></span> | <span data-ttu-id="a5f08-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5f08-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a5f08-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5f08-122">Authorization</span></span>  | <span data-ttu-id="a5f08-123">string</span><span class="sxs-lookup"><span data-stu-id="a5f08-123">string</span></span>  | <span data-ttu-id="a5f08-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5f08-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5f08-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5f08-126">Request body</span></span>
<span data-ttu-id="a5f08-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a5f08-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="a5f08-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5f08-130">Response</span></span>
<span data-ttu-id="a5f08-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a5f08-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a5f08-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5f08-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a5f08-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5f08-133">Request</span></span>
<span data-ttu-id="a5f08-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5f08-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a5f08-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5f08-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

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
# <a name="c"></a>[<span data-ttu-id="a5f08-136">C#</span><span class="sxs-lookup"><span data-stu-id="a5f08-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5f08-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5f08-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5f08-138">Java</span><span class="sxs-lookup"><span data-stu-id="a5f08-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a5f08-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5f08-139">Response</span></span>
<span data-ttu-id="a5f08-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a5f08-140">The following is an example of the response.</span></span>

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
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


