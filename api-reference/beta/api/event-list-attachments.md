---
title: Listar anexos
description: Recupera uma lista de objetos attachment anexados a um evento.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1fbbd07817d2a60faef08757907947dccf32a162
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441020"
---
# <a name="list-attachments"></a><span data-ttu-id="11194-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="11194-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11194-104">Recupera uma lista de objetos [attachment](../resources/attachment.md) anexados a um evento.</span><span class="sxs-lookup"><span data-stu-id="11194-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="11194-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="11194-105">Permissions</span></span>

<span data-ttu-id="11194-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11194-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11194-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11194-108">Permission type</span></span>      | <span data-ttu-id="11194-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11194-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11194-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11194-110">Delegated (work or school account)</span></span> | <span data-ttu-id="11194-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="11194-111">Calendars.Read</span></span>    |
|<span data-ttu-id="11194-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11194-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11194-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="11194-113">Calendars.Read</span></span>    |
|<span data-ttu-id="11194-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11194-114">Application</span></span> | <span data-ttu-id="11194-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="11194-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="11194-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11194-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="11194-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="11194-117">Optional query parameters</span></span>

<span data-ttu-id="11194-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="11194-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="11194-119">Em particular, você pode usar o `$expand` parâmetro de consulta para incluir todos os anexos de evento embutidos com o restante das propriedades do evento.</span><span class="sxs-lookup"><span data-stu-id="11194-119">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="11194-120">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="11194-120">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="11194-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11194-121">Request headers</span></span>

| <span data-ttu-id="11194-122">Nome</span><span class="sxs-lookup"><span data-stu-id="11194-122">Name</span></span>       | <span data-ttu-id="11194-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="11194-123">Type</span></span> | <span data-ttu-id="11194-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="11194-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="11194-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="11194-125">Authorization</span></span>  | <span data-ttu-id="11194-126">string</span><span class="sxs-lookup"><span data-stu-id="11194-126">string</span></span>  | <span data-ttu-id="11194-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11194-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11194-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11194-129">Request body</span></span>

<span data-ttu-id="11194-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11194-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11194-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="11194-131">Response</span></span>

<span data-ttu-id="11194-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11194-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11194-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11194-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="11194-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11194-134">Request</span></span>

<span data-ttu-id="11194-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11194-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="11194-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="11194-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="11194-137">C#</span><span class="sxs-lookup"><span data-stu-id="11194-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11194-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="11194-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="11194-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="11194-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11194-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="11194-140">Response</span></span>

<span data-ttu-id="11194-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11194-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
