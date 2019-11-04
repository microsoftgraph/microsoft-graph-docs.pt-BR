---
title: Criar esquema
description: Crie o esquema para uma conexão do Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 98ccc34bc2e2f26223439a8f87e70ceff3b1589f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938650"
---
# <a name="create-schema"></a><span data-ttu-id="7b474-103">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="7b474-103">Create schema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b474-104">Crie o esquema para uma [conexão](../resources/externalconnection.md)do Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="7b474-104">Create the schema for a Microsoft Search [connection](../resources/externalconnection.md).</span></span>

<span data-ttu-id="7b474-105">Há dois tipos de esquema compatíveis: itens personalizados e arquivos.</span><span class="sxs-lookup"><span data-stu-id="7b474-105">There are two schema types supported: custom items, and files.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b474-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b474-106">Permissions</span></span>

<span data-ttu-id="7b474-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b474-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b474-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b474-109">Permission type</span></span>                        | <span data-ttu-id="7b474-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b474-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7b474-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b474-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b474-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b474-112">Not supported.</span></span> |
| <span data-ttu-id="7b474-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b474-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b474-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b474-114">Not supported.</span></span> |
| <span data-ttu-id="7b474-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b474-115">Application</span></span>                            | <span data-ttu-id="7b474-116">ExternalItem. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7b474-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b474-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b474-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections/{id}/schema
```

## <a name="request-headers"></a><span data-ttu-id="7b474-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b474-118">Request headers</span></span>

| <span data-ttu-id="7b474-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7b474-119">Name</span></span>                  | <span data-ttu-id="7b474-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b474-120">Description</span></span>                                          |
|:----------------------|:-----------------------------------------------------|
| <span data-ttu-id="7b474-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b474-121">Authorization</span></span>         | <span data-ttu-id="7b474-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b474-p102">Bearer {token}. Required.</span></span>                            |
| <span data-ttu-id="7b474-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b474-124">Content-Type</span></span>          | <span data-ttu-id="7b474-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b474-p103">application/json. Required.</span></span>                          |
| <span data-ttu-id="7b474-127">Prefiro: responder-Async</span><span class="sxs-lookup"><span data-stu-id="7b474-127">Prefer: respond-async</span></span> | <span data-ttu-id="7b474-128">Use isso para fazer com que a solicitação seja executada de forma assíncrona.</span><span class="sxs-lookup"><span data-stu-id="7b474-128">Use this to cause the request to execute asynchronously.</span></span> <span data-ttu-id="7b474-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7b474-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b474-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b474-130">Request body</span></span>

<span data-ttu-id="7b474-131">No corpo da solicitação, forneça uma representação JSON de um objeto [Schema](../resources/schema.md) .</span><span class="sxs-lookup"><span data-stu-id="7b474-131">In the request body, supply a JSON representation of a [schema](../resources/schema.md) object.</span></span>

<span data-ttu-id="7b474-132">Ao registrar um esquema de item personalizado, o `schema` objeto deve ter a `baseType` propriedade definida como `microsoft.graph.externalItem` e deve conter a `properties` propriedade.</span><span class="sxs-lookup"><span data-stu-id="7b474-132">When registering a custom item schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalItem` and MUST contain the `properties` property.</span></span> <span data-ttu-id="7b474-133">O `properties` objeto deve conter pelo menos uma propriedade, até um máximo de 64.</span><span class="sxs-lookup"><span data-stu-id="7b474-133">The `properties` object must contain at least one property, up to a maximum of 64.</span></span>

<span data-ttu-id="7b474-134">Ao registrar um esquema de arquivos, o `schema` objeto deve ter a `baseType` propriedade definida como `microsoft.graph.externalFile`.</span><span class="sxs-lookup"><span data-stu-id="7b474-134">When registering a file schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalFile`.</span></span>

## <a name="response"></a><span data-ttu-id="7b474-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b474-135">Response</span></span>

<span data-ttu-id="7b474-136">Com o `Prefer: respond-async` cabeçalho incluído na solicitação, se tiver êxito, este método retornará um `202 Accepted` código de resposta e uma URL no `Location` cabeçalho de resposta que pode ser usada para [obter o status da operação](../api/connectionoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="7b474-136">With the `Prefer: respond-async` header included in the request, if successful, this method returns a `202 Accepted` response code and a URL in the `Location` response header that can be used to [get the operation status](../api/connectionoperation-get.md).</span></span>

<span data-ttu-id="7b474-137">Sem o `Prefer: respond-async` cabeçalho incluído na solicitação, se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto de [esquema](../resources/schema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b474-137">Without the `Prefer: respond-async` header included in the request, if successful, this method returns a `201 Created` response code and a new [schema](../resources/schema.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="7b474-138">A criação de um esquema é um processo de longa execução sujeito a tempos limite de gateway.</span><span class="sxs-lookup"><span data-stu-id="7b474-138">Creating a schema is a long-running process prone to gateway timeouts.</span></span> <span data-ttu-id="7b474-139">O uso `Prefer: respond-async` do é recomendado para evitar erros de tempo limite.</span><span class="sxs-lookup"><span data-stu-id="7b474-139">Using the `Prefer: respond-async` is recommended to avoid timeout errors.</span></span>

## <a name="examples"></a><span data-ttu-id="7b474-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7b474-140">Examples</span></span>

### <a name="example-1-register-custom-schema-asynchronously"></a><span data-ttu-id="7b474-141">Exemplo 1: registrar o esquema personalizado de forma assíncrona</span><span class="sxs-lookup"><span data-stu-id="7b474-141">Example 1: Register custom schema asynchronously</span></span>

#### <a name="request"></a><span data-ttu-id="7b474-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b474-142">Request</span></span>

<span data-ttu-id="7b474-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b474-143">The following is an example of the request.</span></span>
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

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="7b474-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b474-144">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="7b474-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7b474-145">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```

### <a name="example-2-register-file-schema-synchronously"></a><span data-ttu-id="7b474-146">Exemplo 2: registrar o esquema de arquivo de forma síncrona</span><span class="sxs-lookup"><span data-stu-id="7b474-146">Example 2: Register file schema synchronously</span></span>

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a><span data-ttu-id="7b474-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b474-147">Request</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="7b474-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b474-148">The following is an example of the request.</span></span>
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

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="7b474-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b474-149">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="7b474-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7b474-150">The following is an example of the response.</span></span>

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
