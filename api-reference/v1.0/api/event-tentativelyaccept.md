---
title: 'event: tentativelyAccept'
description: Aceite provisoriamente o evento específico em um calendário do usuário.
author: angelgolfer-ms
ms.openlocfilehash: be22b88c444b3720eaf204bda3246d4b99b90623
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335788"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="47400-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="47400-103">event: tentativelyAccept</span></span>

<span data-ttu-id="47400-104">Aceite provisoriamente o [evento](../resources/event.md) específico em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="47400-104">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="47400-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="47400-105">Permissions</span></span>
<span data-ttu-id="47400-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47400-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47400-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47400-108">Permission type</span></span>      | <span data-ttu-id="47400-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47400-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47400-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47400-110">Delegated (work or school account)</span></span> | <span data-ttu-id="47400-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47400-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="47400-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47400-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47400-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47400-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="47400-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47400-114">Application</span></span> | <span data-ttu-id="47400-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47400-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="47400-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47400-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="47400-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47400-117">Request headers</span></span>
| <span data-ttu-id="47400-118">Nome</span><span class="sxs-lookup"><span data-stu-id="47400-118">Name</span></span>       | <span data-ttu-id="47400-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="47400-119">Type</span></span> | <span data-ttu-id="47400-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="47400-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="47400-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="47400-121">Authorization</span></span>  | <span data-ttu-id="47400-122">string</span><span class="sxs-lookup"><span data-stu-id="47400-122">string</span></span>  | <span data-ttu-id="47400-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47400-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47400-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47400-125">Content-Type</span></span> | <span data-ttu-id="47400-126">string</span><span class="sxs-lookup"><span data-stu-id="47400-126">string</span></span>  | <span data-ttu-id="47400-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47400-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47400-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47400-129">Request body</span></span>
<span data-ttu-id="47400-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47400-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="47400-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="47400-131">Parameter</span></span>    | <span data-ttu-id="47400-132">Type</span><span class="sxs-lookup"><span data-stu-id="47400-132">Type</span></span>   |<span data-ttu-id="47400-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="47400-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47400-134">comment</span><span class="sxs-lookup"><span data-stu-id="47400-134">comment</span></span>|<span data-ttu-id="47400-135">String</span><span class="sxs-lookup"><span data-stu-id="47400-135">String</span></span>|<span data-ttu-id="47400-p104">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="47400-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="47400-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="47400-138">sendResponse</span></span>|<span data-ttu-id="47400-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="47400-139">Boolean</span></span>|<span data-ttu-id="47400-p105">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="47400-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="47400-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="47400-143">Response</span></span>

<span data-ttu-id="47400-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47400-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47400-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47400-146">Example</span></span>
<span data-ttu-id="47400-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="47400-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="47400-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47400-148">Request</span></span>
<span data-ttu-id="47400-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47400-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="47400-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="47400-150">Response</span></span>
##### <a name="response"></a><span data-ttu-id="47400-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="47400-151">Response</span></span>
<span data-ttu-id="47400-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47400-152">Here is an example of the response.</span></span>
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
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
