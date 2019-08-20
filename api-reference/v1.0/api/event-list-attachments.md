---
title: Listar anexos
description: Recupera uma lista de objetos attachment anexados a um evento.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 50cc1490643442fa81011a42317aa39b96b4b8d9
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461697"
---
# <a name="list-attachments"></a><span data-ttu-id="3e137-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="3e137-103">List attachments</span></span>

<span data-ttu-id="3e137-104">Recupera uma lista de objetos [attachment](../resources/attachment.md) anexados a um evento.</span><span class="sxs-lookup"><span data-stu-id="3e137-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e137-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e137-105">Permissions</span></span>
<span data-ttu-id="3e137-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e137-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e137-108">Permission type</span></span>      | <span data-ttu-id="3e137-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e137-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e137-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e137-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3e137-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3e137-111">Calendars.Read</span></span>    |
|<span data-ttu-id="3e137-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e137-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e137-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3e137-113">Calendars.Read</span></span>    |
|<span data-ttu-id="3e137-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e137-114">Application</span></span> | <span data-ttu-id="3e137-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3e137-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e137-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e137-116">HTTP request</span></span>
<span data-ttu-id="3e137-117">Anexos de um [evento](../resources/event.md) no [calendário](../resources/calendar.md)padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="3e137-117">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="3e137-118">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="3e137-118">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

GET /me/calendargroup/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="3e137-119">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="3e137-119">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3e137-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3e137-120">Optional query parameters</span></span>
<span data-ttu-id="3e137-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3e137-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3e137-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e137-122">Request headers</span></span>
| <span data-ttu-id="3e137-123">Nome</span><span class="sxs-lookup"><span data-stu-id="3e137-123">Name</span></span>       | <span data-ttu-id="3e137-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e137-124">Type</span></span> | <span data-ttu-id="3e137-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e137-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3e137-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e137-126">Authorization</span></span>  | <span data-ttu-id="3e137-127">string</span><span class="sxs-lookup"><span data-stu-id="3e137-127">string</span></span>  | <span data-ttu-id="3e137-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e137-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e137-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e137-130">Request body</span></span>
<span data-ttu-id="3e137-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e137-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e137-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e137-132">Response</span></span>

<span data-ttu-id="3e137-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e137-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e137-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e137-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e137-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e137-135">Request</span></span>
<span data-ttu-id="3e137-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e137-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3e137-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e137-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_get_attachments_v1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3e137-138">C#</span><span class="sxs-lookup"><span data-stu-id="3e137-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-attachments-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e137-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e137-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-attachments-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3e137-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3e137-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-attachments-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3e137-141">Java</span><span class="sxs-lookup"><span data-stu-id="3e137-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-get-attachments-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3e137-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e137-142">Response</span></span>
<span data-ttu-id="3e137-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e137-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
