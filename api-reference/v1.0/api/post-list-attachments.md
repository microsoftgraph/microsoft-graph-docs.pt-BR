---
title: Listar anexos
description: Recupere uma lista de objetos attachment anexados a uma postagem.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a7ca9f0470e5ea97f7c0737087b6db282c90b740
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275163"
---
# <a name="list-attachments"></a><span data-ttu-id="27304-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="27304-103">List attachments</span></span>

<span data-ttu-id="27304-104">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="27304-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="27304-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="27304-105">Permissions</span></span>
<span data-ttu-id="27304-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27304-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27304-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27304-108">Permission type</span></span>      | <span data-ttu-id="27304-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27304-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27304-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27304-110">Delegated (work or school account)</span></span> | <span data-ttu-id="27304-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27304-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="27304-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27304-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27304-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27304-113">Not supported.</span></span>    |
|<span data-ttu-id="27304-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27304-114">Application</span></span> | <span data-ttu-id="27304-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27304-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27304-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27304-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="27304-117">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="27304-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="27304-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="27304-118">Optional query parameters</span></span>
<span data-ttu-id="27304-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="27304-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="27304-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27304-120">Request headers</span></span>
| <span data-ttu-id="27304-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27304-121">Header</span></span>       | <span data-ttu-id="27304-122">Valor</span><span class="sxs-lookup"><span data-stu-id="27304-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="27304-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="27304-123">Authorization</span></span>  | <span data-ttu-id="27304-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27304-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27304-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27304-126">Request body</span></span>
<span data-ttu-id="27304-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27304-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27304-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="27304-128">Response</span></span>

<span data-ttu-id="27304-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27304-129">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27304-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27304-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27304-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27304-131">Request</span></span>
<span data-ttu-id="27304-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27304-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="27304-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="27304-133">Response</span></span>
<span data-ttu-id="27304-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27304-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="27304-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="27304-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="27304-138">C#</span><span class="sxs-lookup"><span data-stu-id="27304-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_attachments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27304-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="27304-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_attachments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="27304-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="27304-140">Objective-C</span></span>](#tab/objective-c)
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
    "Error: /api-reference/v1.0/api/post-list-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/post-list-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/post-list-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
