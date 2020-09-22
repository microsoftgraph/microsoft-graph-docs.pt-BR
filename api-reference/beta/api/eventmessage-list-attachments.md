---
title: Listar anexos
description: Recupera uma lista de objetos de anexo.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8934b31afee84ddcc45126ed7d18e13e7a445a9f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980901"
---
# <a name="list-attachments"></a><span data-ttu-id="15edc-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="15edc-103">List attachments</span></span>

<span data-ttu-id="15edc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15edc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15edc-105">Recupera uma lista de objetos de anexo.</span><span class="sxs-lookup"><span data-stu-id="15edc-105">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="15edc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="15edc-106">Permissions</span></span>
<span data-ttu-id="15edc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15edc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15edc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15edc-109">Permission type</span></span>      | <span data-ttu-id="15edc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15edc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15edc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15edc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="15edc-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="15edc-112">Mail.Read</span></span>    |
|<span data-ttu-id="15edc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15edc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15edc-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="15edc-114">Mail.Read</span></span>    |
|<span data-ttu-id="15edc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15edc-115">Application</span></span> | <span data-ttu-id="15edc-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="15edc-116">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="15edc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15edc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="15edc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="15edc-118">Optional query parameters</span></span>
<span data-ttu-id="15edc-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="15edc-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15edc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15edc-120">Request headers</span></span>
| <span data-ttu-id="15edc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="15edc-121">Name</span></span>       | <span data-ttu-id="15edc-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="15edc-122">Type</span></span> | <span data-ttu-id="15edc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="15edc-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="15edc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="15edc-124">Authorization</span></span>  | <span data-ttu-id="15edc-125">string</span><span class="sxs-lookup"><span data-stu-id="15edc-125">string</span></span>  | <span data-ttu-id="15edc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15edc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15edc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15edc-128">Request body</span></span>
<span data-ttu-id="15edc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15edc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15edc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="15edc-130">Response</span></span>

<span data-ttu-id="15edc-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15edc-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15edc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15edc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15edc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15edc-133">Request</span></span>
<span data-ttu-id="15edc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15edc-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="15edc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="15edc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "eventmessage_get_attachments_beta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="15edc-136">C#</span><span class="sxs-lookup"><span data-stu-id="15edc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/eventmessage-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15edc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15edc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/eventmessage-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15edc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15edc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/eventmessage-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="15edc-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="15edc-139">Response</span></span>
<span data-ttu-id="15edc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15edc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "eventmessage_get_attachments_beta",
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


