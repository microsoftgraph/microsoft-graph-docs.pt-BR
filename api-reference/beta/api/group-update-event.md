---
title: Atualizar evento
description: Atualize um objeto event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4694f7e9435f886538f7d4d6e21b141e3fd470b0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323119"
---
# <a name="update-event"></a><span data-ttu-id="1ba4e-103">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="1ba4e-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ba4e-104">Atualize um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="1ba4e-104">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ba4e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1ba4e-105">Permissions</span></span>
<span data-ttu-id="1ba4e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ba4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ba4e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ba4e-108">Permission type</span></span>      | <span data-ttu-id="1ba4e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1ba4e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ba4e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ba4e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1ba4e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ba4e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1ba4e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ba4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ba4e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ba4e-113">Not supported.</span></span>    |
|<span data-ttu-id="1ba4e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ba4e-114">Application</span></span> | <span data-ttu-id="1ba4e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ba4e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ba4e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ba4e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1ba4e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ba4e-117">Request headers</span></span>
| <span data-ttu-id="1ba4e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1ba4e-118">Name</span></span>       | <span data-ttu-id="1ba4e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ba4e-119">Type</span></span> | <span data-ttu-id="1ba4e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ba4e-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1ba4e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ba4e-121">Authorization</span></span>  | <span data-ttu-id="1ba4e-122">string</span><span class="sxs-lookup"><span data-stu-id="1ba4e-122">string</span></span>  | <span data-ttu-id="1ba4e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ba4e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ba4e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ba4e-125">Request body</span></span>
<span data-ttu-id="1ba4e-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1ba4e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="1ba4e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ba4e-129">Response</span></span>
<span data-ttu-id="1ba4e-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1ba4e-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1ba4e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ba4e-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1ba4e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ba4e-132">Request</span></span>
<span data-ttu-id="1ba4e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ba4e-133">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1ba4e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ba4e-134">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1ba4e-135">C#</span><span class="sxs-lookup"><span data-stu-id="1ba4e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ba4e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ba4e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1ba4e-137">Java</span><span class="sxs-lookup"><span data-stu-id="1ba4e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1ba4e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ba4e-138">Response</span></span>
<span data-ttu-id="1ba4e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1ba4e-139">The following is an example of the response.</span></span>

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
