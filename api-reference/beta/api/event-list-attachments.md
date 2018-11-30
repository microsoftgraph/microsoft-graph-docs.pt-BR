---
title: Listar anexos
description: Recupera uma lista de objetos attachment anexados a um evento.
ms.openlocfilehash: cc632ab14bf2c64628cdf5177da5601f4b04f4d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034643"
---
# <a name="list-attachments"></a><span data-ttu-id="5ca56-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="5ca56-103">List attachments</span></span>

> <span data-ttu-id="5ca56-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5ca56-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ca56-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5ca56-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5ca56-106">Recupera uma lista de objetos [attachment](../resources/attachment.md) anexados a um evento.</span><span class="sxs-lookup"><span data-stu-id="5ca56-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ca56-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ca56-107">Permissions</span></span>
<span data-ttu-id="5ca56-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ca56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ca56-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ca56-110">Permission type</span></span>      | <span data-ttu-id="5ca56-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ca56-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ca56-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ca56-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5ca56-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5ca56-113">Calendars.Read</span></span>    |
|<span data-ttu-id="5ca56-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ca56-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ca56-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5ca56-115">Calendars.Read</span></span>    |
|<span data-ttu-id="5ca56-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ca56-116">Application</span></span> | <span data-ttu-id="5ca56-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5ca56-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ca56-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ca56-118">HTTP request</span></span>
<span data-ttu-id="5ca56-119">Anexos em um [evento](../resources/event.md) do usuário padrão [calendário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="5ca56-119">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="5ca56-120">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ca56-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

GET /me/calendargroup/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="5ca56-121">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5ca56-121">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5ca56-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5ca56-122">Optional query parameters</span></span>
<span data-ttu-id="5ca56-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ca56-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="5ca56-124">Em particular, você pode usar o $expandir o parâmetro de consulta para incluir todos os o embutido de anexos de evento com o restante das propriedades do evento.</span><span class="sxs-lookup"><span data-stu-id="5ca56-124">In particular, you can use the $expand query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="5ca56-125">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="5ca56-125">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```


## <a name="request-headers"></a><span data-ttu-id="5ca56-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca56-126">Request headers</span></span>
| <span data-ttu-id="5ca56-127">Nome</span><span class="sxs-lookup"><span data-stu-id="5ca56-127">Name</span></span>       | <span data-ttu-id="5ca56-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ca56-128">Type</span></span> | <span data-ttu-id="5ca56-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ca56-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5ca56-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ca56-130">Authorization</span></span>  | <span data-ttu-id="5ca56-131">string</span><span class="sxs-lookup"><span data-stu-id="5ca56-131">string</span></span>  | <span data-ttu-id="5ca56-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ca56-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ca56-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca56-134">Request body</span></span>
<span data-ttu-id="5ca56-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ca56-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ca56-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca56-136">Response</span></span>

<span data-ttu-id="5ca56-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ca56-137">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ca56-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ca56-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ca56-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca56-139">Request</span></span>
<span data-ttu-id="5ca56-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ca56-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="5ca56-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca56-141">Response</span></span>
<span data-ttu-id="5ca56-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ca56-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
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
  "tocPath": ""
}-->