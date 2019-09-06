---
title: Criar workbookCommentReply
description: Use esta API para criar um novo workbookCommentReply.
localization_priority: Normal
author: grangeryy
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: edf4dafa40c7323bde788234f1efa4308f401fd3
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775766"
---
# <a name="create-workbookcommentreply"></a><span data-ttu-id="d6389-103">Criar workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="d6389-103">Create workbookCommentReply</span></span>

<span data-ttu-id="d6389-104">Criar um novo objeto [workbookCommentReply](../resources/workbookcommentreply.md) .</span><span class="sxs-lookup"><span data-stu-id="d6389-104">Create a new [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6389-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6389-105">Permissions</span></span>

<span data-ttu-id="d6389-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6389-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d6389-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6389-108">Permission type</span></span>                        | <span data-ttu-id="d6389-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6389-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d6389-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6389-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6389-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6389-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="d6389-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6389-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6389-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6389-113">Not supported.</span></span> |
| <span data-ttu-id="d6389-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6389-114">Application</span></span>                            | <span data-ttu-id="d6389-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6389-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6389-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6389-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /workbook/comments/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="d6389-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6389-117">Request headers</span></span>

| <span data-ttu-id="d6389-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d6389-118">Name</span></span>          | <span data-ttu-id="d6389-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6389-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d6389-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6389-120">Authorization</span></span> | <span data-ttu-id="d6389-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6389-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6389-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6389-123">Request body</span></span>

<span data-ttu-id="d6389-124">No corpo da solicitação, forneça uma representação JSON de um objeto [workbookCommentReply](../resources/workbookcommentreply.md) .</span><span class="sxs-lookup"><span data-stu-id="d6389-124">In the request body, supply a JSON representation of a [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d6389-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6389-125">Response</span></span>

<span data-ttu-id="d6389-126">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [workbookCommentReply](../resources/workbookcommentreply.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6389-126">If successful, this method returns a `201 Created` response code and a new [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6389-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d6389-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6389-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6389-128">Request</span></span>

<span data-ttu-id="d6389-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6389-129">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d6389-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6389-130">Response</span></span>

<span data-ttu-id="d6389-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d6389-131">The following is an example of the response.</span></span>

> <span data-ttu-id="d6389-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6389-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
