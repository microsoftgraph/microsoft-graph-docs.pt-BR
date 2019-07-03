---
title: Listar anexos
description: Recupere uma lista de objetos attachment anexados a uma postagem.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9b513aa19f4b755c35c8ab158dfec0dc0b3834aa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445139"
---
# <a name="list-attachments"></a><span data-ttu-id="386da-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="386da-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="386da-104">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="386da-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="386da-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="386da-105">Permissions</span></span>
<span data-ttu-id="386da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="386da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="386da-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="386da-108">Permission type</span></span>      | <span data-ttu-id="386da-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="386da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="386da-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="386da-110">Delegated (work or school account)</span></span> | <span data-ttu-id="386da-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="386da-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="386da-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="386da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="386da-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="386da-113">Not supported.</span></span>    |
|<span data-ttu-id="386da-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="386da-114">Application</span></span> | <span data-ttu-id="386da-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="386da-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="386da-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="386da-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="386da-117">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="386da-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="386da-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="386da-118">Optional query parameters</span></span>
<span data-ttu-id="386da-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="386da-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="386da-120">Em particular, você pode usar o $expand parâmetro de consulta para incluir todos os anexos de postagem embutidos com o restante das propriedades post.</span><span class="sxs-lookup"><span data-stu-id="386da-120">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="386da-121">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="386da-121">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="386da-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="386da-122">Request headers</span></span>
| <span data-ttu-id="386da-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="386da-123">Header</span></span>       | <span data-ttu-id="386da-124">Valor</span><span class="sxs-lookup"><span data-stu-id="386da-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="386da-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="386da-125">Authorization</span></span>  | <span data-ttu-id="386da-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="386da-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="386da-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="386da-128">Request body</span></span>
<span data-ttu-id="386da-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="386da-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="386da-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="386da-130">Response</span></span>

<span data-ttu-id="386da-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="386da-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="386da-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="386da-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="386da-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="386da-133">Request</span></span>
<span data-ttu-id="386da-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="386da-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="386da-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="386da-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="386da-136">C#</span><span class="sxs-lookup"><span data-stu-id="386da-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="386da-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="386da-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="386da-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="386da-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="386da-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="386da-139">Response</span></span>
<span data-ttu-id="386da-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="386da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "isInline": false,
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
