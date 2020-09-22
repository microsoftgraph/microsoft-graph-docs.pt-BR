---
title: Obter externalItem
description: Obter um externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: a504455b1f898d675474406e249e2637c12e1c69
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192187"
---
# <a name="get-externalitem"></a><span data-ttu-id="b3827-103">Obter externalItem</span><span class="sxs-lookup"><span data-stu-id="b3827-103">Get externalItem</span></span>

<span data-ttu-id="b3827-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3827-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3827-105">Obtenha as propriedades e os relacionamentos de um objeto [externalitem](../resources/externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="b3827-105">Get the properties and relationships of an [externalitem](../resources/externalitem.md) object.</span></span>

<span data-ttu-id="b3827-106">Essa API é fornecida apenas para fins de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="b3827-106">This API is provided for diagnostic purposes only.</span></span> <span data-ttu-id="b3827-107">Ele não se destina a ser usado para qualquer outra finalidade.</span><span class="sxs-lookup"><span data-stu-id="b3827-107">It is not intended to be used for any other purpose.</span></span> <span data-ttu-id="b3827-108">Solicitações repetidas para essa API podem resultar em `429` erros http.</span><span class="sxs-lookup"><span data-stu-id="b3827-108">Repeated requests to this API might result in `429` HTTP errors.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="b3827-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3827-109">Permissions</span></span>

<span data-ttu-id="b3827-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3827-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3827-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3827-112">Permission type</span></span>                        | <span data-ttu-id="b3827-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3827-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b3827-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3827-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3827-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3827-115">Not supported.</span></span> |
| <span data-ttu-id="b3827-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3827-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3827-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3827-117">Not supported.</span></span> |
| <span data-ttu-id="b3827-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3827-118">Application</span></span>                            | <span data-ttu-id="b3827-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3827-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3827-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3827-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="b3827-121">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="b3827-121">Path parameters</span></span>

| <span data-ttu-id="b3827-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b3827-122">Parameter</span></span>     | <span data-ttu-id="b3827-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3827-123">Type</span></span>   | <span data-ttu-id="b3827-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3827-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="b3827-125">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="b3827-125">connection-id</span></span> | <span data-ttu-id="b3827-126">string</span><span class="sxs-lookup"><span data-stu-id="b3827-126">string</span></span> | <span data-ttu-id="b3827-127">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="b3827-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="b3827-128">item-id</span><span class="sxs-lookup"><span data-stu-id="b3827-128">item-id</span></span>       | <span data-ttu-id="b3827-129">string</span><span class="sxs-lookup"><span data-stu-id="b3827-129">string</span></span> | <span data-ttu-id="b3827-130">A propriedade fornecida pelo desenvolvedor `id` do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="b3827-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="b3827-131">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b3827-131">Optional query parameters</span></span>

<span data-ttu-id="b3827-132">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b3827-132">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3827-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3827-133">Request headers</span></span>

| <span data-ttu-id="b3827-134">Nome</span><span class="sxs-lookup"><span data-stu-id="b3827-134">Name</span></span>          | <span data-ttu-id="b3827-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3827-135">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b3827-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3827-136">Authorization</span></span> | <span data-ttu-id="b3827-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3827-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3827-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3827-139">Request body</span></span>

<span data-ttu-id="b3827-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3827-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3827-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3827-141">Response</span></span>

<span data-ttu-id="b3827-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [externalItem](../resources/externalitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3827-142">If successful, this method returns a `200 OK` response code and an [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3827-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3827-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3827-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3827-144">Request</span></span>

<span data-ttu-id="b3827-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3827-145">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="b3827-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3827-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="b3827-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3827-147">The following is an example of the response.</span></span>

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
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    },
    {
      "type": "group",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny",
      "identitySource": "external"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "Error in payment gateway...",
    "type": "text"
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
