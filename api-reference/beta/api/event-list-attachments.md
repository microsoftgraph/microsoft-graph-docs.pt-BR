---
title: Listar anexos
description: Recupera uma lista de objetos attachment anexados a um evento.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e0c9563fa0408cd4e699e34e7a169a19deae6839
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461026"
---
# <a name="list-attachments"></a><span data-ttu-id="e8b35-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="e8b35-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8b35-104">Recupera uma lista de objetos [attachment](../resources/attachment.md) anexados a um evento.</span><span class="sxs-lookup"><span data-stu-id="e8b35-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8b35-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8b35-105">Permissions</span></span>

<span data-ttu-id="e8b35-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8b35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8b35-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8b35-108">Permission type</span></span>      | <span data-ttu-id="e8b35-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8b35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8b35-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8b35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8b35-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e8b35-111">Calendars.Read</span></span>    |
|<span data-ttu-id="e8b35-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8b35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8b35-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e8b35-113">Calendars.Read</span></span>    |
|<span data-ttu-id="e8b35-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8b35-114">Application</span></span> | <span data-ttu-id="e8b35-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e8b35-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8b35-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8b35-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="e8b35-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8b35-117">Optional query parameters</span></span>

<span data-ttu-id="e8b35-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8b35-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e8b35-119">Em particular, você pode usar o `$expand` parâmetro de consulta para incluir todos os anexos de evento embutidos com o restante das propriedades do evento.</span><span class="sxs-lookup"><span data-stu-id="e8b35-119">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="e8b35-120">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="e8b35-120">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="e8b35-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8b35-121">Request headers</span></span>

| <span data-ttu-id="e8b35-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e8b35-122">Name</span></span>       | <span data-ttu-id="e8b35-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8b35-123">Type</span></span> | <span data-ttu-id="e8b35-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8b35-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e8b35-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8b35-125">Authorization</span></span>  | <span data-ttu-id="e8b35-126">string</span><span class="sxs-lookup"><span data-stu-id="e8b35-126">string</span></span>  | <span data-ttu-id="e8b35-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8b35-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8b35-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8b35-129">Request body</span></span>

<span data-ttu-id="e8b35-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8b35-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8b35-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8b35-131">Response</span></span>

<span data-ttu-id="e8b35-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8b35-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8b35-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8b35-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8b35-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8b35-134">Request</span></span>

<span data-ttu-id="e8b35-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8b35-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e8b35-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8b35-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_get_attachments_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e8b35-137">C#</span><span class="sxs-lookup"><span data-stu-id="e8b35-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8b35-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8b35-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e8b35-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e8b35-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8b35-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8b35-140">Response</span></span>

<span data-ttu-id="e8b35-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8b35-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
