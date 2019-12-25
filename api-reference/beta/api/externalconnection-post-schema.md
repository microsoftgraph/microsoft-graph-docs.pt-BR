---
title: Criar esquema
description: Crie o esquema para uma conexão do Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 560fc240439ed204e349bb09a44f398925007182
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869742"
---
# <a name="create-schema"></a><span data-ttu-id="2546d-103">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="2546d-103">Create schema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2546d-104">Crie o esquema para uma [conexão](../resources/externalconnection.md)do Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="2546d-104">Create the schema for a Microsoft Search [connection](../resources/externalconnection.md).</span></span>

<span data-ttu-id="2546d-105">Dois tipos de esquema são suportados: itens personalizados e arquivos.</span><span class="sxs-lookup"><span data-stu-id="2546d-105">Two schema types are supported: custom items, and files.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="2546d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2546d-106">Permissions</span></span>

<span data-ttu-id="2546d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2546d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2546d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2546d-109">Permission type</span></span>                        | <span data-ttu-id="2546d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2546d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2546d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2546d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2546d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2546d-112">Not supported.</span></span> |
| <span data-ttu-id="2546d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2546d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2546d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2546d-114">Not supported.</span></span> |
| <span data-ttu-id="2546d-115">Application</span><span class="sxs-lookup"><span data-stu-id="2546d-115">Application</span></span>                            | <span data-ttu-id="2546d-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2546d-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2546d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2546d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections/{id}/schema
```

## <a name="request-headers"></a><span data-ttu-id="2546d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2546d-118">Request headers</span></span>

| <span data-ttu-id="2546d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2546d-119">Name</span></span>                  | <span data-ttu-id="2546d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2546d-120">Description</span></span>                                          |
|:----------------------|:-----------------------------------------------------|
| <span data-ttu-id="2546d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2546d-121">Authorization</span></span>         | <span data-ttu-id="2546d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2546d-p102">Bearer {token}. Required.</span></span>                            |
| <span data-ttu-id="2546d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2546d-124">Content-Type</span></span>          | <span data-ttu-id="2546d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2546d-p103">application/json. Required.</span></span>                          |
| <span data-ttu-id="2546d-127">Prefiro: responder-Async</span><span class="sxs-lookup"><span data-stu-id="2546d-127">Prefer: respond-async</span></span> | <span data-ttu-id="2546d-128">Use isso para fazer com que a solicitação seja executada de forma assíncrona.</span><span class="sxs-lookup"><span data-stu-id="2546d-128">Use this to cause the request to execute asynchronously.</span></span> <span data-ttu-id="2546d-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2546d-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2546d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2546d-130">Request body</span></span>

<span data-ttu-id="2546d-131">No corpo da solicitação, forneça uma representação JSON de um objeto [Schema](../resources/schema.md) .</span><span class="sxs-lookup"><span data-stu-id="2546d-131">In the request body, supply a JSON representation of a [schema](../resources/schema.md) object.</span></span>

<span data-ttu-id="2546d-132">Ao registrar um esquema de item personalizado, o `schema` objeto deve ter a `baseType` propriedade definida como `microsoft.graph.externalItem` e deve conter a `properties` propriedade.</span><span class="sxs-lookup"><span data-stu-id="2546d-132">When registering a custom item schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalItem` and MUST contain the `properties` property.</span></span> <span data-ttu-id="2546d-133">O `properties` objeto deve conter pelo menos uma propriedade, até um máximo de 64.</span><span class="sxs-lookup"><span data-stu-id="2546d-133">The `properties` object must contain at least one property, up to a maximum of 64.</span></span>

<span data-ttu-id="2546d-134">Ao registrar um esquema de arquivos, o `schema` objeto deve ter a `baseType` propriedade definida como `microsoft.graph.externalFile`.</span><span class="sxs-lookup"><span data-stu-id="2546d-134">When registering a file schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalFile`.</span></span>

## <a name="response"></a><span data-ttu-id="2546d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2546d-135">Response</span></span>

<span data-ttu-id="2546d-136">Com o `Prefer: respond-async` cabeçalho incluído na solicitação, se tiver êxito, este método retornará um `202 Accepted` código de resposta e uma URL no `Location` cabeçalho de resposta que pode ser usada para [obter o status da operação](../api/connectionoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="2546d-136">With the `Prefer: respond-async` header included in the request, if successful, this method returns a `202 Accepted` response code and a URL in the `Location` response header that can be used to [get the operation status](../api/connectionoperation-get.md).</span></span>

<span data-ttu-id="2546d-137">Sem o `Prefer: respond-async` cabeçalho incluído na solicitação, se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto de [esquema](../resources/schema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2546d-137">Without the `Prefer: respond-async` header included in the request, if successful, this method returns a `201 Created` response code and a new [schema](../resources/schema.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="2546d-138">A criação de um esquema é um processo de longa execução sujeito a tempos limite de gateway.</span><span class="sxs-lookup"><span data-stu-id="2546d-138">Creating a schema is a long-running process prone to gateway timeouts.</span></span> <span data-ttu-id="2546d-139">Recomendamos usar o `Prefer: respond-async` cabeçalho para evitar erros de tempo limite.</span><span class="sxs-lookup"><span data-stu-id="2546d-139">We recommend using the `Prefer: respond-async` header to avoid timeout errors.</span></span>

## <a name="examples"></a><span data-ttu-id="2546d-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2546d-140">Examples</span></span>

### <a name="example-1-register-custom-schema-asynchronously"></a><span data-ttu-id="2546d-141">Exemplo 1: registrar o esquema personalizado de forma assíncrona</span><span class="sxs-lookup"><span data-stu-id="2546d-141">Example 1: Register custom schema asynchronously</span></span>

#### <a name="request"></a><span data-ttu-id="2546d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2546d-142">Request</span></span>

<span data-ttu-id="2546d-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2546d-143">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2546d-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="2546d-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async"
}-->

```http
POST https://graph.microsoft.com/beta/connections/contosohr/schema
Content-type: application/json
Prefer: respond-async

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "title",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true"
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2546d-145">C#</span><span class="sxs-lookup"><span data-stu-id="2546d-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-async-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2546d-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2546d-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-async-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2546d-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2546d-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-async-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="2546d-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="2546d-148">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="2546d-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2546d-149">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```

### <a name="example-2-register-file-schema-synchronously"></a><span data-ttu-id="2546d-150">Exemplo 2: registrar o esquema de arquivo de forma síncrona</span><span class="sxs-lookup"><span data-stu-id="2546d-150">Example 2: Register file schema synchronously</span></span>

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a><span data-ttu-id="2546d-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2546d-151">Request</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="2546d-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2546d-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2546d-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="2546d-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection"
}-->

```http
POST https://graph.microsoft.com/beta/connections/contosofiles/schema
Content-type: application/json

{
  "baseType": "microsoft.graph.externalFile"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2546d-154">C#</span><span class="sxs-lookup"><span data-stu-id="2546d-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2546d-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2546d-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2546d-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2546d-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="2546d-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="2546d-157">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="2546d-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2546d-158">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schema"
} -->

```http
HTTP/1.1 201 Created

{
  "baseType": "microsoft.graph.externalFile"
}
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
