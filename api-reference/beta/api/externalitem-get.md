---
title: Obter externalItem
description: Obter um externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 2c0bdc7d44e2d9fb5c317ab2eb1cbc71cca76031
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366748"
---
# <a name="get-externalitem"></a><span data-ttu-id="8727a-103">Obter externalItem</span><span class="sxs-lookup"><span data-stu-id="8727a-103">Get externalItem</span></span>

<span data-ttu-id="8727a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8727a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8727a-105">Obter as propriedades e as relações de um [objeto externalitem.](../resources/externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="8727a-105">Get the properties and relationships of an [externalitem](../resources/externalitem.md) object.</span></span>

<span data-ttu-id="8727a-106">Essa API é fornecida apenas para fins de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="8727a-106">This API is provided for diagnostic purposes only.</span></span> <span data-ttu-id="8727a-107">Ele não se destina a ser usado para qualquer outra finalidade.</span><span class="sxs-lookup"><span data-stu-id="8727a-107">It is not intended to be used for any other purpose.</span></span> <span data-ttu-id="8727a-108">Solicitações repetidas para essa API podem resultar em `429` erros HTTP.</span><span class="sxs-lookup"><span data-stu-id="8727a-108">Repeated requests to this API might result in `429` HTTP errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="8727a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8727a-109">Permissions</span></span>

<span data-ttu-id="8727a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8727a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8727a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8727a-112">Permission type</span></span>                        | <span data-ttu-id="8727a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8727a-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8727a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8727a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="8727a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8727a-115">Not supported.</span></span> |
| <span data-ttu-id="8727a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8727a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8727a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8727a-117">Not supported.</span></span> |
| <span data-ttu-id="8727a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8727a-118">Application</span></span>                            | <span data-ttu-id="8727a-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8727a-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8727a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8727a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="8727a-121">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="8727a-121">Path parameters</span></span>

| <span data-ttu-id="8727a-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8727a-122">Parameter</span></span>     | <span data-ttu-id="8727a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="8727a-123">Type</span></span>   | <span data-ttu-id="8727a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8727a-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="8727a-125">connection-id</span><span class="sxs-lookup"><span data-stu-id="8727a-125">connection-id</span></span> | <span data-ttu-id="8727a-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8727a-126">string</span></span> | <span data-ttu-id="8727a-127">A `id` propriedade do [externalConnection que](../resources/externalconnection.md) contém</span><span class="sxs-lookup"><span data-stu-id="8727a-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="8727a-128">item-id</span><span class="sxs-lookup"><span data-stu-id="8727a-128">item-id</span></span>       | <span data-ttu-id="8727a-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8727a-129">string</span></span> | <span data-ttu-id="8727a-130">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="8727a-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="8727a-131">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8727a-131">Optional query parameters</span></span>

<span data-ttu-id="8727a-132">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8727a-132">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8727a-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8727a-133">Request headers</span></span>

| <span data-ttu-id="8727a-134">Nome</span><span class="sxs-lookup"><span data-stu-id="8727a-134">Name</span></span>          | <span data-ttu-id="8727a-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="8727a-135">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8727a-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="8727a-136">Authorization</span></span> | <span data-ttu-id="8727a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8727a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8727a-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8727a-139">Request body</span></span>

<span data-ttu-id="8727a-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8727a-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8727a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8727a-141">Response</span></span>

<span data-ttu-id="8727a-142">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [externalItem](../resources/externalitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8727a-142">If successful, this method returns a `200 OK` response code and an [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8727a-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8727a-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="8727a-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8727a-144">Request</span></span>

<span data-ttu-id="8727a-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8727a-145">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="8727a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8727a-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="8727a-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8727a-147">The following is an example of the response.</span></span>

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
