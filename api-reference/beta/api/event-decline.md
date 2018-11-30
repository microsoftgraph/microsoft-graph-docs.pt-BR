---
title: 'event: decline'
description: Recusar o convite para o evento específico em um calendário do usuário.
ms.openlocfilehash: 7012644f28dd6e1172ba8f71b58d6905fe62c1d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034920"
---
# <a name="event-decline"></a><span data-ttu-id="26143-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="26143-103">event: decline</span></span>

> <span data-ttu-id="26143-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="26143-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26143-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="26143-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="26143-106">Recusar o convite para o [evento](../resources/event.md) específico em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="26143-106">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="26143-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="26143-107">Permissions</span></span>
<span data-ttu-id="26143-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26143-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26143-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26143-110">Permission type</span></span>      | <span data-ttu-id="26143-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26143-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26143-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26143-112">Delegated (work or school account)</span></span> | <span data-ttu-id="26143-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26143-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="26143-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26143-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26143-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26143-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="26143-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26143-116">Application</span></span> | <span data-ttu-id="26143-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26143-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="26143-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26143-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/decline
POST /users/{id | userPrincipalName}/events/{id}/decline

POST /me/calendar/events/{id}/decline
POST /users/{id | userPrincipalName}/calendar/events/{id}/decline

POST /me/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/decline

POST /me/calendargroup/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/decline

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/decline
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="26143-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26143-119">Request headers</span></span>

| <span data-ttu-id="26143-120">Nome</span><span class="sxs-lookup"><span data-stu-id="26143-120">Name</span></span>       | <span data-ttu-id="26143-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="26143-121">Type</span></span> | <span data-ttu-id="26143-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="26143-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26143-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="26143-123">Authorization</span></span>  | <span data-ttu-id="26143-124">string</span><span class="sxs-lookup"><span data-stu-id="26143-124">string</span></span>  | <span data-ttu-id="26143-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26143-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26143-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26143-127">Content-Type</span></span> | <span data-ttu-id="26143-128">string</span><span class="sxs-lookup"><span data-stu-id="26143-128">string</span></span>  | <span data-ttu-id="26143-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26143-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26143-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26143-131">Request body</span></span>

<span data-ttu-id="26143-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26143-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="26143-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="26143-133">Parameter</span></span>    | <span data-ttu-id="26143-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="26143-134">Type</span></span>   |<span data-ttu-id="26143-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="26143-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26143-136">comment</span><span class="sxs-lookup"><span data-stu-id="26143-136">comment</span></span>|<span data-ttu-id="26143-137">String</span><span class="sxs-lookup"><span data-stu-id="26143-137">String</span></span>|<span data-ttu-id="26143-p105">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="26143-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="26143-140">sendResponse</span><span class="sxs-lookup"><span data-stu-id="26143-140">sendResponse</span></span>|<span data-ttu-id="26143-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="26143-141">Boolean</span></span>|<span data-ttu-id="26143-p106">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="26143-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="26143-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="26143-145">Response</span></span>

<span data-ttu-id="26143-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26143-p107">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26143-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26143-148">Example</span></span>

<span data-ttu-id="26143-149">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="26143-149">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="26143-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26143-150">Request</span></span>

<span data-ttu-id="26143-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26143-151">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_decline"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/decline
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

### <a name="response"></a><span data-ttu-id="26143-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="26143-152">Response</span></span>

<span data-ttu-id="26143-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26143-153">Here is an example of the response.</span></span>

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
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
