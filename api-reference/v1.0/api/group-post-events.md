---
title: Criar evento
description: Use esta API para criar um novo evento.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: f2cfa417ba5064fd91744d8ded48a7fb3621b67b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613735"
---
# <a name="create-event"></a><span data-ttu-id="66309-103">Criar evento</span><span class="sxs-lookup"><span data-stu-id="66309-103">Create event</span></span>
<span data-ttu-id="66309-104">Use esta API para criar um novo [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="66309-104">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="66309-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="66309-105">Permissions</span></span>
<span data-ttu-id="66309-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66309-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66309-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66309-108">Permission type</span></span>      | <span data-ttu-id="66309-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66309-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66309-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66309-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66309-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66309-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="66309-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66309-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66309-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66309-113">Not supported.</span></span>    |
|<span data-ttu-id="66309-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66309-114">Application</span></span> | <span data-ttu-id="66309-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66309-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66309-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66309-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="66309-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66309-117">Request headers</span></span>
| <span data-ttu-id="66309-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="66309-118">Header</span></span>       | <span data-ttu-id="66309-119">Valor</span><span class="sxs-lookup"><span data-stu-id="66309-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="66309-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="66309-120">Authorization</span></span>  | <span data-ttu-id="66309-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66309-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="66309-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66309-123">Request body</span></span>
<span data-ttu-id="66309-124">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="66309-124">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="66309-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="66309-125">Response</span></span>
<span data-ttu-id="66309-126">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66309-126">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66309-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66309-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="66309-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66309-128">Request</span></span>
<span data-ttu-id="66309-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="66309-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/events
Content-type: application/json
Content-length: 285

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
<span data-ttu-id="66309-130">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="66309-130">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="66309-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="66309-131">Response</span></span>
<span data-ttu-id="66309-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="66309-132">The following is an example of the response.</span></span>
><span data-ttu-id="66309-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66309-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 285

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="66309-135">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="66309-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="66309-136">C#</span><span class="sxs-lookup"><span data-stu-id="66309-136">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_event_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66309-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="66309-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_event_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
