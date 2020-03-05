---
title: Criar externalItem
description: Criar um novo externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 8b75e3753555e840b042e8876f91e27ed77b4a76
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422051"
---
# <a name="create-externalitem"></a><span data-ttu-id="6417e-103">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="6417e-103">Create externalItem</span></span>

<span data-ttu-id="6417e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6417e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6417e-105">Crie um novo [externalItem](../resources/externalitem.md) ou [externalfile](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="6417e-105">Create a new [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

<span data-ttu-id="6417e-106">Essa API pode ser usada para criar um item personalizado ou um arquivo.</span><span class="sxs-lookup"><span data-stu-id="6417e-106">This API can be used to create a custom item or a file.</span></span> <span data-ttu-id="6417e-107">Especifique o tipo que você está criando incluindo a `@odata.type` Propriedade no corpo JSON.</span><span class="sxs-lookup"><span data-stu-id="6417e-107">Specify the type you are creating by including the `@odata.type` property in the JSON body.</span></span> <span data-ttu-id="6417e-108">O [externalConnection](../resources/externalconnection.md) recipiente deve ter um [esquema](../resources/schema.md) registrado do tipo correspondente.</span><span class="sxs-lookup"><span data-stu-id="6417e-108">The containing [externalConnection](../resources/externalconnection.md) must have a [schema](../resources/schema.md) registered of the corresponding type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="6417e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="6417e-109">Permissions</span></span>

<span data-ttu-id="6417e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6417e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6417e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6417e-112">Permission type</span></span>                        | <span data-ttu-id="6417e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6417e-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6417e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6417e-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="6417e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6417e-115">Not supported.</span></span> |
| <span data-ttu-id="6417e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6417e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6417e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6417e-117">Not supported.</span></span> |
| <span data-ttu-id="6417e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6417e-118">Application</span></span>                            | <span data-ttu-id="6417e-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6417e-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6417e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6417e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="6417e-121">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="6417e-121">Path parameters</span></span>

| <span data-ttu-id="6417e-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6417e-122">Parameter</span></span>     | <span data-ttu-id="6417e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="6417e-123">Type</span></span>   | <span data-ttu-id="6417e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6417e-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="6417e-125">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="6417e-125">connection-id</span></span> | <span data-ttu-id="6417e-126">string</span><span class="sxs-lookup"><span data-stu-id="6417e-126">string</span></span> | <span data-ttu-id="6417e-127">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="6417e-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="6417e-128">item-id</span><span class="sxs-lookup"><span data-stu-id="6417e-128">item-id</span></span>       | <span data-ttu-id="6417e-129">string</span><span class="sxs-lookup"><span data-stu-id="6417e-129">string</span></span> | <span data-ttu-id="6417e-130">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalitem.md) ou do [externalfile](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="6417e-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> <span data-ttu-id="6417e-131">Se nenhum item já existir com isso `id`, um novo item é criado.</span><span class="sxs-lookup"><span data-stu-id="6417e-131">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="6417e-132">Se já existir um item com isso `id`, ele será substituído pelo objeto enviado no corpo.</span><span class="sxs-lookup"><span data-stu-id="6417e-132">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6417e-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6417e-133">Request headers</span></span>

| <span data-ttu-id="6417e-134">Nome</span><span class="sxs-lookup"><span data-stu-id="6417e-134">Name</span></span>          | <span data-ttu-id="6417e-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="6417e-135">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="6417e-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="6417e-136">Authorization</span></span> | <span data-ttu-id="6417e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6417e-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="6417e-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6417e-139">Content-Type</span></span>  | <span data-ttu-id="6417e-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6417e-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6417e-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6417e-142">Request body</span></span>

<span data-ttu-id="6417e-143">No corpo da solicitação, forneça uma representação JSON de um objeto [externalItem](../resources/externalitem.md) ou [externalfile](../resources/externalfile.md) .</span><span class="sxs-lookup"><span data-stu-id="6417e-143">In the request body, supply a JSON representation of an [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md) object.</span></span> <span data-ttu-id="6417e-144">A carga é limitada a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="6417e-144">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="6417e-145">Criar um externalItem</span><span class="sxs-lookup"><span data-stu-id="6417e-145">Creating an externalItem</span></span>

<span data-ttu-id="6417e-146">Ao criar um `externalItem`, os campos a seguir são `@odata.type`obrigatórios `acl`:, `properties`e.</span><span class="sxs-lookup"><span data-stu-id="6417e-146">When creating an `externalItem`, the following fields are required: `@odata.type`, `acl`, and `properties`.</span></span> <span data-ttu-id="6417e-147">O `properties` objeto deve conter pelo menos uma propriedade.</span><span class="sxs-lookup"><span data-stu-id="6417e-147">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="6417e-148">Todas `DateTime` as propriedades de tipo devem estar no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="6417e-148">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="6417e-149">As propriedades em `externalItem` um devem usar especificadores de tipo na carga nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="6417e-149">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="6417e-150">Para `String` Propriedades de tipo, se o valor contiver caracteres não-ASCII.</span><span class="sxs-lookup"><span data-stu-id="6417e-150">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="6417e-151">Para todos os tipos de coleção.</span><span class="sxs-lookup"><span data-stu-id="6417e-151">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="6417e-152">Ao incluir uma propriedade de tipo `Collection(DateTime)`, você deve usar o especificador `Collection(DateTimeOffset)`de tipo.</span><span class="sxs-lookup"><span data-stu-id="6417e-152">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

### <a name="creating-an-externalfile"></a><span data-ttu-id="6417e-153">Criando um externalfile</span><span class="sxs-lookup"><span data-stu-id="6417e-153">Creating an externalFile</span></span>

<span data-ttu-id="6417e-154">Ao criar um `externalFile`, os campos a seguir são obrigatórios `acl`: `name` `@odata.type`,, `url`e.</span><span class="sxs-lookup"><span data-stu-id="6417e-154">When creating an `externalFile`, the following fields are required: `@odata.type`, `acl`, `name`, and `url`.</span></span>

## <a name="response"></a><span data-ttu-id="6417e-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="6417e-155">Response</span></span>

<span data-ttu-id="6417e-156">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="6417e-156">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6417e-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6417e-157">Examples</span></span>

### <a name="example-1-create-a-custom-item"></a><span data-ttu-id="6417e-158">Exemplo 1: criar um item personalizado</span><span class="sxs-lookup"><span data-stu-id="6417e-158">Example 1: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="6417e-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6417e-159">Request</span></span>

<span data-ttu-id="6417e-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6417e-160">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6417e-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="6417e-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6417e-162">C#</span><span class="sxs-lookup"><span data-stu-id="6417e-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6417e-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6417e-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6417e-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6417e-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="6417e-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="6417e-165">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="6417e-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6417e-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

### <a name="example-2-create-a-file"></a><span data-ttu-id="6417e-167">Exemplo 2: criar um arquivo</span><span class="sxs-lookup"><span data-stu-id="6417e-167">Example 2: Create a file</span></span>

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a><span data-ttu-id="6417e-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6417e-168">Request</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="6417e-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6417e-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6417e-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="6417e-170">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6417e-171">C#</span><span class="sxs-lookup"><span data-stu-id="6417e-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalfile-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6417e-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6417e-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalfile-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6417e-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6417e-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalfile-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="6417e-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="6417e-174">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="6417e-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6417e-175">The following is an example of the response.</span></span>

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
