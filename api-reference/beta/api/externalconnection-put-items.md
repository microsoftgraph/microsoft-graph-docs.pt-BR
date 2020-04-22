---
title: Criar externalItem
description: Criar um novo externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7d6b7f1abf94aacd7732c7fb767a0220d6892abf
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43718602"
---
# <a name="create-externalitem"></a><span data-ttu-id="0d619-103">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="0d619-103">Create externalItem</span></span>

<span data-ttu-id="0d619-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d619-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d619-105">Criar um novo [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="0d619-105">Create a new [externalItem](../resources/externalitem.md).</span></span>

<span data-ttu-id="0d619-106">Essa API pode ser usada para criar um item personalizado.</span><span class="sxs-lookup"><span data-stu-id="0d619-106">This API can be used to create a custom item.</span></span> <span data-ttu-id="0d619-107">Especifique o tipo que você está criando incluindo a `@odata.type` Propriedade no corpo JSON.</span><span class="sxs-lookup"><span data-stu-id="0d619-107">Specify the type you are creating by including the `@odata.type` property in the JSON body.</span></span> <span data-ttu-id="0d619-108">O [externalConnection](../resources/externalconnection.md) recipiente deve ter um [esquema](../resources/schema.md) registrado do tipo correspondente.</span><span class="sxs-lookup"><span data-stu-id="0d619-108">The containing [externalConnection](../resources/externalconnection.md) must have a [schema](../resources/schema.md) registered of the corresponding type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="0d619-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d619-109">Permissions</span></span>

<span data-ttu-id="0d619-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d619-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d619-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d619-112">Permission type</span></span>                        | <span data-ttu-id="0d619-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d619-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0d619-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d619-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d619-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d619-115">Not supported.</span></span> |
| <span data-ttu-id="0d619-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d619-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d619-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d619-117">Not supported.</span></span> |
| <span data-ttu-id="0d619-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d619-118">Application</span></span>                            | <span data-ttu-id="0d619-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d619-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d619-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d619-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="0d619-121">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="0d619-121">Path parameters</span></span>

| <span data-ttu-id="0d619-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0d619-122">Parameter</span></span>     | <span data-ttu-id="0d619-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d619-123">Type</span></span>   | <span data-ttu-id="0d619-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d619-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="0d619-125">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="0d619-125">connection-id</span></span> | <span data-ttu-id="0d619-126">string</span><span class="sxs-lookup"><span data-stu-id="0d619-126">string</span></span> | <span data-ttu-id="0d619-127">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="0d619-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="0d619-128">item-id</span><span class="sxs-lookup"><span data-stu-id="0d619-128">item-id</span></span>       | <span data-ttu-id="0d619-129">string</span><span class="sxs-lookup"><span data-stu-id="0d619-129">string</span></span> | <span data-ttu-id="0d619-130">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="0d619-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> <span data-ttu-id="0d619-131">Se nenhum item já existir com isso `id`, um novo item é criado.</span><span class="sxs-lookup"><span data-stu-id="0d619-131">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="0d619-132">Se já existir um item com isso `id`, ele será substituído pelo objeto enviado no corpo.</span><span class="sxs-lookup"><span data-stu-id="0d619-132">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0d619-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d619-133">Request headers</span></span>

| <span data-ttu-id="0d619-134">Nome</span><span class="sxs-lookup"><span data-stu-id="0d619-134">Name</span></span>          | <span data-ttu-id="0d619-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d619-135">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="0d619-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d619-136">Authorization</span></span> | <span data-ttu-id="0d619-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d619-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0d619-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d619-139">Content-Type</span></span>  | <span data-ttu-id="0d619-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d619-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d619-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d619-142">Request body</span></span>

<span data-ttu-id="0d619-143">No corpo da solicitação, forneça uma representação JSON de um objeto [externalItem](../resources/externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="0d619-143">In the request body, supply a JSON representation of an [externalItem](../resources/externalitem.md) object.</span></span> <span data-ttu-id="0d619-144">A carga é limitada a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="0d619-144">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="0d619-145">Criar um externalItem</span><span class="sxs-lookup"><span data-stu-id="0d619-145">Creating an externalItem</span></span>

<span data-ttu-id="0d619-146">Ao criar um `externalItem`, os campos a seguir são `@odata.type`obrigatórios `acl`:, `properties`e.</span><span class="sxs-lookup"><span data-stu-id="0d619-146">When creating an `externalItem`, the following fields are required: `@odata.type`, `acl`, and `properties`.</span></span> <span data-ttu-id="0d619-147">O `properties` objeto deve conter pelo menos uma propriedade.</span><span class="sxs-lookup"><span data-stu-id="0d619-147">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="0d619-148">Todas `DateTime` as propriedades de tipo devem estar no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="0d619-148">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="0d619-149">As propriedades em `externalItem` um devem usar especificadores de tipo na carga nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="0d619-149">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="0d619-150">Para `String` Propriedades de tipo, se o valor contiver caracteres não-ASCII.</span><span class="sxs-lookup"><span data-stu-id="0d619-150">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="0d619-151">Para todos os tipos de coleção.</span><span class="sxs-lookup"><span data-stu-id="0d619-151">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="0d619-152">Ao incluir uma propriedade de tipo `Collection(DateTime)`, você deve usar o especificador `Collection(DateTimeOffset)`de tipo.</span><span class="sxs-lookup"><span data-stu-id="0d619-152">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

## <a name="response"></a><span data-ttu-id="0d619-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d619-153">Response</span></span>

<span data-ttu-id="0d619-154">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="0d619-154">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0d619-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0d619-155">Examples</span></span>

### <a name="example-create-a-custom-item"></a><span data-ttu-id="0d619-156">Exemplo: criar um item personalizado</span><span class="sxs-lookup"><span data-stu-id="0d619-156">Example: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="0d619-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d619-157">Request</span></span>

<span data-ttu-id="0d619-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d619-158">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d619-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d619-159">HTTP</span></span>](#tab/http)
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
  "content": {
    "value": "<h1>Error in payment gateway</h1><p>Error details...</p>",
    "type": "html"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="0d619-160">C#</span><span class="sxs-lookup"><span data-stu-id="0d619-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d619-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d619-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d619-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d619-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="0d619-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d619-163">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="0d619-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d619-164">The following is an example of the response.</span></span>

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
