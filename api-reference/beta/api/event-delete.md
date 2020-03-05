---
title: Excluir evento
description: Exclua um evento.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d426d69b42c0f75b2e52abf8a835f3deb170c778
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42423249"
---
# <a name="delete-event"></a><span data-ttu-id="81d94-103">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="81d94-103">Delete event</span></span>

<span data-ttu-id="81d94-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="81d94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81d94-105">Exclua um evento.</span><span class="sxs-lookup"><span data-stu-id="81d94-105">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="81d94-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="81d94-106">Permissions</span></span>
<span data-ttu-id="81d94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81d94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81d94-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81d94-109">Permission type</span></span>      | <span data-ttu-id="81d94-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81d94-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81d94-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81d94-111">Delegated (work or school account)</span></span> | <span data-ttu-id="81d94-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81d94-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="81d94-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81d94-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81d94-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81d94-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="81d94-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81d94-115">Application</span></span> | <span data-ttu-id="81d94-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81d94-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="81d94-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81d94-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}
DELETE /users/{id | userPrincipalName}/events/{id}
DELETE /groups/{id}/events/{id}

DELETE /me/calendar/events/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}
DELETE /groups/{id}/calendar/events/{id}/

DELETE /me/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="81d94-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81d94-118">Request headers</span></span>
| <span data-ttu-id="81d94-119">Nome</span><span class="sxs-lookup"><span data-stu-id="81d94-119">Name</span></span>       | <span data-ttu-id="81d94-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="81d94-120">Type</span></span> | <span data-ttu-id="81d94-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="81d94-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="81d94-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="81d94-122">Authorization</span></span>  | <span data-ttu-id="81d94-123">string</span><span class="sxs-lookup"><span data-stu-id="81d94-123">string</span></span>  | <span data-ttu-id="81d94-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81d94-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81d94-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81d94-126">Request body</span></span>
<span data-ttu-id="81d94-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81d94-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81d94-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="81d94-128">Response</span></span>

<span data-ttu-id="81d94-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81d94-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81d94-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81d94-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81d94-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81d94-132">Request</span></span>
<span data-ttu-id="81d94-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81d94-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="81d94-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="81d94-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}
```
# <a name="c"></a>[<span data-ttu-id="81d94-135">C#</span><span class="sxs-lookup"><span data-stu-id="81d94-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81d94-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81d94-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81d94-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81d94-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="81d94-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="81d94-138">Response</span></span>
<span data-ttu-id="81d94-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81d94-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
