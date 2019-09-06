---
title: Listar workbookCommentReplies
description: Recupere uma lista de objetos workbookcommentreply.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9d7b70d088b92a7abc84a76d08b29924fae5b41f
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775773"
---
# <a name="list-workbookcommentreplies"></a><span data-ttu-id="dfe06-103">Listar workbookCommentReplies</span><span class="sxs-lookup"><span data-stu-id="dfe06-103">List workbookCommentReplies</span></span>

<span data-ttu-id="dfe06-104">Recupere uma lista de objetos [workbookCommentReply](../resources/workbookcommentreply.md) .</span><span class="sxs-lookup"><span data-stu-id="dfe06-104">Retrieve a list of [workbookCommentReply](../resources/workbookcommentreply.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfe06-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfe06-105">Permissions</span></span>

<span data-ttu-id="dfe06-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfe06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfe06-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfe06-108">Permission type</span></span>                        | <span data-ttu-id="dfe06-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfe06-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dfe06-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfe06-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfe06-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfe06-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="dfe06-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfe06-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfe06-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfe06-113">Not supported.</span></span> |
| <span data-ttu-id="dfe06-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfe06-114">Application</span></span>                            | <span data-ttu-id="dfe06-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfe06-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfe06-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfe06-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /workbook/comments/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="dfe06-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfe06-117">Request headers</span></span>

| <span data-ttu-id="dfe06-118">Nome</span><span class="sxs-lookup"><span data-stu-id="dfe06-118">Name</span></span>      |<span data-ttu-id="dfe06-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfe06-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dfe06-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfe06-120">Authorization</span></span> | <span data-ttu-id="dfe06-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfe06-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfe06-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfe06-123">Request body</span></span>

<span data-ttu-id="dfe06-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfe06-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfe06-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfe06-125">Response</span></span>

<span data-ttu-id="dfe06-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [workbookCommentReply](../resources/workbookcommentreply.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfe06-126">If successful, this method returns a `200 OK` response code and a collection of [workbookCommentReply](../resources/workbookcommentreply.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dfe06-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dfe06-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dfe06-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfe06-128">Request</span></span>

<span data-ttu-id="dfe06-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfe06-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_replies"
}-->

```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/comments/{id}/replies
```

### <a name="response"></a><span data-ttu-id="dfe06-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfe06-130">Response</span></span>

<span data-ttu-id="dfe06-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dfe06-131">The following is an example of the response.</span></span>

> <span data-ttu-id="dfe06-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfe06-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
