---
title: Listar workbookComments
description: Recupere uma lista de objetos workbookComment.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 11ec3c796207e216734fb9e858b7fb0fd9ef0007
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52031494"
---
# <a name="list-workbookcomments"></a><span data-ttu-id="5ee77-103">Listar workbookComments</span><span class="sxs-lookup"><span data-stu-id="5ee77-103">List workbookComments</span></span>

<span data-ttu-id="5ee77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ee77-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ee77-105">Recupere uma lista de [objetos workbookComment.](../resources/workbookcomment.md)</span><span class="sxs-lookup"><span data-stu-id="5ee77-105">Retrieve a list of  [workbookComment](../resources/workbookcomment.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ee77-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ee77-106">Permissions</span></span>

<span data-ttu-id="5ee77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ee77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ee77-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ee77-109">Permission type</span></span>                        | <span data-ttu-id="5ee77-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ee77-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5ee77-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ee77-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ee77-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ee77-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="5ee77-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ee77-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ee77-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee77-114">Not supported.</span></span> |
| <span data-ttu-id="5ee77-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ee77-115">Application</span></span>                            | <span data-ttu-id="5ee77-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee77-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ee77-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee77-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/items/{id}/workbook/comments
```

## <a name="request-headers"></a><span data-ttu-id="5ee77-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee77-118">Request headers</span></span>

| <span data-ttu-id="5ee77-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5ee77-119">Name</span></span>      |<span data-ttu-id="5ee77-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ee77-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ee77-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ee77-121">Authorization</span></span> | <span data-ttu-id="5ee77-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ee77-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ee77-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee77-124">Request body</span></span>

<span data-ttu-id="5ee77-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ee77-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ee77-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee77-126">Response</span></span>

<span data-ttu-id="5ee77-127">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos workbookComment](../resources/workbookcomment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee77-127">If successful, this method returns a `200 OK` response code and a collection of [workbookComment](../resources/workbookcomment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ee77-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5ee77-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ee77-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee77-129">Request</span></span>

<span data-ttu-id="5ee77-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee77-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ee77-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee77-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_comments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drive/items/{id}/workbook/comments
```
# <a name="c"></a>[<span data-ttu-id="5ee77-132">C#</span><span class="sxs-lookup"><span data-stu-id="5ee77-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-comments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ee77-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ee77-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-comments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ee77-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ee77-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-comments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ee77-135">Java</span><span class="sxs-lookup"><span data-stu-id="5ee77-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-comments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5ee77-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee77-136">Response</span></span>

<span data-ttu-id="5ee77-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee77-137">The following is an example of the response.</span></span>

> <span data-ttu-id="5ee77-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5ee77-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookComment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "content": "This is text of comment.",
      "contentType": "plain",
      "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List comments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

