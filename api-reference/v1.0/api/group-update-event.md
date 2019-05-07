---
title: Atualizar evento
description: Atualize um objeto event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9b6c61ba2e63fab0572a9efc76dccc56c581be0d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612981"
---
# <a name="update-event"></a><span data-ttu-id="5dc88-103">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="5dc88-103">Update event</span></span>
<span data-ttu-id="5dc88-104">Atualize um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="5dc88-104">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5dc88-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5dc88-105">Permissions</span></span>
<span data-ttu-id="5dc88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dc88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dc88-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dc88-108">Permission type</span></span>      | <span data-ttu-id="5dc88-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5dc88-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dc88-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dc88-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5dc88-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dc88-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5dc88-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dc88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dc88-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dc88-113">Not supported.</span></span>    |
|<span data-ttu-id="5dc88-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dc88-114">Application</span></span> | <span data-ttu-id="5dc88-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dc88-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5dc88-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dc88-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5dc88-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc88-117">Request headers</span></span>
| <span data-ttu-id="5dc88-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5dc88-118">Name</span></span>       | <span data-ttu-id="5dc88-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dc88-119">Type</span></span> | <span data-ttu-id="5dc88-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dc88-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5dc88-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dc88-121">Authorization</span></span>  | <span data-ttu-id="5dc88-122">string</span><span class="sxs-lookup"><span data-stu-id="5dc88-122">string</span></span>  | <span data-ttu-id="5dc88-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dc88-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5dc88-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc88-125">Request body</span></span>
<span data-ttu-id="5dc88-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5dc88-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="5dc88-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc88-129">Response</span></span>
<span data-ttu-id="5dc88-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5dc88-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5dc88-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dc88-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5dc88-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc88-132">Request</span></span>
<span data-ttu-id="5dc88-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dc88-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

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

#### <a name="response"></a><span data-ttu-id="5dc88-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc88-134">Response</span></span>
<span data-ttu-id="5dc88-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5dc88-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5dc88-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5dc88-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5dc88-137">Basic</span><span class="sxs-lookup"><span data-stu-id="5dc88-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_group_event-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5dc88-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5dc88-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_group_event-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-update-event.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-update-event.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
