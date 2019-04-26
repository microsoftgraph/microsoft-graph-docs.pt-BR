---
title: 'event: decline'
description: Recusar o convite para o evento específico em um calendário de usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 920a97db9a6716d2111a8179c86d5556042a6edd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550088"
---
# <a name="event-decline"></a><span data-ttu-id="d5c63-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="d5c63-103">event: decline</span></span>

<span data-ttu-id="d5c63-104">Recusar o convite para o [evento](../resources/event.md) especificado em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="d5c63-104">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5c63-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5c63-105">Permissions</span></span>

<span data-ttu-id="d5c63-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5c63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5c63-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5c63-108">Permission type</span></span>      | <span data-ttu-id="d5c63-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5c63-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5c63-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5c63-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d5c63-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5c63-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d5c63-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5c63-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5c63-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5c63-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d5c63-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5c63-114">Application</span></span> | <span data-ttu-id="d5c63-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5c63-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5c63-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5c63-116">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="d5c63-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c63-117">Request headers</span></span>

| <span data-ttu-id="d5c63-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d5c63-118">Name</span></span>       | <span data-ttu-id="d5c63-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5c63-119">Type</span></span> | <span data-ttu-id="d5c63-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5c63-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d5c63-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5c63-121">Authorization</span></span>  | <span data-ttu-id="d5c63-122">string</span><span class="sxs-lookup"><span data-stu-id="d5c63-122">string</span></span>  | <span data-ttu-id="d5c63-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5c63-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d5c63-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5c63-125">Content-Type</span></span> | <span data-ttu-id="d5c63-126">string</span><span class="sxs-lookup"><span data-stu-id="d5c63-126">string</span></span>  | <span data-ttu-id="d5c63-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5c63-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5c63-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c63-129">Request body</span></span>

<span data-ttu-id="d5c63-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5c63-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d5c63-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d5c63-131">Parameter</span></span>    | <span data-ttu-id="d5c63-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5c63-132">Type</span></span>   |<span data-ttu-id="d5c63-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5c63-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5c63-134">comment</span><span class="sxs-lookup"><span data-stu-id="d5c63-134">comment</span></span>|<span data-ttu-id="d5c63-135">String</span><span class="sxs-lookup"><span data-stu-id="d5c63-135">String</span></span>|<span data-ttu-id="d5c63-p104">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d5c63-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="d5c63-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="d5c63-138">sendResponse</span></span>|<span data-ttu-id="d5c63-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5c63-139">Boolean</span></span>|<span data-ttu-id="d5c63-p105">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="d5c63-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="d5c63-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5c63-143">Response</span></span>

<span data-ttu-id="d5c63-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5c63-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5c63-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5c63-146">Example</span></span>

<span data-ttu-id="d5c63-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d5c63-147">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d5c63-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c63-148">Request</span></span>

<span data-ttu-id="d5c63-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5c63-149">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/decline
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

<br/>

### <a name="response"></a><span data-ttu-id="d5c63-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5c63-150">Response</span></span>

<span data-ttu-id="d5c63-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5c63-151">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
