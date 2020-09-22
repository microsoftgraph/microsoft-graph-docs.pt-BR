---
title: Criar externalItem
description: Criar um novo externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: acbc931f5fb5293d0b073623b43a8df319838644
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006829"
---
# <a name="create-externalitem"></a><span data-ttu-id="cd2f7-103">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="cd2f7-103">Create externalItem</span></span>

<span data-ttu-id="cd2f7-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="cd2f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd2f7-105">Criar um novo [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="cd2f7-105">Create a new [externalItem](../resources/externalitem.md).</span></span>

<span data-ttu-id="cd2f7-106">Essa API pode ser usada para criar um item personalizado.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-106">This API can be used to create a custom item.</span></span> <span data-ttu-id="cd2f7-107">Especifique o tipo que você está criando incluindo a `@odata.type` propriedade no corpo JSON.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-107">Specify the type you are creating by including the `@odata.type` property in the JSON body.</span></span> <span data-ttu-id="cd2f7-108">O [externalConnection](../resources/externalconnection.md) recipiente deve ter um [esquema](../resources/schema.md) registrado do tipo correspondente.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-108">The containing [externalConnection](../resources/externalconnection.md) must have a [schema](../resources/schema.md) registered of the corresponding type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="cd2f7-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd2f7-109">Permissions</span></span>

<span data-ttu-id="cd2f7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd2f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cd2f7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd2f7-112">Permission type</span></span>                        | <span data-ttu-id="cd2f7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd2f7-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cd2f7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd2f7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd2f7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-115">Not supported.</span></span> |
| <span data-ttu-id="cd2f7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd2f7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd2f7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-117">Not supported.</span></span> |
| <span data-ttu-id="cd2f7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd2f7-118">Application</span></span>                            | <span data-ttu-id="cd2f7-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd2f7-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd2f7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd2f7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="cd2f7-121">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="cd2f7-121">Path parameters</span></span>

| <span data-ttu-id="cd2f7-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cd2f7-122">Parameter</span></span>     | <span data-ttu-id="cd2f7-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd2f7-123">Type</span></span>   | <span data-ttu-id="cd2f7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd2f7-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="cd2f7-125">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="cd2f7-125">connection-id</span></span> | <span data-ttu-id="cd2f7-126">string</span><span class="sxs-lookup"><span data-stu-id="cd2f7-126">string</span></span> | <span data-ttu-id="cd2f7-127">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="cd2f7-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="cd2f7-128">item-id</span><span class="sxs-lookup"><span data-stu-id="cd2f7-128">item-id</span></span>       | <span data-ttu-id="cd2f7-129">string</span><span class="sxs-lookup"><span data-stu-id="cd2f7-129">string</span></span> | <span data-ttu-id="cd2f7-130">A propriedade fornecida pelo desenvolvedor `id` do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="cd2f7-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> <span data-ttu-id="cd2f7-131">Se nenhum item já existir com isso `id` , um novo item é criado.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-131">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="cd2f7-132">Se já existir um item com isso `id` , ele será substituído pelo objeto enviado no corpo.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-132">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="cd2f7-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd2f7-133">Request headers</span></span>

| <span data-ttu-id="cd2f7-134">Nome</span><span class="sxs-lookup"><span data-stu-id="cd2f7-134">Name</span></span>          | <span data-ttu-id="cd2f7-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd2f7-135">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="cd2f7-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd2f7-136">Authorization</span></span> | <span data-ttu-id="cd2f7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="cd2f7-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd2f7-139">Content-Type</span></span>  | <span data-ttu-id="cd2f7-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd2f7-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd2f7-142">Request body</span></span>

<span data-ttu-id="cd2f7-143">No corpo da solicitação, forneça uma representação JSON de um objeto [externalItem](../resources/externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="cd2f7-143">In the request body, supply a JSON representation of an [externalItem](../resources/externalitem.md) object.</span></span> <span data-ttu-id="cd2f7-144">A carga é limitada a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-144">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="cd2f7-145">Criar um externalItem</span><span class="sxs-lookup"><span data-stu-id="cd2f7-145">Creating an externalItem</span></span>

<span data-ttu-id="cd2f7-146">Ao criar um `externalItem` , os campos a seguir são obrigatórios: `@odata.type` , `acl` e `properties` .</span><span class="sxs-lookup"><span data-stu-id="cd2f7-146">When creating an `externalItem`, the following fields are required: `@odata.type`, `acl`, and `properties`.</span></span> <span data-ttu-id="cd2f7-147">O `properties` objeto deve conter pelo menos uma propriedade.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-147">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="cd2f7-148">Todas as `DateTime` Propriedades de tipo devem estar no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-148">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="cd2f7-149">As propriedades em um `externalItem` devem usar especificadores de tipo na carga nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="cd2f7-149">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="cd2f7-150">Para `String` Propriedades de tipo, se o valor contiver caracteres não-ASCII.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-150">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="cd2f7-151">Para todos os tipos de coleção.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-151">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="cd2f7-152">Ao incluir uma propriedade de tipo `Collection(DateTime)` , você deve usar o especificador de tipo `Collection(DateTimeOffset)` .</span><span class="sxs-lookup"><span data-stu-id="cd2f7-152">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

## <a name="response"></a><span data-ttu-id="cd2f7-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd2f7-153">Response</span></span>

<span data-ttu-id="cd2f7-154">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-154">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cd2f7-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cd2f7-155">Examples</span></span>

### <a name="example-create-a-custom-item"></a><span data-ttu-id="cd2f7-156">Exemplo: criar um item personalizado</span><span class="sxs-lookup"><span data-stu-id="cd2f7-156">Example: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="cd2f7-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd2f7-157">Request</span></span>

<span data-ttu-id="cd2f7-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-158">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cd2f7-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd2f7-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cd2f7-160">C#</span><span class="sxs-lookup"><span data-stu-id="cd2f7-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd2f7-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd2f7-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd2f7-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd2f7-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="cd2f7-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd2f7-163">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="cd2f7-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cd2f7-164">The following is an example of the response.</span></span>

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


