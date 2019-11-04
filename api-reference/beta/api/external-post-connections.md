---
title: Criar conexão
description: Use esta API para criar um novo externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 6b85c5a9a09690f91f3e0934512f3cc874e54b46
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938678"
---
# <a name="create-connection"></a><span data-ttu-id="a412e-103">Criar conexão</span><span class="sxs-lookup"><span data-stu-id="a412e-103">Create connection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a412e-104">Criar um novo [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="a412e-104">Create a new [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a412e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a412e-105">Permissions</span></span>

<span data-ttu-id="a412e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a412e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a412e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a412e-108">Permission type</span></span>                        | <span data-ttu-id="a412e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a412e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a412e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a412e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a412e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a412e-111">Not supported.</span></span> |
| <span data-ttu-id="a412e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a412e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a412e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a412e-113">Not supported.</span></span> |
| <span data-ttu-id="a412e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a412e-114">Application</span></span>                            | <span data-ttu-id="a412e-115">ExternalItem. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a412e-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a412e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a412e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections
```

## <a name="request-headers"></a><span data-ttu-id="a412e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a412e-117">Request headers</span></span>

| <span data-ttu-id="a412e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a412e-118">Name</span></span>          | <span data-ttu-id="a412e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a412e-119">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="a412e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a412e-120">Authorization</span></span> | <span data-ttu-id="a412e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a412e-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="a412e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a412e-123">Content-Type</span></span>  | <span data-ttu-id="a412e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a412e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a412e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a412e-126">Request body</span></span>

<span data-ttu-id="a412e-127">No corpo da solicitação, forneça uma representação JSON de um objeto [externalConnection](../resources/externalconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="a412e-127">In the request body, supply a JSON representation of a [externalConnection](../resources/externalconnection.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a412e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a412e-128">Response</span></span>

<span data-ttu-id="a412e-129">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [externalConnection](../resources/externalconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a412e-129">If successful, this method returns `201 Created` response code and a new [externalConnection](../resources/externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a412e-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a412e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a412e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a412e-131">Request</span></span>

<span data-ttu-id="a412e-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a412e-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connection_from_external"
}-->

```http
POST https://graph.microsoft.com/beta/external/connections
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system"
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="a412e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a412e-133">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="a412e-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a412e-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnection"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system",
  "configuration": {
    "authorizedApps": [
      "d310d35d-72ec-47dd-92f2-fb9c40936555"
    ]
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
