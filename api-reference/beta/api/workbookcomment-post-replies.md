---
title: Criar workbookCommentReply
description: Crie uma nova workbookCommentReply.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cfa09de241b74bb9bd1a3289791564a9edac5128
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049552"
---
# <a name="create-workbookcommentreply"></a><span data-ttu-id="fc068-103">Criar workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="fc068-103">Create workbookCommentReply</span></span>

<span data-ttu-id="fc068-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc068-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc068-105">Crie um novo [objeto workbookCommentReply.](../resources/workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="fc068-105">Create a new [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc068-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc068-106">Permissions</span></span>

<span data-ttu-id="fc068-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc068-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc068-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc068-109">Permission type</span></span>                        | <span data-ttu-id="fc068-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc068-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fc068-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc068-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc068-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc068-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="fc068-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc068-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc068-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc068-114">Not supported.</span></span> |
| <span data-ttu-id="fc068-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc068-115">Application</span></span>                            | <span data-ttu-id="fc068-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc068-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc068-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc068-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{id}/workbook/comments/{id}/replies
POST /me/drive/root:/{item-path}:/workbook/comments/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="fc068-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc068-118">Request headers</span></span>

| <span data-ttu-id="fc068-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fc068-119">Name</span></span>          | <span data-ttu-id="fc068-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc068-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fc068-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc068-121">Authorization</span></span> | <span data-ttu-id="fc068-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc068-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc068-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc068-124">Request body</span></span>

<span data-ttu-id="fc068-125">No corpo da solicitação, fornece uma representação JSON de um [objeto workbookCommentReply.](../resources/workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="fc068-125">In the request body, supply a JSON representation of a [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fc068-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc068-126">Response</span></span>

<span data-ttu-id="fc068-127">Se tiver êxito, este método retornará um código de resposta e um novo objeto `201 Created` [workbookCommentReply](../resources/workbookcommentreply.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc068-127">If successful, this method returns a `201 Created` response code and a new [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc068-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fc068-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fc068-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc068-129">Request</span></span>

<span data-ttu-id="fc068-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc068-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc068-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc068-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workbookcommentreply_from_workbookcomment"
}-->

```http
POST https://graph.microsoft.com/beta/drive/items/{id}/workbook/comments/{id}/replies
Content-type: application/json

{
  "content": "This is my reply to the comment.",
  "contentType": "plain"
}
```
# <a name="c"></a>[<span data-ttu-id="fc068-132">C#</span><span class="sxs-lookup"><span data-stu-id="fc068-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workbookcommentreply-from-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc068-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc068-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workbookcommentreply-from-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc068-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc068-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workbookcommentreply-from-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc068-135">Java</span><span class="sxs-lookup"><span data-stu-id="fc068-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-workbookcommentreply-from-workbookcomment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fc068-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc068-136">Response</span></span>

<span data-ttu-id="fc068-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc068-137">The following is an example of the response.</span></span>

> <span data-ttu-id="fc068-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fc068-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookCommentReply"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "content": "This is my reply to the comment.",
  "contentType": "plain",
  "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create workbookCommentReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


