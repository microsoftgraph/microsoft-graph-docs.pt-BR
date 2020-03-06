---
title: Excluir calendário
description: Exclua um calendário que não o calendário padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f39115551e5bd8890e95075245946f48c8a8bc23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518823"
---
# <a name="delete-calendar"></a><span data-ttu-id="444b5-103">Excluir calendário</span><span class="sxs-lookup"><span data-stu-id="444b5-103">Delete calendar</span></span>

<span data-ttu-id="444b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="444b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="444b5-105">Exclua um calendário que não o calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="444b5-105">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="444b5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="444b5-106">Permissions</span></span>
<span data-ttu-id="444b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="444b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="444b5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="444b5-109">Permission type</span></span>      | <span data-ttu-id="444b5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="444b5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="444b5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="444b5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="444b5-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="444b5-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="444b5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="444b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="444b5-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="444b5-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="444b5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="444b5-115">Application</span></span> | <span data-ttu-id="444b5-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="444b5-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="444b5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="444b5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="444b5-118">Um [calendar](../resources/calendar.md) de usuário, que não seja o padrão, no [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="444b5-118">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="444b5-119">Um [calendar](../resources/calendar.md), que não seja o padrão, em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="444b5-119">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="444b5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="444b5-120">Request headers</span></span>
| <span data-ttu-id="444b5-121">Nome</span><span class="sxs-lookup"><span data-stu-id="444b5-121">Name</span></span>           |  <span data-ttu-id="444b5-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="444b5-122">Type</span></span>    | <span data-ttu-id="444b5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="444b5-123">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="444b5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="444b5-124">Authorization</span></span>  |  <span data-ttu-id="444b5-125">string</span><span class="sxs-lookup"><span data-stu-id="444b5-125">string</span></span>  | <span data-ttu-id="444b5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="444b5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="444b5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="444b5-128">Request body</span></span>
<span data-ttu-id="444b5-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="444b5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="444b5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="444b5-130">Response</span></span>

<span data-ttu-id="444b5-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="444b5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="444b5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="444b5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="444b5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="444b5-134">Request</span></span>
<span data-ttu-id="444b5-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="444b5-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="444b5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="444b5-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
# <a name="c"></a>[<span data-ttu-id="444b5-137">C#</span><span class="sxs-lookup"><span data-stu-id="444b5-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="444b5-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="444b5-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="444b5-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="444b5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="444b5-140">Java</span><span class="sxs-lookup"><span data-stu-id="444b5-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="444b5-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="444b5-141">Response</span></span>
<span data-ttu-id="444b5-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="444b5-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
