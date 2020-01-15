---
title: Obter workbookComment
description: Recupere as propriedades e os relacionamentos do objeto workbookcomment.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f4fb64993431200c4689f11d41eec58b2781f856
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2020
ms.locfileid: "41119788"
---
# <a name="get-workbookcomment"></a><span data-ttu-id="46bca-103">Obter workbookComment</span><span class="sxs-lookup"><span data-stu-id="46bca-103">Get workbookComment</span></span>

<span data-ttu-id="46bca-104">Recupere as propriedades e os relacionamentos de um objeto [workbookComment](../resources/workbookcomment.md) .</span><span class="sxs-lookup"><span data-stu-id="46bca-104">Retrieve the properties and relationships of a [workbookComment](../resources/workbookcomment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="46bca-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="46bca-105">Permissions</span></span>

<span data-ttu-id="46bca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46bca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46bca-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46bca-108">Permission type</span></span>                        | <span data-ttu-id="46bca-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46bca-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="46bca-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46bca-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="46bca-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46bca-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="46bca-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46bca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46bca-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46bca-113">Not supported.</span></span> |
| <span data-ttu-id="46bca-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46bca-114">Application</span></span>                            | <span data-ttu-id="46bca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46bca-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46bca-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46bca-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET workbook/comments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="46bca-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46bca-117">Request headers</span></span>

| <span data-ttu-id="46bca-118">Nome</span><span class="sxs-lookup"><span data-stu-id="46bca-118">Name</span></span>      |<span data-ttu-id="46bca-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="46bca-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46bca-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="46bca-120">Authorization</span></span> | <span data-ttu-id="46bca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46bca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46bca-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46bca-123">Request body</span></span>

<span data-ttu-id="46bca-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46bca-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46bca-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="46bca-125">Response</span></span>

<span data-ttu-id="46bca-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [workbookComment](../resources/workbookcomment.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46bca-126">If successful, this method returns a `200 OK` response code and the requested [workbookComment](../resources/workbookcomment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46bca-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46bca-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46bca-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46bca-128">Request</span></span>

<span data-ttu-id="46bca-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="46bca-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="46bca-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="46bca-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookcomment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drive/items/{id}/workbook/comments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46bca-131">C#</span><span class="sxs-lookup"><span data-stu-id="46bca-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46bca-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46bca-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46bca-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46bca-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="46bca-134">Java</span><span class="sxs-lookup"><span data-stu-id="46bca-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookcomment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="46bca-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="46bca-135">Response</span></span>

<span data-ttu-id="46bca-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="46bca-136">The following is an example of the response.</span></span>

> <span data-ttu-id="46bca-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46bca-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookComment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "content": "This is my comment.",
  "contentType": "plain",
  "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workbookComment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
