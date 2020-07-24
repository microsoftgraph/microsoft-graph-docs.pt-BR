---
title: Obter workbookOperation
description: Recuperar o status de um objeto workbookOperation.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0d790d7bfc243cb5cfbc32a12d6a00db32c46cd9
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408135"
---
# <a name="get-workbookoperation"></a><span data-ttu-id="f7670-103">Obter workbookOperation</span><span class="sxs-lookup"><span data-stu-id="f7670-103">Get workbookOperation</span></span>

<span data-ttu-id="f7670-104">Recuperar o status de um objeto [workbookOperation](../resources/workbookoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="f7670-104">Retrieve the status of a [workbookOperation](../resources/workbookoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7670-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7670-105">Permissions</span></span>

<span data-ttu-id="f7670-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7670-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7670-108">Permission type</span></span>                        | <span data-ttu-id="f7670-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7670-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f7670-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7670-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7670-111">Files. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="f7670-111">Files.ReadWrite.</span></span> |
| <span data-ttu-id="f7670-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7670-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7670-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7670-113">Not supported.</span></span> |
| <span data-ttu-id="f7670-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7670-114">Application</span></span>                            | <span data-ttu-id="f7670-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7670-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7670-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7670-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET workbook/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="f7670-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7670-117">Request headers</span></span>

| <span data-ttu-id="f7670-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f7670-118">Name</span></span>      |<span data-ttu-id="f7670-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7670-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f7670-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7670-120">Authorization</span></span> | <span data-ttu-id="f7670-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7670-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7670-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7670-123">Request body</span></span>

<span data-ttu-id="f7670-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7670-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7670-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7670-125">Response</span></span>

<span data-ttu-id="f7670-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [workbookOperation](../resources/workbookoperation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7670-126">If successful, this method returns a `200 OK` response code and the requested [workbookOperation](../resources/workbookoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7670-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7670-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7670-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7670-128">Request</span></span>

<span data-ttu-id="f7670-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7670-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookoperation"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
```

### <a name="response"></a><span data-ttu-id="f7670-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7670-130">Response</span></span>

<span data-ttu-id="f7670-131">Veja a seguir a resposta com o status "em execução".</span><span class="sxs-lookup"><span data-stu-id="f7670-131">The following is the response with the status of "running".</span></span>


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

<span data-ttu-id="f7670-132">Veja a seguir a resposta com o status de "êxito".</span><span class="sxs-lookup"><span data-stu-id="f7670-132">The following is the response with the status of "succeeded".</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "succeeded",
  "resourceLocation":"https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')"
}
```

<span data-ttu-id="f7670-133">Veja a seguir a resposta com o status de "falha".</span><span class="sxs-lookup"><span data-stu-id="f7670-133">The following is the response with the status of "failed".</span></span>

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
