---
title: 'evento: dismissReminder'
description: Ignorar um lembrete que foi disparado para um evento em um calendário do usuário.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a5613b2a250e5845baa7fd9d53743ed7a24c9da1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43371054"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="006cf-103">evento: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="006cf-103">event: dismissReminder</span></span>

<span data-ttu-id="006cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="006cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="006cf-105">Ignorar um lembrete que foi disparado para um [evento](../resources/event.md) em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="006cf-105">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="006cf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="006cf-106">Permissions</span></span>
<span data-ttu-id="006cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="006cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="006cf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="006cf-109">Permission type</span></span>      | <span data-ttu-id="006cf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="006cf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="006cf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="006cf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="006cf-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="006cf-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="006cf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="006cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="006cf-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="006cf-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="006cf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="006cf-115">Application</span></span> | <span data-ttu-id="006cf-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="006cf-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="006cf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="006cf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroup/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="006cf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="006cf-118">Request headers</span></span>
| <span data-ttu-id="006cf-119">Nome</span><span class="sxs-lookup"><span data-stu-id="006cf-119">Name</span></span>       | <span data-ttu-id="006cf-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="006cf-120">Type</span></span> | <span data-ttu-id="006cf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="006cf-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="006cf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="006cf-122">Authorization</span></span>  | <span data-ttu-id="006cf-123">string</span><span class="sxs-lookup"><span data-stu-id="006cf-123">string</span></span>  | <span data-ttu-id="006cf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="006cf-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="006cf-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="006cf-126">Response</span></span>

<span data-ttu-id="006cf-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="006cf-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="006cf-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="006cf-129">Example</span></span>

<span data-ttu-id="006cf-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="006cf-130">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="006cf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="006cf-131">Request</span></span>
<span data-ttu-id="006cf-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="006cf-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="006cf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="006cf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```
# <a name="c"></a>[<span data-ttu-id="006cf-134">C#</span><span class="sxs-lookup"><span data-stu-id="006cf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-dismissreminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="006cf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="006cf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-dismissreminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="006cf-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="006cf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-dismissreminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="006cf-137">Java</span><span class="sxs-lookup"><span data-stu-id="006cf-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-dismissreminder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<br/>

### <a name="response"></a><span data-ttu-id="006cf-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="006cf-138">Response</span></span>
<span data-ttu-id="006cf-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="006cf-139">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
