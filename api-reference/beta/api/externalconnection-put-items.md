---
title: Criar externalItem
description: Criar um novo externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 298a5bc01b3891831e1a8fd6774d721dc977b940
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869771"
---
# <a name="create-externalitem"></a><span data-ttu-id="46207-103">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="46207-103">Create externalItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46207-104">Crie um novo [externalItem](../resources/externalitem.md) ou [externalfile](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="46207-104">Create a new [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

<span data-ttu-id="46207-105">Essa API pode ser usada para criar um item personalizado ou um arquivo.</span><span class="sxs-lookup"><span data-stu-id="46207-105">This API can be used to create a custom item or a file.</span></span> <span data-ttu-id="46207-106">Especifique o tipo que você está criando incluindo a `@odata.type` Propriedade no corpo JSON.</span><span class="sxs-lookup"><span data-stu-id="46207-106">Specify the type you are creating by including the `@odata.type` property in the JSON body.</span></span> <span data-ttu-id="46207-107">O [externalConnection](../resources/externalconnection.md) recipiente deve ter um [esquema](../resources/schema.md) registrado do tipo correspondente.</span><span class="sxs-lookup"><span data-stu-id="46207-107">The containing [externalConnection](../resources/externalconnection.md) must have a [schema](../resources/schema.md) registered of the corresponding type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="46207-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="46207-108">Permissions</span></span>

<span data-ttu-id="46207-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46207-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46207-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46207-111">Permission type</span></span>                        | <span data-ttu-id="46207-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46207-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="46207-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46207-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="46207-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46207-114">Not supported.</span></span> |
| <span data-ttu-id="46207-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46207-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46207-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46207-116">Not supported.</span></span> |
| <span data-ttu-id="46207-117">Application</span><span class="sxs-lookup"><span data-stu-id="46207-117">Application</span></span>                            | <span data-ttu-id="46207-118">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46207-118">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46207-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46207-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="46207-120">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="46207-120">Path parameters</span></span>

| <span data-ttu-id="46207-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="46207-121">Parameter</span></span>     | <span data-ttu-id="46207-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="46207-122">Type</span></span>   | <span data-ttu-id="46207-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="46207-123">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="46207-124">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="46207-124">connection-id</span></span> | <span data-ttu-id="46207-125">string</span><span class="sxs-lookup"><span data-stu-id="46207-125">string</span></span> | <span data-ttu-id="46207-126">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="46207-126">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="46207-127">item-id</span><span class="sxs-lookup"><span data-stu-id="46207-127">item-id</span></span>       | <span data-ttu-id="46207-128">string</span><span class="sxs-lookup"><span data-stu-id="46207-128">string</span></span> | <span data-ttu-id="46207-129">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalitem.md) ou do [externalfile](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="46207-129">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> <span data-ttu-id="46207-130">Se nenhum item já existir com isso `id`, um novo item é criado.</span><span class="sxs-lookup"><span data-stu-id="46207-130">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="46207-131">Se já existir um item com isso `id`, ele será substituído pelo objeto enviado no corpo.</span><span class="sxs-lookup"><span data-stu-id="46207-131">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="46207-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46207-132">Request headers</span></span>

| <span data-ttu-id="46207-133">Nome</span><span class="sxs-lookup"><span data-stu-id="46207-133">Name</span></span>          | <span data-ttu-id="46207-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="46207-134">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="46207-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="46207-135">Authorization</span></span> | <span data-ttu-id="46207-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46207-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="46207-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46207-138">Content-Type</span></span>  | <span data-ttu-id="46207-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46207-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46207-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46207-141">Request body</span></span>

<span data-ttu-id="46207-142">No corpo da solicitação, forneça uma representação JSON de um objeto [externalItem](../resources/externalitem.md) ou [externalfile](../resources/externalfile.md) .</span><span class="sxs-lookup"><span data-stu-id="46207-142">In the request body, supply a JSON representation of an [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md) object.</span></span> <span data-ttu-id="46207-143">A carga é limitada a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="46207-143">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="46207-144">Criar um externalItem</span><span class="sxs-lookup"><span data-stu-id="46207-144">Creating an externalItem</span></span>

