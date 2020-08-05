---
title: Obter workbookOperation
description: Recupere as propriedades e os relacionamentos de um objeto workbookOperation.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c5ead367116603a286574a30551134f9176d1477
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566165"
---
# <a name="get-workbookoperation"></a><span data-ttu-id="4f37b-103">Obter workbookOperation</span><span class="sxs-lookup"><span data-stu-id="4f37b-103">Get workbookOperation</span></span>

<span data-ttu-id="4f37b-104">Recuperar o status de um objeto [workbookOperation](../resources/workbookoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="4f37b-104">Retrieve the status of a [workbookOperation](../resources/workbookoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f37b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f37b-105">Permissions</span></span>

<span data-ttu-id="4f37b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f37b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f37b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f37b-108">Permission type</span></span>                        | <span data-ttu-id="4f37b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f37b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4f37b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f37b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f37b-111">Files. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="4f37b-111">Files.ReadWrite.</span></span> |
| <span data-ttu-id="4f37b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f37b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f37b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f37b-113">Not supported.</span></span> |
| <span data-ttu-id="4f37b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f37b-114">Application</span></span>                            | <span data-ttu-id="4f37b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f37b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f37b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f37b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET workbook/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="4f37b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f37b-117">Request headers</span></span>

| <span data-ttu-id="4f37b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4f37b-118">Name</span></span>      |<span data-ttu-id="4f37b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f37b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4f37b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f37b-120">Authorization</span></span> | <span data-ttu-id="4f37b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f37b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f37b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f37b-123">Request body</span></span>

<span data-ttu-id="4f37b-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f37b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f37b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f37b-125">Response</span></span>

<span data-ttu-id="4f37b-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [workbookOperation](../resources/workbookoperation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f37b-126">If successful, this method returns a `200 OK` response code and the requested [workbookOperation](../resources/workbookoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f37b-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4f37b-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4f37b-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f37b-128">Request</span></span>

<span data-ttu-id="4f37b-129">Veja a seguir um exemplo de uma solicitação de operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="4f37b-129">The following is an example of a long-running operation request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4f37b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f37b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
```
# <a name="c"></a>[<span data-ttu-id="4f37b-131">C#</span><span class="sxs-lookup"><span data-stu-id="4f37b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f37b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f37b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f37b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f37b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f37b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f37b-134">Response</span></span>

<span data-ttu-id="4f37b-135">Veja a seguir a resposta com o status "em execução".</span><span class="sxs-lookup"><span data-stu-id="4f37b-135">The following is the response with the status of "running".</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookOperation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "running"
}
```

<span data-ttu-id="4f37b-136">Veja a seguir a resposta com o status de "êxito".</span><span class="sxs-lookup"><span data-stu-id="4f37b-136">The following is the response with the status of "succeeded".</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "succeeded",
  "resourceLocation":"https://graph.microsoft.com/beta/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')"
}
```

<span data-ttu-id="4f37b-137">Veja a seguir a resposta com o status de "falha".</span><span class="sxs-lookup"><span data-stu-id="4f37b-137">The following is the response with the status of "failed".</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "failed",
  "error":
  {
      "code": "internalServerError",
      "message": "An internal server error occurred while processing the request.",
      "innerError": {
          "code": ""internalServerErrorUncategorized",
          "message": "An unspecified error has occurred.",
          "innerError": {
               "code": "GenericFileOpenError",
               "message": "The workbook cannot be opened."
          }
      }
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workbookOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
