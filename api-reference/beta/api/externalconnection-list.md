---
title: Listar conexões
description: Recupere uma lista de externalConnections.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 04f878f81e2b3d1679c44fff1a80681f5a868848
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938657"
---
# <a name="list-connections"></a><span data-ttu-id="5488b-103">Listar conexões</span><span class="sxs-lookup"><span data-stu-id="5488b-103">List connections</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5488b-104">Recupere uma lista de [externalConnections](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="5488b-104">Retrieve a list of [externalConnections](../resources/externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5488b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5488b-105">Permissions</span></span>

<span data-ttu-id="5488b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5488b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5488b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5488b-108">Permission type</span></span>                        | <span data-ttu-id="5488b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5488b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5488b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5488b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5488b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5488b-111">Not supported.</span></span> |
| <span data-ttu-id="5488b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5488b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5488b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5488b-113">Not supported.</span></span> |
| <span data-ttu-id="5488b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5488b-114">Application</span></span>                            | <span data-ttu-id="5488b-115">ExternalItem. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5488b-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5488b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5488b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5488b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5488b-117">Optional query parameters</span></span>

<span data-ttu-id="5488b-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5488b-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5488b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5488b-119">Request headers</span></span>

| <span data-ttu-id="5488b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5488b-120">Name</span></span>          | <span data-ttu-id="5488b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5488b-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5488b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5488b-122">Authorization</span></span> | <span data-ttu-id="5488b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5488b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5488b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5488b-125">Request body</span></span>

<span data-ttu-id="5488b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5488b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5488b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5488b-127">Response</span></span>

<span data-ttu-id="5488b-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [externalConnection](../resources/externalconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5488b-128">If successful, this method returns a `200 OK` response code and a collection of [externalConnection](../resources/externalconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5488b-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5488b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5488b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5488b-130">Request</span></span>

<span data-ttu-id="5488b-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5488b-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connections"
}-->

```http
GET https://graph.microsoft.com/beta/external/connections
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="5488b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5488b-132">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="5488b-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5488b-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnection",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contosohr",
      "name": "Contoso HR",
      "description": "Connection to index Contoso HR system",
      "configuration": {
        "authorizedApps": [
          "d310d35d-72ec-47dd-92f2-fb9c40936555"
        ]
      }
    },
    {
      "id": "contosofinance",
      "name": "Contoso Finance",
      "description": "Connection to index Contoso Finance system",
      "configuration": {
        "authorizedApps": [
          "fbdc7d4e-07f4-4143-8258-e5a2fcebeadb"
        ]
      }
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List connections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
