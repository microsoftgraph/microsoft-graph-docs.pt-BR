---
title: Listar anexos
description: Recupera uma lista de objetos attachment anexados a um evento.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: abdfc3353e5fee94bbcec3b219d2cb6890bab939
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006944"
---
# <a name="list-attachments"></a><span data-ttu-id="bf910-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="bf910-103">List attachments</span></span>

<span data-ttu-id="bf910-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf910-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf910-105">Recupera uma lista de objetos [attachment](../resources/attachment.md) anexados a um evento.</span><span class="sxs-lookup"><span data-stu-id="bf910-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf910-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf910-106">Permissions</span></span>

<span data-ttu-id="bf910-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf910-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf910-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf910-109">Permission type</span></span>      | <span data-ttu-id="bf910-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf910-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf910-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf910-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bf910-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bf910-112">Calendars.Read</span></span>    |
|<span data-ttu-id="bf910-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf910-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf910-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bf910-114">Calendars.Read</span></span>    |
|<span data-ttu-id="bf910-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf910-115">Application</span></span> | <span data-ttu-id="bf910-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bf910-116">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf910-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf910-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="bf910-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bf910-118">Optional query parameters</span></span>

<span data-ttu-id="bf910-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bf910-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="bf910-120">Em particular, você pode usar o `$expand` parâmetro de consulta para incluir todos os anexos de evento embutidos com o restante das propriedades do evento.</span><span class="sxs-lookup"><span data-stu-id="bf910-120">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="bf910-121">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="bf910-121">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="bf910-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf910-122">Request headers</span></span>

| <span data-ttu-id="bf910-123">Nome</span><span class="sxs-lookup"><span data-stu-id="bf910-123">Name</span></span>       | <span data-ttu-id="bf910-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf910-124">Type</span></span> | <span data-ttu-id="bf910-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf910-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bf910-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf910-126">Authorization</span></span>  | <span data-ttu-id="bf910-127">string</span><span class="sxs-lookup"><span data-stu-id="bf910-127">string</span></span>  | <span data-ttu-id="bf910-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf910-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf910-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf910-130">Request body</span></span>

<span data-ttu-id="bf910-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bf910-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf910-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf910-132">Response</span></span>

<span data-ttu-id="bf910-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf910-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf910-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf910-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf910-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf910-135">Request</span></span>

<span data-ttu-id="bf910-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf910-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bf910-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf910-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_get_attachments_beta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="bf910-138">C#</span><span class="sxs-lookup"><span data-stu-id="bf910-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf910-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf910-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf910-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf910-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bf910-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf910-141">Response</span></span>

<span data-ttu-id="bf910-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf910-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "event_get_attachments_beta",
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
      "@odata.type":"#microsoft.graph.fileAttachment",
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
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


