---
title: Obter externalItem
description: Obter um externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 0e668c6ee1d571287304e0920a4636c81cd06ca7
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45005135"
---
# <a name="get-externalitem"></a><span data-ttu-id="c0f89-103">Obter externalItem</span><span class="sxs-lookup"><span data-stu-id="c0f89-103">Get externalItem</span></span>

<span data-ttu-id="c0f89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0f89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0f89-105">Obtenha as propriedades e os relacionamentos de um objeto [externalitem](../resources/externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="c0f89-105">Get the properties and relationships of an [externalitem](../resources/externalitem.md) object.</span></span>

<span data-ttu-id="c0f89-106">Essa API é fornecida apenas para fins de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="c0f89-106">This API is provided for diagnostic purposes only.</span></span> <span data-ttu-id="c0f89-107">Ele não se destina a ser usado para qualquer outra finalidade.</span><span class="sxs-lookup"><span data-stu-id="c0f89-107">It is not intended to be used for any other purpose.</span></span> <span data-ttu-id="c0f89-108">Solicitações repetidas para essa API podem resultar em `429` erros http.</span><span class="sxs-lookup"><span data-stu-id="c0f89-108">Repeated requests to this API might result in `429` HTTP errors.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="c0f89-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0f89-109">Permissions</span></span>

<span data-ttu-id="c0f89-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c0f89-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c0f89-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0f89-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0f89-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0f89-112">Permission type</span></span>                        | <span data-ttu-id="c0f89-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0f89-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c0f89-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0f89-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0f89-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0f89-115">Not supported.</span></span> |
| <span data-ttu-id="c0f89-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0f89-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0f89-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0f89-117">Not supported.</span></span> |
| <span data-ttu-id="c0f89-118">Application</span><span class="sxs-lookup"><span data-stu-id="c0f89-118">Application</span></span>                            | <span data-ttu-id="c0f89-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0f89-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0f89-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0f89-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="c0f89-121">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="c0f89-121">Path parameters</span></span>

| <span data-ttu-id="c0f89-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c0f89-122">Parameter</span></span>     | <span data-ttu-id="c0f89-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0f89-123">Type</span></span>   | <span data-ttu-id="c0f89-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0f89-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="c0f89-125">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="c0f89-125">connection-id</span></span> | <span data-ttu-id="c0f89-126">string</span><span class="sxs-lookup"><span data-stu-id="c0f89-126">string</span></span> | <span data-ttu-id="c0f89-127">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="c0f89-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="c0f89-128">item-id</span><span class="sxs-lookup"><span data-stu-id="c0f89-128">item-id</span></span>       | <span data-ttu-id="c0f89-129">string</span><span class="sxs-lookup"><span data-stu-id="c0f89-129">string</span></span> | <span data-ttu-id="c0f89-130">A propriedade fornecida pelo desenvolvedor `id` do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="c0f89-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="c0f89-131">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c0f89-131">Optional query parameters</span></span>

<span data-ttu-id="c0f89-132">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c0f89-132">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0f89-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0f89-133">Request headers</span></span>

| <span data-ttu-id="c0f89-134">Nome</span><span class="sxs-lookup"><span data-stu-id="c0f89-134">Name</span></span>          | <span data-ttu-id="c0f89-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0f89-135">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c0f89-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0f89-136">Authorization</span></span> | <span data-ttu-id="c0f89-137">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="c0f89-137">Bearer {token}.</span></span> <span data-ttu-id="c0f89-138">Required.</span><span class="sxs-lookup"><span data-stu-id="c0f89-138">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0f89-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0f89-139">Request body</span></span>

<span data-ttu-id="c0f89-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0f89-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0f89-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0f89-141">Response</span></span>

<span data-ttu-id="c0f89-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [externalItem](../resources/externalitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0f89-142">If successful, this method returns a `200 OK` response code and an [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0f89-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0f89-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0f89-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0f89-144">Request</span></span>

<span data-ttu-id="c0f89-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0f89-145">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="c0f89-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0f89-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="c0f89-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c0f89-147">The following is an example of the response.</span></span>

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
      "identitySource": "Azure Active Directory"
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
