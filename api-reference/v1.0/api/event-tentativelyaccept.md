---
title: 'event: tentativelyAccept'
description: Aceitar provisoriamente o evento específico em um calendário de usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 52acf0c7f39c3559e3c2d1eb220c760d79e77845
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517324"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="38120-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="38120-103">event: tentativelyAccept</span></span>

<span data-ttu-id="38120-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38120-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="38120-105">Aceitar provisoriamente o [evento](../resources/event.md) especificado em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="38120-105">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="38120-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="38120-106">Permissions</span></span>
<span data-ttu-id="38120-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38120-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38120-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38120-109">Permission type</span></span>      | <span data-ttu-id="38120-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38120-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38120-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38120-111">Delegated (work or school account)</span></span> | <span data-ttu-id="38120-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38120-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="38120-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38120-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38120-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38120-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="38120-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38120-115">Application</span></span> | <span data-ttu-id="38120-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38120-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="38120-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38120-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="38120-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38120-118">Request headers</span></span>
| <span data-ttu-id="38120-119">Nome</span><span class="sxs-lookup"><span data-stu-id="38120-119">Name</span></span>       | <span data-ttu-id="38120-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="38120-120">Type</span></span> | <span data-ttu-id="38120-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="38120-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="38120-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="38120-122">Authorization</span></span>  | <span data-ttu-id="38120-123">string</span><span class="sxs-lookup"><span data-stu-id="38120-123">string</span></span>  | <span data-ttu-id="38120-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38120-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38120-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38120-126">Content-Type</span></span> | <span data-ttu-id="38120-127">string</span><span class="sxs-lookup"><span data-stu-id="38120-127">string</span></span>  | <span data-ttu-id="38120-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38120-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38120-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38120-130">Request body</span></span>
<span data-ttu-id="38120-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38120-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="38120-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="38120-132">Parameter</span></span>    | <span data-ttu-id="38120-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="38120-133">Type</span></span>   |<span data-ttu-id="38120-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="38120-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38120-135">comment</span><span class="sxs-lookup"><span data-stu-id="38120-135">comment</span></span>|<span data-ttu-id="38120-136">String</span><span class="sxs-lookup"><span data-stu-id="38120-136">String</span></span>|<span data-ttu-id="38120-p104">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="38120-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="38120-139">sendResponse</span><span class="sxs-lookup"><span data-stu-id="38120-139">sendResponse</span></span>|<span data-ttu-id="38120-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="38120-140">Boolean</span></span>|<span data-ttu-id="38120-p105">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="38120-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="38120-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="38120-144">Response</span></span>

<span data-ttu-id="38120-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38120-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38120-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38120-147">Example</span></span>
<span data-ttu-id="38120-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="38120-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="38120-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38120-149">Request</span></span>
<span data-ttu-id="38120-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38120-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38120-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="38120-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/tentativelyAccept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```
# <a name="c"></a>[<span data-ttu-id="38120-152">C#</span><span class="sxs-lookup"><span data-stu-id="38120-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38120-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38120-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38120-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38120-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38120-155">Java</span><span class="sxs-lookup"><span data-stu-id="38120-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-tentativelyaccept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="38120-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="38120-156">Response</span></span>
##### <a name="response"></a><span data-ttu-id="38120-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="38120-157">Response</span></span>
<span data-ttu-id="38120-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38120-158">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
