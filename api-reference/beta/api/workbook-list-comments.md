---
title: Listar workbookComments
description: Recupere uma lista de objetos workbookComments.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 255acd6d36aa61e3aa044ad1ffe167f007253593
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575319"
---
# <a name="list-workbookcomments"></a><span data-ttu-id="afaef-103">Listar workbookComments</span><span class="sxs-lookup"><span data-stu-id="afaef-103">List workbookComments</span></span>

<span data-ttu-id="afaef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afaef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="afaef-105">Recupere uma lista de [objetos workbookComment.](../resources/workbookcomment.md)</span><span class="sxs-lookup"><span data-stu-id="afaef-105">Retrieve a list of  [workbookComment](../resources/workbookcomment.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="afaef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="afaef-106">Permissions</span></span>

<span data-ttu-id="afaef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afaef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="afaef-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afaef-109">Permission type</span></span>                        | <span data-ttu-id="afaef-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="afaef-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="afaef-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afaef-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="afaef-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="afaef-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="afaef-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afaef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afaef-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afaef-114">Not supported.</span></span> |
| <span data-ttu-id="afaef-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afaef-115">Application</span></span>                            | <span data-ttu-id="afaef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afaef-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="afaef-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afaef-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/items/{id}/workbook/comments
GET /me/drive/root:/{item-path}:/workbook/comments
```

## <a name="request-headers"></a><span data-ttu-id="afaef-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afaef-118">Request headers</span></span>

| <span data-ttu-id="afaef-119">Nome</span><span class="sxs-lookup"><span data-stu-id="afaef-119">Name</span></span>      |<span data-ttu-id="afaef-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="afaef-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="afaef-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="afaef-121">Authorization</span></span> | <span data-ttu-id="afaef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afaef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="afaef-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afaef-124">Request body</span></span>

<span data-ttu-id="afaef-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="afaef-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afaef-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="afaef-126">Response</span></span>

<span data-ttu-id="afaef-127">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos workbookComment](../resources/workbookcomment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afaef-127">If successful, this method returns a `200 OK` response code and a collection of [workbookComment](../resources/workbookcomment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="afaef-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="afaef-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="afaef-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afaef-129">Request</span></span>

<span data-ttu-id="afaef-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="afaef-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="afaef-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="afaef-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_comments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{id}/workbook/comments
```
# <a name="c"></a>[<span data-ttu-id="afaef-132">C#</span><span class="sxs-lookup"><span data-stu-id="afaef-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-comments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afaef-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afaef-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-comments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afaef-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afaef-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-comments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="afaef-135">Java</span><span class="sxs-lookup"><span data-stu-id="afaef-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-comments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="afaef-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="afaef-136">Response</span></span>

<span data-ttu-id="afaef-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="afaef-137">The following is an example of the response.</span></span>

> <span data-ttu-id="afaef-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afaef-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


