---
title: Listar anexos
description: Recupere uma lista de objetos attachment anexados a uma postagem.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 581080cb2177e13df8518958a1a6b312d7d7aeaa
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053920"
---
# <a name="list-attachments"></a><span data-ttu-id="52996-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="52996-103">List attachments</span></span>

<span data-ttu-id="52996-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52996-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52996-105">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="52996-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="52996-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="52996-106">Permissions</span></span>
<span data-ttu-id="52996-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52996-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52996-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52996-109">Permission type</span></span>      | <span data-ttu-id="52996-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52996-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52996-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52996-111">Delegated (work or school account)</span></span> | <span data-ttu-id="52996-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52996-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="52996-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52996-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52996-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52996-114">Not supported.</span></span>    |
|<span data-ttu-id="52996-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52996-115">Application</span></span> | <span data-ttu-id="52996-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52996-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52996-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52996-117">HTTP request</span></span>
<span data-ttu-id="52996-118">Obter os anexos de uma [postagem](../resources/post.md) em [uma conversaThread](../resources/conversationthread.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="52996-118">Get the attachments for a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="52996-119">Especificar a conversa [pai](../resources/conversation.md) é opcional.</span><span class="sxs-lookup"><span data-stu-id="52996-119">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="52996-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="52996-120">Optional query parameters</span></span>
<span data-ttu-id="52996-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="52996-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="52996-122">Em particular, você pode usar o parâmetro $expand de consulta para incluir todos os anexos de postagem em linha com o restante das propriedades de postagem.</span><span class="sxs-lookup"><span data-stu-id="52996-122">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="52996-123">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="52996-123">For example:</span></span>

<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="52996-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52996-124">Request headers</span></span>
| <span data-ttu-id="52996-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52996-125">Header</span></span>       | <span data-ttu-id="52996-126">Valor</span><span class="sxs-lookup"><span data-stu-id="52996-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="52996-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="52996-127">Authorization</span></span>  | <span data-ttu-id="52996-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52996-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="52996-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52996-130">Request body</span></span>
<span data-ttu-id="52996-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52996-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52996-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="52996-132">Response</span></span>

<span data-ttu-id="52996-133">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [anexos](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52996-133">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52996-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52996-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52996-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52996-135">Request</span></span>
<span data-ttu-id="52996-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52996-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52996-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="52996-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_get_attachments_v1",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJfolA==","AAMkADJ-aHAAA="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJfolA==/posts/AAMkADJ-aHAAA=/attachments
```
# <a name="c"></a>[<span data-ttu-id="52996-138">C#</span><span class="sxs-lookup"><span data-stu-id="52996-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-get-attachments-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52996-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52996-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-get-attachments-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52996-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52996-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-get-attachments-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52996-141">Java</span><span class="sxs-lookup"><span data-stu-id="52996-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-get-attachments-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="52996-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="52996-142">Response</span></span>
<span data-ttu-id="52996-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52996-143">Here is an example of the response.</span></span> <span data-ttu-id="52996-144">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52996-144">Note: The response object shown here might be shortened for readability.</span></span>
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

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('1848753d-185d-4c08-a4e4-6ee40521d115')/threads('AAQkADJfolA%3D%3D')/posts('AAMkADJ-aHAAA%3D')/attachments",
    "value": [
        {
            "@odata.type": "#microsoft.graph.fileAttachment",
            "id": "AAMkADJ-aHAAABEgAQAO5ZYuLGBmNFnelXXQqAN6I=",
            "lastModifiedDateTime": "2019-08-23T01:53:41Z",
            "name": "FileAsAttachment.txt",
            "contentType": "text/plain",
            "size": 244,
            "isInline": false,
            "contentId": null,
            "contentLocation": null,
            "contentBytes": "VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu"
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
