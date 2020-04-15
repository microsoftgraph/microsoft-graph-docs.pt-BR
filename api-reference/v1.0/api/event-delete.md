---
title: Excluir evento
description: Exclua um evento.
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5198db8d842f81c2968fa3a3a5315f34ec246790
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461679"
---
# <a name="delete-event"></a><span data-ttu-id="bdd89-103">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="bdd89-103">Delete event</span></span>

<span data-ttu-id="bdd89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdd89-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bdd89-105">Remove o [evento](../resources/event.md) especificado do calendário que o contém.</span><span class="sxs-lookup"><span data-stu-id="bdd89-105">Removes the specified [event](../resources/event.md) from the containing calendar.</span></span> 

<span data-ttu-id="bdd89-106">Se o evento for uma reunião, exclui-lo no calendário do organizador enviará uma mensagem de cancelamento aos participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="bdd89-106">If the event is a meeting, deleting the event on the organizer's calendar sends a cancellation message to the meeting attendees.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdd89-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdd89-107">Permissions</span></span>
<span data-ttu-id="bdd89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdd89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdd89-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdd89-110">Permission type</span></span>      | <span data-ttu-id="bdd89-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdd89-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdd89-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdd89-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bdd89-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdd89-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bdd89-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdd89-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdd89-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdd89-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bdd89-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdd89-116">Application</span></span> | <span data-ttu-id="bdd89-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdd89-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdd89-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdd89-118">HTTP request</span></span>
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

DELETE /me/calendargroup/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bdd89-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdd89-119">Request headers</span></span>
| <span data-ttu-id="bdd89-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bdd89-120">Name</span></span>       | <span data-ttu-id="bdd89-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdd89-121">Type</span></span> | <span data-ttu-id="bdd89-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdd89-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bdd89-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdd89-123">Authorization</span></span>  | <span data-ttu-id="bdd89-124">string</span><span class="sxs-lookup"><span data-stu-id="bdd89-124">string</span></span>  | <span data-ttu-id="bdd89-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdd89-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdd89-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdd89-127">Request body</span></span>
<span data-ttu-id="bdd89-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bdd89-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdd89-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdd89-129">Response</span></span>

<span data-ttu-id="bdd89-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdd89-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdd89-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdd89-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bdd89-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdd89-133">Request</span></span>
<span data-ttu-id="bdd89-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdd89-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bdd89-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdd89-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}
```
# <a name="c"></a>[<span data-ttu-id="bdd89-136">C#</span><span class="sxs-lookup"><span data-stu-id="bdd89-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bdd89-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdd89-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bdd89-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bdd89-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bdd89-139">Java</span><span class="sxs-lookup"><span data-stu-id="bdd89-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bdd89-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdd89-140">Response</span></span>
<span data-ttu-id="bdd89-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdd89-141">Here is an example of the response.</span></span> 
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
