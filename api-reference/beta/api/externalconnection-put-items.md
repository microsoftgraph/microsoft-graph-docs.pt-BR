---
title: Criar externalItem
description: Criar um novo externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6e0ee2ca2eebcca9b912c62242c2606590d9cbc4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192263"
---
# <a name="create-externalitem"></a><span data-ttu-id="53762-103">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="53762-103">Create externalItem</span></span>

<span data-ttu-id="53762-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53762-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53762-105">Criar um novo [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="53762-105">Create a new [externalItem](../resources/externalitem.md).</span></span>

<span data-ttu-id="53762-106">Essa API pode ser usada para criar um item personalizado.</span><span class="sxs-lookup"><span data-stu-id="53762-106">This API can be used to create a custom item.</span></span> <span data-ttu-id="53762-107">Especifique o tipo que você está criando incluindo a `@odata.type` propriedade no corpo JSON.</span><span class="sxs-lookup"><span data-stu-id="53762-107">Specify the type you are creating by including the `@odata.type` property in the JSON body.</span></span> <span data-ttu-id="53762-108">O [externalConnection](../resources/externalconnection.md) recipiente deve ter um [esquema](../resources/schema.md) registrado do tipo correspondente.</span><span class="sxs-lookup"><span data-stu-id="53762-108">The containing [externalConnection](../resources/externalconnection.md) must have a [schema](../resources/schema.md) registered of the corresponding type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="53762-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="53762-109">Permissions</span></span>

<span data-ttu-id="53762-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53762-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53762-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53762-112">Permission type</span></span>                        | <span data-ttu-id="53762-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53762-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="53762-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53762-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="53762-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53762-115">Not supported.</span></span> |
| <span data-ttu-id="53762-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53762-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53762-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53762-117">Not supported.</span></span> |
| <span data-ttu-id="53762-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53762-118">Application</span></span>                            | <span data-ttu-id="53762-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53762-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53762-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53762-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="53762-121">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="53762-121">Path parameters</span></span>

| <span data-ttu-id="53762-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="53762-122">Parameter</span></span>     | <span data-ttu-id="53762-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="53762-123">Type</span></span>   | <span data-ttu-id="53762-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="53762-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="53762-125">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="53762-125">connection-id</span></span> | <span data-ttu-id="53762-126">string</span><span class="sxs-lookup"><span data-stu-id="53762-126">string</span></span> | <span data-ttu-id="53762-127">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="53762-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="53762-128">item-id</span><span class="sxs-lookup"><span data-stu-id="53762-128">item-id</span></span>       | <span data-ttu-id="53762-129">string</span><span class="sxs-lookup"><span data-stu-id="53762-129">string</span></span> | <span data-ttu-id="53762-130">A propriedade fornecida pelo desenvolvedor `id` do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="53762-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> <span data-ttu-id="53762-131">Se nenhum item já existir com isso `id` , um novo item é criado.</span><span class="sxs-lookup"><span data-stu-id="53762-131">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="53762-132">Se já existir um item com isso `id` , ele será substituído pelo objeto enviado no corpo.</span><span class="sxs-lookup"><span data-stu-id="53762-132">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="53762-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53762-133">Request headers</span></span>

| <span data-ttu-id="53762-134">Nome</span><span class="sxs-lookup"><span data-stu-id="53762-134">Name</span></span>          | <span data-ttu-id="53762-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="53762-135">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="53762-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="53762-136">Authorization</span></span> | <span data-ttu-id="53762-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53762-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="53762-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53762-139">Content-Type</span></span>  | <span data-ttu-id="53762-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53762-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53762-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53762-142">Request body</span></span>

<span data-ttu-id="53762-143">No corpo da solicitação, forneça uma representação JSON de um objeto [externalItem](../resources/externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="53762-143">In the request body, supply a JSON representation of an [externalItem](../resources/externalitem.md) object.</span></span> <span data-ttu-id="53762-144">A carga é limitada a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="53762-144">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="53762-145">Criar um externalItem</span><span class="sxs-lookup"><span data-stu-id="53762-145">Creating an externalItem</span></span>

<span data-ttu-id="53762-146">Ao criar um `externalItem` , os campos a seguir são obrigatórios: `@odata.type` , `acl` e `properties` .</span><span class="sxs-lookup"><span data-stu-id="53762-146">When creating an `externalItem`, the following fields are required: `@odata.type`, `acl`, and `properties`.</span></span> <span data-ttu-id="53762-147">O `properties` objeto deve conter pelo menos uma propriedade.</span><span class="sxs-lookup"><span data-stu-id="53762-147">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="53762-148">Todas as `DateTime` Propriedades de tipo devem estar no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="53762-148">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="53762-149">As propriedades em um `externalItem` devem usar especificadores de tipo na carga nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="53762-149">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="53762-150">Para `String` Propriedades de tipo, se o valor contiver caracteres não-ASCII.</span><span class="sxs-lookup"><span data-stu-id="53762-150">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="53762-151">Para todos os tipos de coleção.</span><span class="sxs-lookup"><span data-stu-id="53762-151">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="53762-152">Ao incluir uma propriedade de tipo `Collection(DateTime)` , você deve usar o especificador de tipo `Collection(DateTimeOffset)` .</span><span class="sxs-lookup"><span data-stu-id="53762-152">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

## <a name="response"></a><span data-ttu-id="53762-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="53762-153">Response</span></span>

<span data-ttu-id="53762-154">Quando é bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="53762-154">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="53762-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="53762-155">Examples</span></span>

### <a name="example-create-a-custom-item"></a><span data-ttu-id="53762-156">Exemplo: criar um item personalizado</span><span class="sxs-lookup"><span data-stu-id="53762-156">Example: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="53762-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53762-157">Request</span></span>

<span data-ttu-id="53762-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="53762-158">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53762-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="53762-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="53762-160">C#</span><span class="sxs-lookup"><span data-stu-id="53762-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53762-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53762-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53762-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53762-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="53762-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="53762-163">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="53762-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="53762-164">The following is an example of the response.</span></span>

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
