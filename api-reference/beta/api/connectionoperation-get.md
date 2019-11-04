---
title: Obter connectionOperation
description: Recupere as propriedades de um connectionOperation.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 76936584883549fb2fd2fedbeed42cbe78702e55
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936591"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="09ec8-103">Obter connectionOperation</span><span class="sxs-lookup"><span data-stu-id="09ec8-103">Get connectionOperation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09ec8-104">Recupere as propriedades de um [connectionOperation](../resources/connectionoperation.md).</span><span class="sxs-lookup"><span data-stu-id="09ec8-104">Retrieve the properties of a [connectionOperation](../resources/connectionoperation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="09ec8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="09ec8-105">Permissions</span></span>

<span data-ttu-id="09ec8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09ec8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09ec8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09ec8-108">Permission type</span></span>                        | <span data-ttu-id="09ec8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09ec8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="09ec8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09ec8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="09ec8-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09ec8-111">Not supported.</span></span> |
| <span data-ttu-id="09ec8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09ec8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09ec8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09ec8-113">Not supported.</span></span> |
| <span data-ttu-id="09ec8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09ec8-114">Application</span></span>                            | <span data-ttu-id="09ec8-115">ExternalItem. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="09ec8-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09ec8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09ec8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="09ec8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09ec8-117">Request headers</span></span>

| <span data-ttu-id="09ec8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="09ec8-118">Name</span></span>          | <span data-ttu-id="09ec8-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="09ec8-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="09ec8-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="09ec8-120">Authorization</span></span> | <span data-ttu-id="09ec8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09ec8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09ec8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09ec8-123">Request body</span></span>

<span data-ttu-id="09ec8-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09ec8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09ec8-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="09ec8-125">Response</span></span>

<span data-ttu-id="09ec8-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [connectionOperation](../resources/connectionoperation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09ec8-126">If successful, this method returns a `200 OK` response code and the requested [connectionOperation](../resources/connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="09ec8-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="09ec8-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="09ec8-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09ec8-128">Request</span></span>

<span data-ttu-id="09ec8-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="09ec8-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}-->

```http
GET https://graph.microsoft.com/beta/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="09ec8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="09ec8-130">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="09ec8-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="09ec8-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "expectError": true,
  "@odata.type": "microsoft.graph.connectionOperation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "3ed1595a-4bae-43c2-acda-ef973e581323",
  "status": "failed",
  "error": {
    "message": "Server error, something went wrong"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connectionOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
