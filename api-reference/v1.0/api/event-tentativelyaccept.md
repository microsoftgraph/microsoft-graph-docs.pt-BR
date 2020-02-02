---
title: 'event: tentativelyAccept'
description: Aceitar provisoriamente o evento específico em um calendário de usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 67644ac12f39d15e75609c00b0e7e551e1b7e569
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2020
ms.locfileid: "41652148"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="eaadd-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="eaadd-103">event: tentativelyAccept</span></span>

<span data-ttu-id="eaadd-104">Aceitar provisoriamente o [evento](../resources/event.md) especificado em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="eaadd-104">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eaadd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="eaadd-105">Permissions</span></span>
<span data-ttu-id="eaadd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaadd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaadd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eaadd-108">Permission type</span></span>      | <span data-ttu-id="eaadd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eaadd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eaadd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eaadd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eaadd-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaadd-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="eaadd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eaadd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaadd-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaadd-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="eaadd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eaadd-114">Application</span></span> | <span data-ttu-id="eaadd-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaadd-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eaadd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eaadd-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="eaadd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eaadd-117">Request headers</span></span>
| <span data-ttu-id="eaadd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="eaadd-118">Name</span></span>       | <span data-ttu-id="eaadd-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaadd-119">Type</span></span> | <span data-ttu-id="eaadd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaadd-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eaadd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="eaadd-121">Authorization</span></span>  | <span data-ttu-id="eaadd-122">string</span><span class="sxs-lookup"><span data-stu-id="eaadd-122">string</span></span>  | <span data-ttu-id="eaadd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaadd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eaadd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eaadd-125">Content-Type</span></span> | <span data-ttu-id="eaadd-126">string</span><span class="sxs-lookup"><span data-stu-id="eaadd-126">string</span></span>  | <span data-ttu-id="eaadd-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaadd-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eaadd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eaadd-129">Request body</span></span>
<span data-ttu-id="eaadd-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eaadd-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eaadd-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="eaadd-131">Parameter</span></span>    | <span data-ttu-id="eaadd-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaadd-132">Type</span></span>   |<span data-ttu-id="eaadd-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaadd-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eaadd-134">comment</span><span class="sxs-lookup"><span data-stu-id="eaadd-134">comment</span></span>|<span data-ttu-id="eaadd-135">String</span><span class="sxs-lookup"><span data-stu-id="eaadd-135">String</span></span>|<span data-ttu-id="eaadd-p104">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="eaadd-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="eaadd-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="eaadd-138">sendResponse</span></span>|<span data-ttu-id="eaadd-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="eaadd-139">Boolean</span></span>|<span data-ttu-id="eaadd-p105">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="eaadd-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="eaadd-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaadd-143">Response</span></span>

<span data-ttu-id="eaadd-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eaadd-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaadd-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eaadd-146">Example</span></span>
<span data-ttu-id="eaadd-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="eaadd-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eaadd-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eaadd-148">Request</span></span>
<span data-ttu-id="eaadd-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eaadd-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="eaadd-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="eaadd-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="eaadd-151">C#</span><span class="sxs-lookup"><span data-stu-id="eaadd-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eaadd-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eaadd-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eaadd-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eaadd-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="eaadd-154">Java</span><span class="sxs-lookup"><span data-stu-id="eaadd-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-tentativelyaccept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eaadd-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaadd-155">Response</span></span>
##### <a name="response"></a><span data-ttu-id="eaadd-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaadd-156">Response</span></span>
<span data-ttu-id="eaadd-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eaadd-157">Here is an example of the response.</span></span>
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
