---
title: 'event: accept'
description: Aceite o evento específico em um calendário do usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ccf2d3cf1bf25720decb6eb009639f6ea9c252c4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587183"
---
# <a name="event-accept"></a><span data-ttu-id="eccfc-103">event: accept</span><span class="sxs-lookup"><span data-stu-id="eccfc-103">event: accept</span></span>

<span data-ttu-id="eccfc-104">Aceite o [evento](../resources/event.md) especificado em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="eccfc-104">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eccfc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="eccfc-105">Permissions</span></span>
<span data-ttu-id="eccfc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eccfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eccfc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eccfc-108">Permission type</span></span>      | <span data-ttu-id="eccfc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eccfc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eccfc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eccfc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eccfc-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eccfc-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="eccfc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eccfc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eccfc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eccfc-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="eccfc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eccfc-114">Application</span></span> | <span data-ttu-id="eccfc-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eccfc-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eccfc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eccfc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/accept
POST /users/{id | userPrincipalName}/events/{id}/accept

POST /me/calendar/events/{id}/accept
POST /users/{id | userPrincipalName}/calendar/events/{id}/accept

POST /me/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/accept

POST /me/calendargroup/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/accept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/accept
```
## <a name="request-headers"></a><span data-ttu-id="eccfc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eccfc-117">Request headers</span></span>
| <span data-ttu-id="eccfc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="eccfc-118">Name</span></span>       | <span data-ttu-id="eccfc-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="eccfc-119">Type</span></span> | <span data-ttu-id="eccfc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="eccfc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eccfc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="eccfc-121">Authorization</span></span>  | <span data-ttu-id="eccfc-122">string</span><span class="sxs-lookup"><span data-stu-id="eccfc-122">string</span></span>  | <span data-ttu-id="eccfc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eccfc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eccfc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eccfc-125">Content-Type</span></span> | <span data-ttu-id="eccfc-126">string</span><span class="sxs-lookup"><span data-stu-id="eccfc-126">string</span></span>  | <span data-ttu-id="eccfc-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eccfc-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eccfc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eccfc-129">Request body</span></span>
<span data-ttu-id="eccfc-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eccfc-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eccfc-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="eccfc-131">Parameter</span></span>    | <span data-ttu-id="eccfc-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="eccfc-132">Type</span></span>   |<span data-ttu-id="eccfc-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="eccfc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eccfc-134">comment</span><span class="sxs-lookup"><span data-stu-id="eccfc-134">comment</span></span>|<span data-ttu-id="eccfc-135">String</span><span class="sxs-lookup"><span data-stu-id="eccfc-135">String</span></span>|<span data-ttu-id="eccfc-p104">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="eccfc-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="eccfc-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="eccfc-138">sendResponse</span></span>|<span data-ttu-id="eccfc-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="eccfc-139">Boolean</span></span>|<span data-ttu-id="eccfc-p105">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="eccfc-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="eccfc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="eccfc-143">Response</span></span>

<span data-ttu-id="eccfc-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eccfc-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eccfc-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eccfc-146">Example</span></span>
<span data-ttu-id="eccfc-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="eccfc-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eccfc-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eccfc-148">Request</span></span>
<span data-ttu-id="eccfc-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eccfc-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_accept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/accept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="eccfc-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="eccfc-150">Response</span></span>
<span data-ttu-id="eccfc-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eccfc-151">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="eccfc-152">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="eccfc-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eccfc-153">Basic</span><span class="sxs-lookup"><span data-stu-id="eccfc-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_accept-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eccfc-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eccfc-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_accept-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/event-accept.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/event-accept.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
