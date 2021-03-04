---
title: Excluir calendário
description: Exclua um calendário que não o calendário padrão.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3d8e0b7749d08fc7d0d58c3bfc3adc4f4d9f6110
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437972"
---
# <a name="delete-calendar"></a><span data-ttu-id="4a475-103">Excluir calendário</span><span class="sxs-lookup"><span data-stu-id="4a475-103">Delete calendar</span></span>

<span data-ttu-id="4a475-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a475-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a475-105">Exclua um calendário que não o calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="4a475-105">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a475-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a475-106">Permissions</span></span>
<span data-ttu-id="4a475-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a475-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a475-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a475-109">Permission type</span></span>      | <span data-ttu-id="4a475-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a475-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a475-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a475-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4a475-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a475-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4a475-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a475-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a475-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a475-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4a475-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a475-115">Application</span></span> | <span data-ttu-id="4a475-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a475-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a475-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a475-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="4a475-118">Um [calendar](../resources/calendar.md) de usuário, que não seja o padrão, no [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="4a475-118">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}
```
<span data-ttu-id="4a475-119">Um [calendar](../resources/calendar.md), que não seja o padrão, em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="4a475-119">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4a475-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a475-120">Request headers</span></span>
| <span data-ttu-id="4a475-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4a475-121">Name</span></span>           |  <span data-ttu-id="4a475-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a475-122">Type</span></span>    | <span data-ttu-id="4a475-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a475-123">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="4a475-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a475-124">Authorization</span></span>  |  <span data-ttu-id="4a475-125">string</span><span class="sxs-lookup"><span data-stu-id="4a475-125">string</span></span>  | <span data-ttu-id="4a475-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a475-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a475-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a475-128">Request body</span></span>
<span data-ttu-id="4a475-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a475-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a475-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a475-130">Response</span></span>

<span data-ttu-id="4a475-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a475-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a475-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a475-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a475-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a475-134">Request</span></span>
<span data-ttu-id="4a475-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a475-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a475-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a475-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
# <a name="c"></a>[<span data-ttu-id="4a475-137">C#</span><span class="sxs-lookup"><span data-stu-id="4a475-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a475-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a475-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a475-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a475-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a475-140">Java</span><span class="sxs-lookup"><span data-stu-id="4a475-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4a475-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a475-141">Response</span></span>
<span data-ttu-id="4a475-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a475-142">Here is an example of the response.</span></span> 
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
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


