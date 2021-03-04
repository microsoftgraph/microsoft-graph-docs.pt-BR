---
title: Excluir evento
description: Exclua um evento.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b73bdae172fe87e91a5485aa786e7556157eb6f1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436257"
---
# <a name="delete-event"></a><span data-ttu-id="42f93-103">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="42f93-103">Delete event</span></span>

<span data-ttu-id="42f93-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42f93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42f93-105">Remove o [evento](../resources/event.md) especificado do calendário que o contém.</span><span class="sxs-lookup"><span data-stu-id="42f93-105">Removes the specified [event](../resources/event.md) from the containing calendar.</span></span> 

<span data-ttu-id="42f93-106">Se o evento for uma reunião, exclui-lo no calendário do organizador enviará uma mensagem de cancelamento aos participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="42f93-106">If the event is a meeting, deleting the event on the organizer's calendar sends a cancellation message to the meeting attendees.</span></span>

## <a name="permissions"></a><span data-ttu-id="42f93-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="42f93-107">Permissions</span></span>
<span data-ttu-id="42f93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42f93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42f93-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42f93-110">Permission type</span></span>      | <span data-ttu-id="42f93-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42f93-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42f93-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42f93-112">Delegated (work or school account)</span></span> | <span data-ttu-id="42f93-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42f93-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="42f93-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42f93-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42f93-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42f93-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="42f93-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42f93-116">Application</span></span> | <span data-ttu-id="42f93-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42f93-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="42f93-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42f93-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="42f93-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42f93-119">Request headers</span></span>
| <span data-ttu-id="42f93-120">Nome</span><span class="sxs-lookup"><span data-stu-id="42f93-120">Name</span></span>       | <span data-ttu-id="42f93-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="42f93-121">Type</span></span> | <span data-ttu-id="42f93-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="42f93-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="42f93-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="42f93-123">Authorization</span></span>  | <span data-ttu-id="42f93-124">string</span><span class="sxs-lookup"><span data-stu-id="42f93-124">string</span></span>  | <span data-ttu-id="42f93-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42f93-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42f93-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42f93-127">Request body</span></span>
<span data-ttu-id="42f93-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42f93-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42f93-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="42f93-129">Response</span></span>

<span data-ttu-id="42f93-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42f93-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42f93-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42f93-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42f93-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42f93-133">Request</span></span>
<span data-ttu-id="42f93-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42f93-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42f93-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="42f93-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}
```
# <a name="c"></a>[<span data-ttu-id="42f93-136">C#</span><span class="sxs-lookup"><span data-stu-id="42f93-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42f93-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42f93-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42f93-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42f93-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42f93-139">Java</span><span class="sxs-lookup"><span data-stu-id="42f93-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="42f93-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="42f93-140">Response</span></span>
<span data-ttu-id="42f93-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42f93-141">Here is an example of the response.</span></span> 
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


