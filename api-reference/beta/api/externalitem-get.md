---
title: Obter externalItem
description: Obter um externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: a894afa05207dc483e5fbbf3e4de14e0b400f894
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006801"
---
# <a name="get-externalitem"></a><span data-ttu-id="1f323-103">Obter externalItem</span><span class="sxs-lookup"><span data-stu-id="1f323-103">Get externalItem</span></span>

<span data-ttu-id="1f323-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1f323-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f323-105">Obtenha as propriedades e os relacionamentos de um objeto [externalitem](../resources/externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="1f323-105">Get the properties and relationships of an [externalitem](../resources/externalitem.md) object.</span></span>

<span data-ttu-id="1f323-106">Essa API é fornecida apenas para fins de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="1f323-106">This API is provided for diagnostic purposes only.</span></span> <span data-ttu-id="1f323-107">Ele não se destina a ser usado para qualquer outra finalidade.</span><span class="sxs-lookup"><span data-stu-id="1f323-107">It is not intended to be used for any other purpose.</span></span> <span data-ttu-id="1f323-108">Solicitações repetidas para essa API podem resultar em `429` erros http.</span><span class="sxs-lookup"><span data-stu-id="1f323-108">Repeated requests to this API might result in `429` HTTP errors.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="1f323-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f323-109">Permissions</span></span>

<span data-ttu-id="1f323-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f323-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f323-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f323-112">Permission type</span></span>                        | <span data-ttu-id="1f323-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f323-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1f323-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f323-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f323-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f323-115">Not supported.</span></span> |
| <span data-ttu-id="1f323-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f323-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f323-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f323-117">Not supported.</span></span> |
| <span data-ttu-id="1f323-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f323-118">Application</span></span>                            | <span data-ttu-id="1f323-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f323-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f323-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f323-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="1f323-121">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="1f323-121">Path parameters</span></span>

| <span data-ttu-id="1f323-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1f323-122">Parameter</span></span>     | <span data-ttu-id="1f323-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f323-123">Type</span></span>   | <span data-ttu-id="1f323-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f323-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="1f323-125">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="1f323-125">connection-id</span></span> | <span data-ttu-id="1f323-126">string</span><span class="sxs-lookup"><span data-stu-id="1f323-126">string</span></span> | <span data-ttu-id="1f323-127">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="1f323-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="1f323-128">item-id</span><span class="sxs-lookup"><span data-stu-id="1f323-128">item-id</span></span>       | <span data-ttu-id="1f323-129">string</span><span class="sxs-lookup"><span data-stu-id="1f323-129">string</span></span> | <span data-ttu-id="1f323-130">A propriedade fornecida pelo desenvolvedor `id` do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="1f323-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="1f323-131">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1f323-131">Optional query parameters</span></span>

<span data-ttu-id="1f323-132">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1f323-132">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f323-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f323-133">Request headers</span></span>

| <span data-ttu-id="1f323-134">Nome</span><span class="sxs-lookup"><span data-stu-id="1f323-134">Name</span></span>          | <span data-ttu-id="1f323-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f323-135">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1f323-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f323-136">Authorization</span></span> | <span data-ttu-id="1f323-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f323-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f323-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f323-139">Request body</span></span>

<span data-ttu-id="1f323-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f323-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f323-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f323-141">Response</span></span>

<span data-ttu-id="1f323-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [externalItem](../resources/externalitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f323-142">If successful, this method returns a `200 OK` response code and an [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f323-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f323-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f323-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f323-144">Request</span></span>

<span data-ttu-id="1f323-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f323-145">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="1f323-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f323-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="1f323-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1f323-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalItem",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "deny",
      "identitySource": "azureActiveDirectory"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "<h1>Error in payment gateway</h1><p>Error details...</p>",
    "type": "html"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


