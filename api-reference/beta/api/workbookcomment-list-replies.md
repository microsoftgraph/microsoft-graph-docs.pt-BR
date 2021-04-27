---
title: Listar workbookCommentReplies
description: Recupere uma lista de objetos workbookCommentReplies.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0c3e96d13266b294f51105bbdd4437cb526f3a33
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049559"
---
# <a name="list-workbookcommentreplies"></a><span data-ttu-id="2e56c-103">Listar workbookCommentReplies</span><span class="sxs-lookup"><span data-stu-id="2e56c-103">List workbookCommentReplies</span></span>

<span data-ttu-id="2e56c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e56c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e56c-105">Recupere uma lista [de objetos workbookCommentReply.](../resources/workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="2e56c-105">Retrieve a list of [workbookCommentReply](../resources/workbookcommentreply.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e56c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e56c-106">Permissions</span></span>

<span data-ttu-id="2e56c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e56c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e56c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e56c-109">Permission type</span></span>                        | <span data-ttu-id="2e56c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e56c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2e56c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e56c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e56c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e56c-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="2e56c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e56c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e56c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e56c-114">Not supported.</span></span> |
| <span data-ttu-id="2e56c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e56c-115">Application</span></span>                            | <span data-ttu-id="2e56c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e56c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e56c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e56c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/items/{id}/workbook/comments/{id}/replies
GET /me/drive/root:/{item-path}:/workbook/comments/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="2e56c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e56c-118">Request headers</span></span>

| <span data-ttu-id="2e56c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2e56c-119">Name</span></span>      |<span data-ttu-id="2e56c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e56c-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2e56c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e56c-121">Authorization</span></span> | <span data-ttu-id="2e56c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e56c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e56c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e56c-124">Request body</span></span>

<span data-ttu-id="2e56c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e56c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e56c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e56c-126">Response</span></span>

<span data-ttu-id="2e56c-127">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [workbookCommentReply](../resources/workbookcommentreply.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e56c-127">If successful, this method returns a `200 OK` response code and a collection of [workbookCommentReply](../resources/workbookcommentreply.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e56c-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2e56c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e56c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e56c-129">Request</span></span>

<span data-ttu-id="2e56c-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e56c-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e56c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e56c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{id}/workbook/comments/{id}/replies
```
# <a name="c"></a>[<span data-ttu-id="2e56c-132">C#</span><span class="sxs-lookup"><span data-stu-id="2e56c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e56c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e56c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e56c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e56c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e56c-135">Java</span><span class="sxs-lookup"><span data-stu-id="2e56c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-replies-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2e56c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e56c-136">Response</span></span>

<span data-ttu-id="2e56c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2e56c-137">The following is an example of the response.</span></span>

> <span data-ttu-id="2e56c-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2e56c-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookCommentReply",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "content": "This is the first piece of reply.",
      "contentType": "plain",
      "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}" 
    },
    {
      "content": "This is the second piece of reply.",
      "contentType": "plain",
      "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFF9}"
     }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


