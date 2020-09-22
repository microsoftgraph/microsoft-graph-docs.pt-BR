---
title: Obter workbookCommentReply
description: Recupere as propriedades e os relacionamentos do objeto workbookcommentreply.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2c6727cd0500b9ece8a84cff5a2b42e64ee5dda7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970702"
---
# <a name="get-workbookcommentreply"></a><span data-ttu-id="35404-103">Obter workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="35404-103">Get workbookCommentReply</span></span>

<span data-ttu-id="35404-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35404-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35404-105">Recupere as propriedades e os relacionamentos do objeto [workbookCommentReply](../resources/workbookcommentreply.md) .</span><span class="sxs-lookup"><span data-stu-id="35404-105">Retrieve the properties and relationships of [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="35404-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="35404-106">Permissions</span></span>

<span data-ttu-id="35404-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35404-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35404-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35404-109">Permission type</span></span>                        | <span data-ttu-id="35404-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35404-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="35404-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35404-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="35404-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35404-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="35404-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35404-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35404-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35404-114">Not supported.</span></span> |
| <span data-ttu-id="35404-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35404-115">Application</span></span>                            | <span data-ttu-id="35404-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35404-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="35404-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35404-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /workbook/comments/{id}/replies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="35404-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35404-118">Request headers</span></span>

| <span data-ttu-id="35404-119">Nome</span><span class="sxs-lookup"><span data-stu-id="35404-119">Name</span></span>      |<span data-ttu-id="35404-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="35404-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="35404-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="35404-121">Authorization</span></span> | <span data-ttu-id="35404-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35404-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35404-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35404-124">Request body</span></span>

<span data-ttu-id="35404-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="35404-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35404-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="35404-126">Response</span></span>

<span data-ttu-id="35404-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [workbookCommentReply](../resources/workbookcommentreply.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35404-127">If successful, this method returns a `200 OK` response code and the requested [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="35404-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="35404-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35404-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35404-129">Request</span></span>

<span data-ttu-id="35404-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="35404-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="35404-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="35404-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookcommentreply"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drive/items/{id}/workbook/comments/{id}/replies/{id}
```
# <a name="c"></a>[<span data-ttu-id="35404-132">C#</span><span class="sxs-lookup"><span data-stu-id="35404-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookcommentreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35404-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35404-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookcommentreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35404-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35404-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookcommentreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35404-135">Java</span><span class="sxs-lookup"><span data-stu-id="35404-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookcommentreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="35404-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="35404-136">Response</span></span>

<span data-ttu-id="35404-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="35404-137">The following is an example of the response.</span></span>

> <span data-ttu-id="35404-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35404-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookCommentReply"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "content": "This is text of comment.",
  "contentType": "Plain",
  "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workbookCommentReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

