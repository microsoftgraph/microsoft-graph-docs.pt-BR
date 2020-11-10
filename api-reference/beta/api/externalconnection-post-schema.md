---
title: Criar esquema
description: Crie o esquema para uma conexão do Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 27820a392d0a37363f447609713f86df1affef15
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965584"
---
# <a name="create-schema"></a><span data-ttu-id="831c1-103">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="831c1-103">Create schema</span></span>

<span data-ttu-id="831c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="831c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="831c1-105">Crie o esquema para uma [conexão](../resources/externalconnection.md)do Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="831c1-105">Create the schema for a Microsoft Search [connection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="831c1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="831c1-106">Permissions</span></span>

<span data-ttu-id="831c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="831c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="831c1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="831c1-109">Permission type</span></span>                        | <span data-ttu-id="831c1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="831c1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="831c1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="831c1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="831c1-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="831c1-112">Not supported.</span></span> |
| <span data-ttu-id="831c1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="831c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="831c1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="831c1-114">Not supported.</span></span> |
| <span data-ttu-id="831c1-115">Application</span><span class="sxs-lookup"><span data-stu-id="831c1-115">Application</span></span>                            | <span data-ttu-id="831c1-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="831c1-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="831c1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="831c1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections/{id}/schema
```

## <a name="request-headers"></a><span data-ttu-id="831c1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="831c1-118">Request headers</span></span>

| <span data-ttu-id="831c1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="831c1-119">Name</span></span>                  | <span data-ttu-id="831c1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="831c1-120">Description</span></span>                                                        |
|:----------------------|:-------------------------------------------------------------------|
| <span data-ttu-id="831c1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="831c1-121">Authorization</span></span>         | <span data-ttu-id="831c1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="831c1-p102">Bearer {token}. Required.</span></span>                                          |
| <span data-ttu-id="831c1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="831c1-124">Content-Type</span></span>          | <span data-ttu-id="831c1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="831c1-p103">application/json. Required.</span></span>                                        |
| <span data-ttu-id="831c1-127">Prefiro: responder-Async</span><span class="sxs-lookup"><span data-stu-id="831c1-127">Prefer: respond-async</span></span> | <span data-ttu-id="831c1-128">Use isso para fazer com que a solicitação seja executada de forma assíncrona.</span><span class="sxs-lookup"><span data-stu-id="831c1-128">Use this to cause the request to execute asynchronously.</span></span> <span data-ttu-id="831c1-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="831c1-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="831c1-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="831c1-130">Request body</span></span>

<span data-ttu-id="831c1-131">No corpo da solicitação, forneça uma representação JSON de um objeto [Schema](../resources/schema.md) .</span><span class="sxs-lookup"><span data-stu-id="831c1-131">In the request body, supply a JSON representation of a [schema](../resources/schema.md) object.</span></span>

<span data-ttu-id="831c1-132">Ao registrar um esquema de item personalizado, o `schema` objeto deve ter a `baseType` propriedade definida como `microsoft.graph.externalItem` e deve conter a `properties` propriedade.</span><span class="sxs-lookup"><span data-stu-id="831c1-132">When registering a custom item schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalItem` and MUST contain the `properties` property.</span></span> <span data-ttu-id="831c1-133">O `properties` objeto deve conter pelo menos uma propriedade, até um máximo de 64.</span><span class="sxs-lookup"><span data-stu-id="831c1-133">The `properties` object must contain at least one property, up to a maximum of 64.</span></span>

## <a name="response"></a><span data-ttu-id="831c1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="831c1-134">Response</span></span>

<span data-ttu-id="831c1-135">Com o `Prefer: respond-async` cabeçalho incluído na solicitação, se tiver êxito, este método retornará um `202 Accepted` código de resposta e uma URL no `Location` cabeçalho de resposta que pode ser usada para [obter o status da operação](../api/connectionoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="831c1-135">With the `Prefer: respond-async` header included in the request, if successful, this method returns a `202 Accepted` response code and a URL in the `Location` response header that can be used to [get the operation status](../api/connectionoperation-get.md).</span></span>

<span data-ttu-id="831c1-136">Sem o `Prefer: respond-async` cabeçalho incluído na solicitação, se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto de [esquema](../resources/schema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="831c1-136">Without the `Prefer: respond-async` header included in the request, if successful, this method returns a `201 Created` response code and a new [schema](../resources/schema.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="831c1-137">A criação de um esquema é um processo de longa execução sujeito a tempos limite de gateway.</span><span class="sxs-lookup"><span data-stu-id="831c1-137">Creating a schema is a long-running process prone to gateway timeouts.</span></span> <span data-ttu-id="831c1-138">Recomendamos usar o `Prefer: respond-async` cabeçalho para evitar erros de tempo limite.</span><span class="sxs-lookup"><span data-stu-id="831c1-138">We recommend using the `Prefer: respond-async` header to avoid timeout errors.</span></span>

## <a name="examples"></a><span data-ttu-id="831c1-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="831c1-139">Examples</span></span>

### <a name="example-register-custom-schema-asynchronously"></a><span data-ttu-id="831c1-140">Exemplo: registrar esquema personalizado de forma assíncrona</span><span class="sxs-lookup"><span data-stu-id="831c1-140">Example: Register custom schema asynchronously</span></span>

#### <a name="request"></a><span data-ttu-id="831c1-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="831c1-141">Request</span></span>

<span data-ttu-id="831c1-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="831c1-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="831c1-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="831c1-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async"
}-->

```http
POST https://graph.microsoft.com/beta/external/connections/contosohr/schema
Content-type: application/json
Prefer: respond-async

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true",
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true",
      "isSearchable": "false"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="831c1-144">C#</span><span class="sxs-lookup"><span data-stu-id="831c1-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-async-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="831c1-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="831c1-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-async-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="831c1-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="831c1-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-async-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="831c1-147">Java</span><span class="sxs-lookup"><span data-stu-id="831c1-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schema-from-connection-async-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="831c1-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="831c1-148">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="831c1-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="831c1-149">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


