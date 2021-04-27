---
title: Listar anexos
description: Recupera uma lista de objetos attachment anexados a um evento.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: acfcbd41c07cd9e308e6ad1d705c8590298e04f3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042552"
---
# <a name="list-attachments"></a><span data-ttu-id="e9a79-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="e9a79-103">List attachments</span></span>

<span data-ttu-id="e9a79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9a79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9a79-105">Recupera uma lista de objetos [attachment](../resources/attachment.md) anexados a um evento.</span><span class="sxs-lookup"><span data-stu-id="e9a79-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9a79-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9a79-106">Permissions</span></span>

<span data-ttu-id="e9a79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9a79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9a79-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9a79-109">Permission type</span></span>      | <span data-ttu-id="e9a79-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9a79-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9a79-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9a79-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e9a79-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e9a79-112">Calendars.Read</span></span>    |
|<span data-ttu-id="e9a79-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9a79-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9a79-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e9a79-114">Calendars.Read</span></span>    |
|<span data-ttu-id="e9a79-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9a79-115">Application</span></span> | <span data-ttu-id="e9a79-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e9a79-116">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9a79-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9a79-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="e9a79-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9a79-118">Optional query parameters</span></span>

<span data-ttu-id="e9a79-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9a79-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="e9a79-120">Em particular, você pode usar o parâmetro de consulta para incluir todos os anexos de evento em linha com o `$expand` restante das propriedades do evento.</span><span class="sxs-lookup"><span data-stu-id="e9a79-120">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="e9a79-121">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="e9a79-121">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="e9a79-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a79-122">Request headers</span></span>

| <span data-ttu-id="e9a79-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e9a79-123">Name</span></span>       | <span data-ttu-id="e9a79-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9a79-124">Type</span></span> | <span data-ttu-id="e9a79-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9a79-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e9a79-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9a79-126">Authorization</span></span>  | <span data-ttu-id="e9a79-127">string</span><span class="sxs-lookup"><span data-stu-id="e9a79-127">string</span></span>  | <span data-ttu-id="e9a79-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9a79-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9a79-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a79-130">Request body</span></span>

<span data-ttu-id="e9a79-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9a79-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9a79-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9a79-132">Response</span></span>

<span data-ttu-id="e9a79-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9a79-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9a79-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9a79-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9a79-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a79-135">Request</span></span>

<span data-ttu-id="e9a79-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9a79-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9a79-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9a79-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_get_attachments_beta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="e9a79-138">C#</span><span class="sxs-lookup"><span data-stu-id="e9a79-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9a79-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9a79-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9a79-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9a79-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9a79-141">Java</span><span class="sxs-lookup"><span data-stu-id="e9a79-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-get-attachments-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e9a79-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9a79-142">Response</span></span>

<span data-ttu-id="e9a79-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9a79-143">Here is an example of the response.</span></span> <span data-ttu-id="e9a79-144">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e9a79-144">Note: The response object shown here might be shortened for readability.</span></span>
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
