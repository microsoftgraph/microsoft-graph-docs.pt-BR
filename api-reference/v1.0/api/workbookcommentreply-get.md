---
title: Obter workbookCommentReply
description: Recupere as propriedades e os relacionamentos do objeto workbookcommentreply.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 20ebf0318dd1d66744551ca93fb7cd1ed28a4c27
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539264"
---
# <a name="get-workbookcommentreply"></a><span data-ttu-id="cff6c-103">Obter workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="cff6c-103">Get workbookCommentReply</span></span>

<span data-ttu-id="cff6c-104">Recupere as propriedades e os relacionamentos do objeto [workbookCommentReply](../resources/workbookcommentreply.md) .</span><span class="sxs-lookup"><span data-stu-id="cff6c-104">Retrieve the properties and relationships of [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cff6c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cff6c-105">Permissions</span></span>

<span data-ttu-id="cff6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cff6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cff6c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cff6c-108">Permission type</span></span>                        | <span data-ttu-id="cff6c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cff6c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cff6c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cff6c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cff6c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cff6c-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="cff6c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cff6c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cff6c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cff6c-113">Not supported.</span></span> |
| <span data-ttu-id="cff6c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cff6c-114">Application</span></span>                            | <span data-ttu-id="cff6c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cff6c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cff6c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cff6c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /workbook/comments/{id}/replies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cff6c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cff6c-117">Request headers</span></span>

| <span data-ttu-id="cff6c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="cff6c-118">Name</span></span>      |<span data-ttu-id="cff6c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="cff6c-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cff6c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="cff6c-120">Authorization</span></span> | <span data-ttu-id="cff6c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cff6c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cff6c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cff6c-123">Request body</span></span>

<span data-ttu-id="cff6c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cff6c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cff6c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="cff6c-125">Response</span></span>

<span data-ttu-id="cff6c-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [workbookCommentReply](../resources/workbookcommentreply.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cff6c-126">If successful, this method returns a `200 OK` response code and the requested [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cff6c-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cff6c-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cff6c-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cff6c-128">Request</span></span>

<span data-ttu-id="cff6c-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cff6c-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cff6c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="cff6c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookcommentreply"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drive/root/workbook/comments/{id}/replies/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cff6c-131">C#</span><span class="sxs-lookup"><span data-stu-id="cff6c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookcommentreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cff6c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cff6c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookcommentreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cff6c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cff6c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookcommentreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cff6c-134">Java</span><span class="sxs-lookup"><span data-stu-id="cff6c-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookcommentreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cff6c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cff6c-135">Response</span></span>

<span data-ttu-id="cff6c-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cff6c-136">The following is an example of the response.</span></span>

> <span data-ttu-id="cff6c-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cff6c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