<span data-ttu-id="46207-145">Ao criar um `externalItem`, os campos a seguir são `@odata.type`obrigatórios `acl`:, `properties`e.</span><span class="sxs-lookup"><span data-stu-id="46207-145">When creating an `externalItem`, the following fields are required: `@odata.type`, `acl`, and `properties`.</span></span> <span data-ttu-id="46207-146">O `properties` objeto deve conter pelo menos uma propriedade.</span><span class="sxs-lookup"><span data-stu-id="46207-146">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="46207-147">Todas `DateTime` as propriedades de tipo devem estar no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="46207-147">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="46207-148">As propriedades em `externalItem` um devem usar especificadores de tipo na carga nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="46207-148">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="46207-149">Para `String` Propriedades de tipo, se o valor contiver caracteres não-ASCII.</span><span class="sxs-lookup"><span data-stu-id="46207-149">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="46207-150">Para todos os tipos de coleção.</span><span class="sxs-lookup"><span data-stu-id="46207-150">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="46207-151">Ao incluir uma propriedade de tipo `Collection(DateTime)`, você deve usar o especificador `Collection(DateTimeOffset)`de tipo.</span><span class="sxs-lookup"><span data-stu-id="46207-151">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

### <a name="creating-an-externalfile"></a><span data-ttu-id="46207-152">Criando um externalfile</span><span class="sxs-lookup"><span data-stu-id="46207-152">Creating an externalFile</span></span>

<span data-ttu-id="46207-153">Ao criar um `externalFile`, os campos a seguir são obrigatórios `acl`: `name` `@odata.type`,, `url`e.</span><span class="sxs-lookup"><span data-stu-id="46207-153">When creating an `externalFile`, the following fields are required: `@odata.type`, `acl`, `name`, and `url`.</span></span>

## <a name="response"></a><span data-ttu-id="46207-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="46207-154">Response</span></span>

<span data-ttu-id="46207-155">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="46207-155">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="46207-156">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46207-156">Examples</span></span>

### <a name="example-1-create-a-custom-item"></a><span data-ttu-id="46207-157">Exemplo 1: criar um item personalizado</span><span class="sxs-lookup"><span data-stu-id="46207-157">Example 1: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="46207-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46207-158">Request</span></span>

<span data-ttu-id="46207-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="46207-159">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="46207-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="46207-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
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
  "content": "Textual content of the file"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46207-161">C#</span><span class="sxs-lookup"><span data-stu-id="46207-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46207-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46207-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46207-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46207-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="46207-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="46207-164">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="46207-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="46207-165">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

### <a name="example-2-create-a-file"></a><span data-ttu-id="46207-166">Exemplo 2: criar um arquivo</span><span class="sxs-lookup"><span data-stu-id="46207-166">Example 2: Create a file</span></span>

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a><span data-ttu-id="46207-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46207-167">Request</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="46207-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="46207-168">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="46207-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="46207-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalfile_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/connections/contosofiles/items/myFile01
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalFile",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "grant",
      "identitySource": "Azure Active Directory"
    }
  ],
  "createdDateTime": "2019-01-31T03:44:19.0354159Z",
  "modifiedDateTime": "2019-01-31T03:44:19.0354159Z",
  "createdBy": "Pradeep Gupta",
  "lastModifiedBy": "Adele Vance",
  "title": "Enterprise Search Graph Ingestion API",
  "url": "file://filesrv02.corp.contoso.com/data/project/Enterprise Search.docx",
  "name": "Enterprise Search.docx",
  "extension": "docx",
  "size": 8676776,
  "content": "The quick brown fox jumps over the lazy dog."
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46207-170">C#</span><span class="sxs-lookup"><span data-stu-id="46207-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalfile-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46207-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46207-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalfile-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46207-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46207-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalfile-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="46207-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="46207-173">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="46207-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="46207-174">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
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
