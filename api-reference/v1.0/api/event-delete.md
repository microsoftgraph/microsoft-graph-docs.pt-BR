---
title: Excluir evento
description: Exclua um evento.
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6732793721fb57f789a15a2decc491ea368de96f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441918"
---
# <a name="delete-event"></a><span data-ttu-id="60b5b-103">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="60b5b-103">Delete event</span></span>

<span data-ttu-id="60b5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60b5b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60b5b-105">Remove o [evento](../resources/event.md) especificado do calendário que o contém.</span><span class="sxs-lookup"><span data-stu-id="60b5b-105">Removes the specified [event](../resources/event.md) from the containing calendar.</span></span> 

<span data-ttu-id="60b5b-106">Se o evento for uma reunião, exclui-lo no calendário do organizador enviará uma mensagem de cancelamento aos participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="60b5b-106">If the event is a meeting, deleting the event on the organizer's calendar sends a cancellation message to the meeting attendees.</span></span>

## <a name="permissions"></a><span data-ttu-id="60b5b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="60b5b-107">Permissions</span></span>
<span data-ttu-id="60b5b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60b5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60b5b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60b5b-110">Permission type</span></span>      | <span data-ttu-id="60b5b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60b5b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60b5b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60b5b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="60b5b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60b5b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="60b5b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60b5b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60b5b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60b5b-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="60b5b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60b5b-116">Application</span></span> | <span data-ttu-id="60b5b-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60b5b-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="60b5b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60b5b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}
DELETE /users/{id | userPrincipalName}/events/{id}
DELETE /groups/{id}/events/{id}

DELETE /me/calendar/events/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}
DELETE /groups/{id}/calendar/events/{id}/

DELETE /me/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="60b5b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60b5b-119">Request headers</span></span>
| <span data-ttu-id="60b5b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="60b5b-120">Name</span></span>       | <span data-ttu-id="60b5b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="60b5b-121">Type</span></span> | <span data-ttu-id="60b5b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="60b5b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="60b5b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="60b5b-123">Authorization</span></span>  | <span data-ttu-id="60b5b-124">string</span><span class="sxs-lookup"><span data-stu-id="60b5b-124">string</span></span>  | <span data-ttu-id="60b5b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60b5b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60b5b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60b5b-127">Request body</span></span>
<span data-ttu-id="60b5b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60b5b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60b5b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="60b5b-129">Response</span></span>

<span data-ttu-id="60b5b-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60b5b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60b5b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60b5b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60b5b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60b5b-133">Request</span></span>
<span data-ttu-id="60b5b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60b5b-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="60b5b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="60b5b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}
```
# <a name="c"></a>[<span data-ttu-id="60b5b-136">C#</span><span class="sxs-lookup"><span data-stu-id="60b5b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60b5b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60b5b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60b5b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60b5b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60b5b-139">Java</span><span class="sxs-lookup"><span data-stu-id="60b5b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="60b5b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="60b5b-140">Response</span></span>
<span data-ttu-id="60b5b-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60b5b-141">Here is an example of the response.</span></span> 
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

