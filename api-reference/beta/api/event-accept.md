---
title: 'event: accept'
description: Aceite o evento específico em um calendário do usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: afff4a9eebb72fa9c624decb55d2677d4c5d41fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894464"
---
# <a name="event-accept"></a><span data-ttu-id="30e8d-103">event: accept</span><span class="sxs-lookup"><span data-stu-id="30e8d-103">event: accept</span></span>

> <span data-ttu-id="30e8d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="30e8d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30e8d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="30e8d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="30e8d-106">Aceite o [evento](../resources/event.md) específico em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="30e8d-106">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="30e8d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="30e8d-107">Permissions</span></span>
<span data-ttu-id="30e8d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30e8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30e8d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30e8d-110">Permission type</span></span>      | <span data-ttu-id="30e8d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30e8d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30e8d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30e8d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="30e8d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30e8d-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="30e8d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30e8d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30e8d-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30e8d-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="30e8d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30e8d-116">Application</span></span> | <span data-ttu-id="30e8d-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30e8d-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="30e8d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30e8d-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="30e8d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30e8d-119">Request headers</span></span>
| <span data-ttu-id="30e8d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="30e8d-120">Name</span></span>       | <span data-ttu-id="30e8d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="30e8d-121">Type</span></span> | <span data-ttu-id="30e8d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="30e8d-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="30e8d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="30e8d-123">Authorization</span></span>  | <span data-ttu-id="30e8d-124">string</span><span class="sxs-lookup"><span data-stu-id="30e8d-124">string</span></span>  | <span data-ttu-id="30e8d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30e8d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="30e8d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="30e8d-127">Content-Type</span></span> | <span data-ttu-id="30e8d-128">string</span><span class="sxs-lookup"><span data-stu-id="30e8d-128">string</span></span>  | <span data-ttu-id="30e8d-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30e8d-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30e8d-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30e8d-131">Request body</span></span>
<span data-ttu-id="30e8d-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30e8d-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="30e8d-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="30e8d-133">Parameter</span></span>    | <span data-ttu-id="30e8d-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="30e8d-134">Type</span></span>   |<span data-ttu-id="30e8d-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="30e8d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30e8d-136">comment</span><span class="sxs-lookup"><span data-stu-id="30e8d-136">comment</span></span>|<span data-ttu-id="30e8d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30e8d-137">String</span></span>|<span data-ttu-id="30e8d-p105">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="30e8d-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="30e8d-140">sendResponse</span><span class="sxs-lookup"><span data-stu-id="30e8d-140">sendResponse</span></span>|<span data-ttu-id="30e8d-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="30e8d-141">Boolean</span></span>|<span data-ttu-id="30e8d-p106">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="30e8d-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="30e8d-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="30e8d-145">Response</span></span>

<span data-ttu-id="30e8d-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30e8d-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30e8d-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30e8d-148">Example</span></span>
<span data-ttu-id="30e8d-149">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="30e8d-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="30e8d-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30e8d-150">Request</span></span>
<span data-ttu-id="30e8d-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30e8d-151">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="30e8d-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="30e8d-152">Response</span></span>
<span data-ttu-id="30e8d-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30e8d-153">Here is an example of the response.</span></span>
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
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
