---
title: 'evento: dismissReminder'
description: Descartar um lembrete que foi disparado para um evento em um calendário do usuário.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fb0b85a804013f4b282de3d2fae33bcc3f7f67ef
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436215"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="8a9f2-103">evento: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="8a9f2-103">event: dismissReminder</span></span>

<span data-ttu-id="8a9f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a9f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a9f2-105">Descartar um lembrete que foi disparado para um [evento](../resources/event.md) em um calendário do [usuário.](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="8a9f2-105">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8a9f2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a9f2-106">Permissions</span></span>
<span data-ttu-id="8a9f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a9f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a9f2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a9f2-109">Permission type</span></span>      | <span data-ttu-id="8a9f2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a9f2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a9f2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a9f2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8a9f2-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a9f2-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8a9f2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a9f2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a9f2-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a9f2-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8a9f2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a9f2-115">Application</span></span> | <span data-ttu-id="8a9f2-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a9f2-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a9f2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a9f2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```

## <a name="request-headers"></a><span data-ttu-id="8a9f2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a9f2-118">Request headers</span></span>

| <span data-ttu-id="8a9f2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8a9f2-119">Name</span></span>       | <span data-ttu-id="8a9f2-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a9f2-120">Type</span></span> | <span data-ttu-id="8a9f2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a9f2-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8a9f2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a9f2-122">Authorization</span></span>  | <span data-ttu-id="8a9f2-123">string</span><span class="sxs-lookup"><span data-stu-id="8a9f2-123">string</span></span>  | <span data-ttu-id="8a9f2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a9f2-p102">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="8a9f2-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a9f2-126">Response</span></span>

<span data-ttu-id="8a9f2-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a9f2-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a9f2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a9f2-129">Example</span></span>

<span data-ttu-id="8a9f2-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8a9f2-130">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8a9f2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a9f2-131">Request</span></span>
<span data-ttu-id="8a9f2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a9f2-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8a9f2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a9f2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```
# <a name="c"></a>[<span data-ttu-id="8a9f2-134">C#</span><span class="sxs-lookup"><span data-stu-id="8a9f2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-dismissreminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a9f2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a9f2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-dismissreminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a9f2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a9f2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-dismissreminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a9f2-137">Java</span><span class="sxs-lookup"><span data-stu-id="8a9f2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-dismissreminder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8a9f2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a9f2-138">Response</span></span>
<span data-ttu-id="8a9f2-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a9f2-139">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


