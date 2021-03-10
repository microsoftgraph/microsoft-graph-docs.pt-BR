---
title: Obter workbookOperation
description: Recupere as propriedades e as relações de um objeto workbookOperation.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bf5f7abd26368b233091ff4294e0f1707c4f01ab
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626185"
---
# <a name="get-workbookoperation"></a><span data-ttu-id="aeb22-103">Obter workbookOperation</span><span class="sxs-lookup"><span data-stu-id="aeb22-103">Get workbookOperation</span></span>

<span data-ttu-id="aeb22-104">Recupere o status de um [objeto workbookOperation.](../resources/workbookoperation.md)</span><span class="sxs-lookup"><span data-stu-id="aeb22-104">Retrieve the status of a [workbookOperation](../resources/workbookoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aeb22-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="aeb22-105">Permissions</span></span>

<span data-ttu-id="aeb22-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aeb22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aeb22-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aeb22-108">Permission type</span></span>                        | <span data-ttu-id="aeb22-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aeb22-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aeb22-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aeb22-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="aeb22-111">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="aeb22-111">Files.ReadWrite.</span></span> |
| <span data-ttu-id="aeb22-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aeb22-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aeb22-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aeb22-113">Not supported.</span></span> |
| <span data-ttu-id="aeb22-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aeb22-114">Application</span></span>                            | <span data-ttu-id="aeb22-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aeb22-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aeb22-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aeb22-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/items/{id}/workbook/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="aeb22-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aeb22-117">Request headers</span></span>

| <span data-ttu-id="aeb22-118">Nome</span><span class="sxs-lookup"><span data-stu-id="aeb22-118">Name</span></span>      |<span data-ttu-id="aeb22-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="aeb22-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aeb22-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="aeb22-120">Authorization</span></span> | <span data-ttu-id="aeb22-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aeb22-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aeb22-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aeb22-123">Request body</span></span>

<span data-ttu-id="aeb22-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aeb22-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aeb22-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="aeb22-125">Response</span></span>

<span data-ttu-id="aeb22-126">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [workbookOperation](../resources/workbookoperation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aeb22-126">If successful, this method returns a `200 OK` response code and the requested [workbookOperation](../resources/workbookoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aeb22-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="aeb22-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aeb22-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aeb22-128">Request</span></span>

<span data-ttu-id="aeb22-129">A seguir, um exemplo de uma solicitação de operação de longa duração.</span><span class="sxs-lookup"><span data-stu-id="aeb22-129">The following is an example of a long-running operation request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aeb22-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="aeb22-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
```
# <a name="c"></a>[<span data-ttu-id="aeb22-131">C#</span><span class="sxs-lookup"><span data-stu-id="aeb22-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aeb22-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aeb22-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aeb22-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aeb22-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aeb22-134">Java</span><span class="sxs-lookup"><span data-stu-id="aeb22-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aeb22-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="aeb22-135">Response</span></span>

<span data-ttu-id="aeb22-136">A seguir está a resposta com o status de "running".</span><span class="sxs-lookup"><span data-stu-id="aeb22-136">The following is the response with the status of "running".</span></span>


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

<span data-ttu-id="aeb22-137">A seguir está a resposta com o status de "bem-sucedido".</span><span class="sxs-lookup"><span data-stu-id="aeb22-137">The following is the response with the status of "succeeded".</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "succeeded",
  "resourceLocation":"https://graph.microsoft.com/beta/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')"
}
```

<span data-ttu-id="aeb22-138">A seguir está a resposta com o status de "failed".</span><span class="sxs-lookup"><span data-stu-id="aeb22-138">The following is the response with the status of "failed".</span></span>

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


