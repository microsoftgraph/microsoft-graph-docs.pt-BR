---
title: Listar anexos
description: Recupere uma lista de objetos attachment anexados a uma postagem.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2150f50d228dc0567152d5ccf233a76f71176d47
ms.sourcegitcommit: 36066afdced00f32838a03747d3e7760fc43683a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36453105"
---
# <a name="list-attachments"></a><span data-ttu-id="64c3e-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="64c3e-103">List attachments</span></span>

<span data-ttu-id="64c3e-104">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="64c3e-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="64c3e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="64c3e-105">Permissions</span></span>
<span data-ttu-id="64c3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64c3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64c3e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64c3e-108">Permission type</span></span>      | <span data-ttu-id="64c3e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64c3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64c3e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64c3e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="64c3e-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64c3e-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="64c3e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64c3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64c3e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64c3e-113">Not supported.</span></span>    |
|<span data-ttu-id="64c3e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64c3e-114">Application</span></span> | <span data-ttu-id="64c3e-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64c3e-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64c3e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64c3e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="64c3e-117">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="64c3e-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="64c3e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="64c3e-118">Optional query parameters</span></span>
<span data-ttu-id="64c3e-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="64c3e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="64c3e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64c3e-120">Request headers</span></span>
| <span data-ttu-id="64c3e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64c3e-121">Header</span></span>       | <span data-ttu-id="64c3e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="64c3e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64c3e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="64c3e-123">Authorization</span></span>  | <span data-ttu-id="64c3e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64c3e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64c3e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64c3e-126">Request body</span></span>
<span data-ttu-id="64c3e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64c3e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64c3e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="64c3e-128">Response</span></span>

<span data-ttu-id="64c3e-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64c3e-129">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="64c3e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64c3e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64c3e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64c3e-131">Request</span></span>
<span data-ttu-id="64c3e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64c3e-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="64c3e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="64c3e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_get_attachments_v1"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="64c3e-134">C#</span><span class="sxs-lookup"><span data-stu-id="64c3e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64c3e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64c3e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="64c3e-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="64c3e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="64c3e-137">Java</span><span class="sxs-lookup"><span data-stu-id="64c3e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="64c3e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="64c3e-138">Response</span></span>
<span data-ttu-id="64c3e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64c3e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "post_get_attachments_v1",
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
      "@odata.type": "microsoft.graph.fileAttachment",
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "isInline": false,
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
