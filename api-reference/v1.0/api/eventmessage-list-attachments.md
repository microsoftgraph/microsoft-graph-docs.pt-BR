---
title: Listar anexos
description: Recupera uma lista de objetos de anexo.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 385c51f328051a60f18c615a9f32cce8cf498b0c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277403"
---
# <a name="list-attachments"></a><span data-ttu-id="ce341-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="ce341-103">List attachments</span></span>

<span data-ttu-id="ce341-104">Recupera uma lista de objetos de anexo.</span><span class="sxs-lookup"><span data-stu-id="ce341-104">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ce341-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce341-105">Permissions</span></span>
<span data-ttu-id="ce341-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce341-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce341-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce341-108">Permission type</span></span>      | <span data-ttu-id="ce341-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce341-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce341-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce341-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce341-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ce341-111">Mail.Read</span></span>    |
|<span data-ttu-id="ce341-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce341-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce341-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ce341-113">Mail.Read</span></span>    |
|<span data-ttu-id="ce341-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce341-114">Application</span></span> | <span data-ttu-id="ce341-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ce341-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce341-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce341-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ce341-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ce341-117">Optional query parameters</span></span>
<span data-ttu-id="ce341-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ce341-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce341-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce341-119">Request headers</span></span>
| <span data-ttu-id="ce341-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ce341-120">Name</span></span>       | <span data-ttu-id="ce341-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce341-121">Type</span></span> | <span data-ttu-id="ce341-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce341-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ce341-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce341-123">Authorization</span></span>  | <span data-ttu-id="ce341-124">string</span><span class="sxs-lookup"><span data-stu-id="ce341-124">string</span></span>  | <span data-ttu-id="ce341-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce341-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce341-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce341-127">Request body</span></span>
<span data-ttu-id="ce341-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ce341-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce341-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce341-129">Response</span></span>

<span data-ttu-id="ce341-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce341-130">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce341-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce341-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce341-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce341-132">Request</span></span>
<span data-ttu-id="ce341-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce341-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="ce341-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce341-134">Response</span></span>
<span data-ttu-id="ce341-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce341-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
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
      "contentBytes": "base64-contentBytes-value",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ce341-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ce341-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ce341-139">C#</span><span class="sxs-lookup"><span data-stu-id="ce341-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_attachments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce341-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce341-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_attachments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ce341-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ce341-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_attachments-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/eventmessage-list-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/eventmessage-list-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/eventmessage-list-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
