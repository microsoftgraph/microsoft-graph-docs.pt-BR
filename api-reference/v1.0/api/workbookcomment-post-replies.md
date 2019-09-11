---
title: Criar workbookCommentReply
description: Use esta API para criar um novo workbookCommentReply.
localization_priority: Normal
author: grangeryy
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 0ec38cda1c2c138f4ae2168fbfe60f9d61b890fd
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839064"
---
# <a name="create-workbookcommentreply"></a><span data-ttu-id="82101-103">Criar workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="82101-103">Create workbookCommentReply</span></span>

<span data-ttu-id="82101-104">Criar um novo objeto [workbookCommentReply](../resources/workbookcommentreply.md) .</span><span class="sxs-lookup"><span data-stu-id="82101-104">Create a new [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="82101-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="82101-105">Permissions</span></span>

<span data-ttu-id="82101-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82101-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="82101-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82101-108">Permission type</span></span>                        | <span data-ttu-id="82101-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="82101-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="82101-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82101-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="82101-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82101-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="82101-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82101-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82101-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82101-113">Not supported.</span></span> |
| <span data-ttu-id="82101-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82101-114">Application</span></span>                            | <span data-ttu-id="82101-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82101-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82101-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82101-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /workbook/comments/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="82101-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82101-117">Request headers</span></span>

| <span data-ttu-id="82101-118">Nome</span><span class="sxs-lookup"><span data-stu-id="82101-118">Name</span></span>          | <span data-ttu-id="82101-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="82101-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="82101-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="82101-120">Authorization</span></span> | <span data-ttu-id="82101-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82101-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82101-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82101-123">Request body</span></span>

<span data-ttu-id="82101-124">No corpo da solicitação, forneça uma representação JSON de um objeto [workbookCommentReply](../resources/workbookcommentreply.md) .</span><span class="sxs-lookup"><span data-stu-id="82101-124">In the request body, supply a JSON representation of a [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="82101-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="82101-125">Response</span></span>

<span data-ttu-id="82101-126">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [workbookCommentReply](../resources/workbookcommentreply.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82101-126">If successful, this method returns a `201 Created` response code and a new [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82101-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="82101-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="82101-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82101-128">Request</span></span>

<span data-ttu-id="82101-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="82101-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="82101-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="82101-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workbookcommentreply_from_workbookcomment"
}-->

```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/comments/{id}/replies
Content-type: application/json

{
  "content": "This is my reply to the comment.",
  "contentType": "plain"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82101-131">C#</span><span class="sxs-lookup"><span data-stu-id="82101-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workbookcommentreply-from-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82101-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82101-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workbookcommentreply-from-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82101-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="82101-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workbookcommentreply-from-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="82101-134">Java</span><span class="sxs-lookup"><span data-stu-id="82101-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-workbookcommentreply-from-workbookcomment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="82101-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="82101-135">Response</span></span>

<span data-ttu-id="82101-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="82101-136">The following is an example of the response.</span></span>

> <span data-ttu-id="82101-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82101-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
