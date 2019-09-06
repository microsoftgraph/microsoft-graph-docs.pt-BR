---
title: Listar workbookComments
description: Recupere uma lista de objetos workbookComment.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 25bfb1f893fe3ba02b620b319f60ef72e275f0b7
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775780"
---
# <a name="list-workbookcomments"></a><span data-ttu-id="54195-103">Listar workbookComments</span><span class="sxs-lookup"><span data-stu-id="54195-103">List workbookComments</span></span>

<span data-ttu-id="54195-104">Recupere uma lista de objetos [workbookComment](../resources/workbookcomment.md) .</span><span class="sxs-lookup"><span data-stu-id="54195-104">Retrieve a list of  [workbookComment](../resources/workbookcomment.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="54195-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="54195-105">Permissions</span></span>

<span data-ttu-id="54195-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54195-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54195-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54195-108">Permission type</span></span>                        | <span data-ttu-id="54195-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54195-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="54195-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54195-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="54195-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54195-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="54195-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54195-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54195-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54195-113">Not supported.</span></span> |
| <span data-ttu-id="54195-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54195-114">Application</span></span>                            | <span data-ttu-id="54195-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54195-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="54195-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54195-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET workbook/comments
```

## <a name="request-headers"></a><span data-ttu-id="54195-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54195-117">Request headers</span></span>

| <span data-ttu-id="54195-118">Nome</span><span class="sxs-lookup"><span data-stu-id="54195-118">Name</span></span>      |<span data-ttu-id="54195-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="54195-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="54195-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="54195-120">Authorization</span></span> | <span data-ttu-id="54195-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54195-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54195-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54195-123">Request body</span></span>

<span data-ttu-id="54195-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54195-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54195-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="54195-125">Response</span></span>

<span data-ttu-id="54195-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [workbookComment](../resources/workbookcomment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54195-126">If successful, this method returns a `200 OK` response code and a collection of [workbookComment](../resources/workbookcomment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54195-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="54195-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54195-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54195-128">Request</span></span>

<span data-ttu-id="54195-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="54195-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_comments"
}-->

```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/comments
```

### <a name="response"></a><span data-ttu-id="54195-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="54195-130">Response</span></span>

<span data-ttu-id="54195-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="54195-131">The following is an example of the response.</span></span>

> <span data-ttu-id="54195-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54195-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
