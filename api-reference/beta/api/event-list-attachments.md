---
title: Listar anexos
description: Recupera uma lista de objetos attachment anexados a um evento.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cf092595f558d3aa1529023029ce84c6f2a4cb87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463954"
---
# <a name="list-attachments"></a><span data-ttu-id="e8fdd-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="e8fdd-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8fdd-104">Recupera uma lista de objetos [attachment](../resources/attachment.md) anexados a um evento.</span><span class="sxs-lookup"><span data-stu-id="e8fdd-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8fdd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8fdd-105">Permissions</span></span>

<span data-ttu-id="e8fdd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8fdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8fdd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8fdd-108">Permission type</span></span>      | <span data-ttu-id="e8fdd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8fdd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8fdd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8fdd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8fdd-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e8fdd-111">Calendars.Read</span></span>    |
|<span data-ttu-id="e8fdd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8fdd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8fdd-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e8fdd-113">Calendars.Read</span></span>    |
|<span data-ttu-id="e8fdd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8fdd-114">Application</span></span> | <span data-ttu-id="e8fdd-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e8fdd-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8fdd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8fdd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="e8fdd-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8fdd-117">Optional query parameters</span></span>

<span data-ttu-id="e8fdd-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8fdd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e8fdd-119">Em particular, você pode usar o `$expand` parâmetro de consulta para incluir todos os anexos de evento embutidos com o restante das propriedades do evento.</span><span class="sxs-lookup"><span data-stu-id="e8fdd-119">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="e8fdd-120">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="e8fdd-120">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="e8fdd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8fdd-121">Request headers</span></span>

| <span data-ttu-id="e8fdd-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e8fdd-122">Name</span></span>       | <span data-ttu-id="e8fdd-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8fdd-123">Type</span></span> | <span data-ttu-id="e8fdd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8fdd-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e8fdd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8fdd-125">Authorization</span></span>  | <span data-ttu-id="e8fdd-126">string</span><span class="sxs-lookup"><span data-stu-id="e8fdd-126">string</span></span>  | <span data-ttu-id="e8fdd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8fdd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8fdd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8fdd-129">Request body</span></span>

<span data-ttu-id="e8fdd-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8fdd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8fdd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8fdd-131">Response</span></span>

<span data-ttu-id="e8fdd-132">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8fdd-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8fdd-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8fdd-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8fdd-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8fdd-134">Request</span></span>

<span data-ttu-id="e8fdd-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8fdd-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="e8fdd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8fdd-136">Response</span></span>

<span data-ttu-id="e8fdd-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8fdd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/event-list-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
