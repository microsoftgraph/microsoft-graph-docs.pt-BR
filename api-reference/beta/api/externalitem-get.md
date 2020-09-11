---
title: Obter externalItem
description: Obter um externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c24a456759a7921faf353f8c7cba6e8407362f65
ms.sourcegitcommit: c7c198f6fa252b68e91be341b93b818afd387486
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2020
ms.locfileid: "47439952"
---
# <a name="get-externalitem"></a><span data-ttu-id="3a550-103">Obter externalItem</span><span class="sxs-lookup"><span data-stu-id="3a550-103">Get externalItem</span></span>

<span data-ttu-id="3a550-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a550-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a550-105">Obtenha as propriedades e os relacionamentos de um objeto [externalitem](../resources/externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="3a550-105">Get the properties and relationships of an [externalitem](../resources/externalitem.md) object.</span></span>

<span data-ttu-id="3a550-106">Essa API é fornecida apenas para fins de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="3a550-106">This API is provided for diagnostic purposes only.</span></span> <span data-ttu-id="3a550-107">Ele não se destina a ser usado para qualquer outra finalidade.</span><span class="sxs-lookup"><span data-stu-id="3a550-107">It is not intended to be used for any other purpose.</span></span> <span data-ttu-id="3a550-108">Solicitações repetidas para essa API podem resultar em `429` erros http.</span><span class="sxs-lookup"><span data-stu-id="3a550-108">Repeated requests to this API might result in `429` HTTP errors.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="3a550-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a550-109">Permissions</span></span>

<span data-ttu-id="3a550-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a550-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a550-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a550-112">Permission type</span></span>                        | <span data-ttu-id="3a550-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a550-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3a550-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a550-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a550-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a550-115">Not supported.</span></span> |
| <span data-ttu-id="3a550-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a550-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a550-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a550-117">Not supported.</span></span> |
| <span data-ttu-id="3a550-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a550-118">Application</span></span>                            | <span data-ttu-id="3a550-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a550-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a550-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a550-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="3a550-121">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="3a550-121">Path parameters</span></span>

| <span data-ttu-id="3a550-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3a550-122">Parameter</span></span>     | <span data-ttu-id="3a550-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a550-123">Type</span></span>   | <span data-ttu-id="3a550-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a550-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="3a550-125">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="3a550-125">connection-id</span></span> | <span data-ttu-id="3a550-126">string</span><span class="sxs-lookup"><span data-stu-id="3a550-126">string</span></span> | <span data-ttu-id="3a550-127">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="3a550-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="3a550-128">item-id</span><span class="sxs-lookup"><span data-stu-id="3a550-128">item-id</span></span>       | <span data-ttu-id="3a550-129">string</span><span class="sxs-lookup"><span data-stu-id="3a550-129">string</span></span> | <span data-ttu-id="3a550-130">A propriedade fornecida pelo desenvolvedor `id` do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="3a550-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="3a550-131">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3a550-131">Optional query parameters</span></span>

<span data-ttu-id="3a550-132">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3a550-132">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a550-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a550-133">Request headers</span></span>

| <span data-ttu-id="3a550-134">Nome</span><span class="sxs-lookup"><span data-stu-id="3a550-134">Name</span></span>          | <span data-ttu-id="3a550-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a550-135">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3a550-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a550-136">Authorization</span></span> | <span data-ttu-id="3a550-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a550-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a550-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a550-139">Request body</span></span>

<span data-ttu-id="3a550-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a550-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a550-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a550-141">Response</span></span>

<span data-ttu-id="3a550-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [externalItem](../resources/externalitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a550-142">If successful, this method returns a `200 OK` response code and an [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a550-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a550-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a550-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a550-144">Request</span></span>

<span data-ttu-id="3a550-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a550-145">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="3a550-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a550-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="3a550-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3a550-147">The following is an example of the response.</span></span>

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
