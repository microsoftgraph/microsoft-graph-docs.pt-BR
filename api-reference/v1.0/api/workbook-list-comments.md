---
title: Listar workbookComments
description: Recupere uma lista de objetos workbookComment.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4fddb5eac07994fa9b1b837320e2e5891f8e38c1
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539271"
---
# <a name="list-workbookcomments"></a><span data-ttu-id="daccd-103">Listar workbookComments</span><span class="sxs-lookup"><span data-stu-id="daccd-103">List workbookComments</span></span>

<span data-ttu-id="daccd-104">Recupere uma lista de objetos [workbookComment](../resources/workbookcomment.md) .</span><span class="sxs-lookup"><span data-stu-id="daccd-104">Retrieve a list of  [workbookComment](../resources/workbookcomment.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="daccd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="daccd-105">Permissions</span></span>

<span data-ttu-id="daccd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daccd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="daccd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="daccd-108">Permission type</span></span>                        | <span data-ttu-id="daccd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="daccd-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="daccd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="daccd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="daccd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="daccd-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="daccd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="daccd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daccd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daccd-113">Not supported.</span></span> |
| <span data-ttu-id="daccd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="daccd-114">Application</span></span>                            | <span data-ttu-id="daccd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daccd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="daccd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="daccd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET workbook/comments
```

## <a name="request-headers"></a><span data-ttu-id="daccd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="daccd-117">Request headers</span></span>

| <span data-ttu-id="daccd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="daccd-118">Name</span></span>      |<span data-ttu-id="daccd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="daccd-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="daccd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="daccd-120">Authorization</span></span> | <span data-ttu-id="daccd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="daccd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="daccd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="daccd-123">Request body</span></span>

<span data-ttu-id="daccd-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="daccd-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="daccd-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="daccd-125">Response</span></span>

<span data-ttu-id="daccd-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [workbookComment](../resources/workbookcomment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="daccd-126">If successful, this method returns a `200 OK` response code and a collection of [workbookComment](../resources/workbookcomment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="daccd-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="daccd-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="daccd-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="daccd-128">Request</span></span>

<span data-ttu-id="daccd-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="daccd-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="daccd-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="daccd-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_comments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drive/root/workbook/comments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="daccd-131">C#</span><span class="sxs-lookup"><span data-stu-id="daccd-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-comments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="daccd-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="daccd-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-comments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="daccd-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="daccd-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-comments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="daccd-134">Java</span><span class="sxs-lookup"><span data-stu-id="daccd-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-comments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="daccd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="daccd-135">Response</span></span>

<span data-ttu-id="daccd-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="daccd-136">The following is an example of the response.</span></span>

> <span data-ttu-id="daccd-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="daccd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
