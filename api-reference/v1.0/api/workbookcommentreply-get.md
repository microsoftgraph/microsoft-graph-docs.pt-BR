---
title: Obter workbookCommentReply
description: Recupere as propriedades e os relacionamentos do objeto workbookcommentreply.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 97ae39d4cfb68aafaea0613f524deb9a7f6be0af
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775724"
---
# <a name="get-workbookcommentreply"></a><span data-ttu-id="8ad87-103">Obter workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="8ad87-103">Get workbookCommentReply</span></span>

<span data-ttu-id="8ad87-104">Recupere as propriedades e os relacionamentos do objeto [workbookCommentReply](../resources/workbookcommentreply.md) .</span><span class="sxs-lookup"><span data-stu-id="8ad87-104">Retrieve the properties and relationships of [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ad87-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ad87-105">Permissions</span></span>

<span data-ttu-id="8ad87-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ad87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ad87-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ad87-108">Permission type</span></span>                        | <span data-ttu-id="8ad87-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ad87-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8ad87-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ad87-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ad87-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ad87-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="8ad87-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ad87-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ad87-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ad87-113">Not supported.</span></span> |
| <span data-ttu-id="8ad87-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ad87-114">Application</span></span>                            | <span data-ttu-id="8ad87-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ad87-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ad87-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ad87-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /workbook/comments/{id}/replies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8ad87-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ad87-117">Request headers</span></span>

| <span data-ttu-id="8ad87-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8ad87-118">Name</span></span>      |<span data-ttu-id="8ad87-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ad87-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8ad87-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ad87-120">Authorization</span></span> | <span data-ttu-id="8ad87-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ad87-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ad87-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ad87-123">Request body</span></span>

<span data-ttu-id="8ad87-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ad87-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ad87-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ad87-125">Response</span></span>

<span data-ttu-id="8ad87-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [workbookCommentReply](../resources/workbookcommentreply.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ad87-126">If successful, this method returns a `200 OK` response code and the requested [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ad87-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8ad87-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8ad87-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ad87-128">Request</span></span>

<span data-ttu-id="8ad87-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ad87-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookcommentreply"
}-->

```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/comments/{id}/replies/{id}
```

### <a name="response"></a><span data-ttu-id="8ad87-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ad87-130">Response</span></span>

<span data-ttu-id="8ad87-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8ad87-131">The following is an example of the response.</span></span>

> <span data-ttu-id="8ad87-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ad87-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
