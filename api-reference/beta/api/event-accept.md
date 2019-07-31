---
title: 'event: accept'
description: Aceite o evento específico em um calendário do usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5df91e774139cd416459982a5c3d44988299af3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954610"
---
# <a name="event-accept"></a><span data-ttu-id="7bb72-103">event: accept</span><span class="sxs-lookup"><span data-stu-id="7bb72-103">event: accept</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bb72-104">Aceite o [evento](../resources/event.md) especificado em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="7bb72-104">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7bb72-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bb72-105">Permissions</span></span>
<span data-ttu-id="7bb72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bb72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bb72-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bb72-108">Permission type</span></span>      | <span data-ttu-id="7bb72-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7bb72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bb72-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bb72-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7bb72-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bb72-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7bb72-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bb72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bb72-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bb72-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7bb72-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bb72-114">Application</span></span> | <span data-ttu-id="7bb72-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bb72-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bb72-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bb72-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="7bb72-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bb72-117">Request headers</span></span>
| <span data-ttu-id="7bb72-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7bb72-118">Name</span></span>       | <span data-ttu-id="7bb72-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bb72-119">Type</span></span> | <span data-ttu-id="7bb72-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bb72-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7bb72-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bb72-121">Authorization</span></span>  | <span data-ttu-id="7bb72-122">string</span><span class="sxs-lookup"><span data-stu-id="7bb72-122">string</span></span>  | <span data-ttu-id="7bb72-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bb72-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7bb72-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7bb72-125">Content-Type</span></span> | <span data-ttu-id="7bb72-126">string</span><span class="sxs-lookup"><span data-stu-id="7bb72-126">string</span></span>  | <span data-ttu-id="7bb72-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bb72-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bb72-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bb72-129">Request body</span></span>
<span data-ttu-id="7bb72-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7bb72-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7bb72-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7bb72-131">Parameter</span></span>    | <span data-ttu-id="7bb72-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bb72-132">Type</span></span>   |<span data-ttu-id="7bb72-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bb72-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bb72-134">comment</span><span class="sxs-lookup"><span data-stu-id="7bb72-134">comment</span></span>|<span data-ttu-id="7bb72-135">String</span><span class="sxs-lookup"><span data-stu-id="7bb72-135">String</span></span>|<span data-ttu-id="7bb72-p104">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7bb72-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="7bb72-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="7bb72-138">sendResponse</span></span>|<span data-ttu-id="7bb72-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="7bb72-139">Boolean</span></span>|<span data-ttu-id="7bb72-p105">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="7bb72-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="7bb72-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bb72-143">Response</span></span>

<span data-ttu-id="7bb72-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bb72-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bb72-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bb72-146">Example</span></span>
<span data-ttu-id="7bb72-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7bb72-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7bb72-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bb72-148">Request</span></span>
<span data-ttu-id="7bb72-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7bb72-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7bb72-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bb72-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_accept"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/accept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7bb72-151">C#</span><span class="sxs-lookup"><span data-stu-id="7bb72-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-accept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bb72-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="7bb72-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-accept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7bb72-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7bb72-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-accept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7bb72-154">Java</span><span class="sxs-lookup"><span data-stu-id="7bb72-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-accept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7bb72-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bb72-155">Response</span></span>
<span data-ttu-id="7bb72-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bb72-156">Here is an example of the response.</span></span>
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
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
