---
title: Listar anexos
description: Recupera uma lista de objetos attachment anexados a um evento.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e324d67cd6e7c57d3a936a0ec6d6e9ace3ec5df0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039584"
---
# <a name="list-attachments"></a><span data-ttu-id="ec097-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="ec097-103">List attachments</span></span>

<span data-ttu-id="ec097-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec097-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ec097-105">Recupera uma lista de objetos [attachment](../resources/attachment.md) anexados a um evento.</span><span class="sxs-lookup"><span data-stu-id="ec097-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec097-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec097-106">Permissions</span></span>
<span data-ttu-id="ec097-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec097-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec097-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec097-109">Permission type</span></span>      | <span data-ttu-id="ec097-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec097-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec097-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec097-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ec097-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ec097-112">Calendars.Read</span></span>    |
|<span data-ttu-id="ec097-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec097-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec097-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ec097-114">Calendars.Read</span></span>    |
|<span data-ttu-id="ec097-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec097-115">Application</span></span> | <span data-ttu-id="ec097-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ec097-116">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec097-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec097-117">HTTP request</span></span>
<span data-ttu-id="ec097-118">Anexos de um [event](../resources/event.md) no [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="ec097-118">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->

<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/attachments
GET /users/{id | userPrincipalName}/events/{id}/attachments

GET /me/calendar/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
GET /groups/{id}/calendar/events/{id}/attachments
-->

<span data-ttu-id="ec097-119">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="ec097-119">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="ec097-120">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ec097-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec097-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ec097-121">Optional query parameters</span></span>
<span data-ttu-id="ec097-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ec097-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ec097-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec097-123">Request headers</span></span>
| <span data-ttu-id="ec097-124">Nome</span><span class="sxs-lookup"><span data-stu-id="ec097-124">Name</span></span>       | <span data-ttu-id="ec097-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec097-125">Type</span></span> | <span data-ttu-id="ec097-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec097-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ec097-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec097-127">Authorization</span></span>  | <span data-ttu-id="ec097-128">string</span><span class="sxs-lookup"><span data-stu-id="ec097-128">string</span></span>  | <span data-ttu-id="ec097-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec097-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec097-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec097-131">Request body</span></span>
<span data-ttu-id="ec097-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ec097-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec097-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec097-133">Response</span></span>

<span data-ttu-id="ec097-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec097-134">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec097-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec097-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec097-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec097-136">Request</span></span>
<span data-ttu-id="ec097-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec097-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ec097-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec097-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_get_attachments_v1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="ec097-139">C#</span><span class="sxs-lookup"><span data-stu-id="ec097-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-attachments-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec097-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec097-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-attachments-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec097-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec097-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-attachments-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec097-142">Java</span><span class="sxs-lookup"><span data-stu-id="ec097-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-get-attachments-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ec097-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec097-143">Response</span></span>
<span data-ttu-id="ec097-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec097-144">Here is an example of the response.</span></span> <span data-ttu-id="ec097-145">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ec097-145">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "event_get_attachments_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
