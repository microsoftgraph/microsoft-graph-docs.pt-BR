---
title: Criar externalItem
description: Crie um novo externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7939689cf113e709853e5da666d1479e600fe4cd
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467551"
---
# <a name="create-externalitem"></a><span data-ttu-id="a1d54-103">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="a1d54-103">Create externalItem</span></span>

<span data-ttu-id="a1d54-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="a1d54-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1d54-105">Crie um novo [externalItem](../resources/externalconnectors-externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="a1d54-105">Create a new [externalItem](../resources/externalconnectors-externalitem.md).</span></span>

<span data-ttu-id="a1d54-106">Essa API pode ser usada para criar um item personalizado.</span><span class="sxs-lookup"><span data-stu-id="a1d54-106">This API can be used to create a custom item.</span></span> <span data-ttu-id="a1d54-107">O [externalConnection que contém](../resources/externalconnectors-externalconnection.md) deve ter um [esquema](../resources/externalconnectors-schema.md) registrado do tipo correspondente.</span><span class="sxs-lookup"><span data-stu-id="a1d54-107">The containing [externalConnection](../resources/externalconnectors-externalconnection.md) must have a [schema](../resources/externalconnectors-schema.md) registered of the corresponding type.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1d54-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1d54-108">Permissions</span></span>

<span data-ttu-id="a1d54-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1d54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1d54-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1d54-111">Permission type</span></span>                        | <span data-ttu-id="a1d54-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1d54-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a1d54-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1d54-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1d54-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1d54-114">Not supported.</span></span> |
| <span data-ttu-id="a1d54-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1d54-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1d54-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1d54-116">Not supported.</span></span> |
| <span data-ttu-id="a1d54-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1d54-117">Application</span></span>                            | <span data-ttu-id="a1d54-118">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1d54-118">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1d54-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1d54-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="a1d54-120">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="a1d54-120">Path parameters</span></span>

| <span data-ttu-id="a1d54-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a1d54-121">Parameter</span></span>     | <span data-ttu-id="a1d54-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1d54-122">Type</span></span>   | <span data-ttu-id="a1d54-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1d54-123">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="a1d54-124">connection-id</span><span class="sxs-lookup"><span data-stu-id="a1d54-124">connection-id</span></span> | <span data-ttu-id="a1d54-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1d54-125">string</span></span> | <span data-ttu-id="a1d54-126">A `id` propriedade do [externalConnection que](../resources/externalconnectors-externalconnection.md) contém</span><span class="sxs-lookup"><span data-stu-id="a1d54-126">The `id` property of the containing [externalConnection](../resources/externalconnectors-externalconnection.md)</span></span> |
| <span data-ttu-id="a1d54-127">item-id</span><span class="sxs-lookup"><span data-stu-id="a1d54-127">item-id</span></span>       | <span data-ttu-id="a1d54-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1d54-128">string</span></span> | <span data-ttu-id="a1d54-129">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalconnectors-externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="a1d54-129">The developer-provided `id` property of the [externalItem](../resources/externalconnectors-externalitem.md).</span></span> <span data-ttu-id="a1d54-130">Se nenhum item já existir com `id` isso, um novo item será criado.</span><span class="sxs-lookup"><span data-stu-id="a1d54-130">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="a1d54-131">Se um item já existir com isso `id` , ele será substituído pelo objeto enviado no corpo.</span><span class="sxs-lookup"><span data-stu-id="a1d54-131">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a1d54-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d54-132">Request headers</span></span>

| <span data-ttu-id="a1d54-133">Nome</span><span class="sxs-lookup"><span data-stu-id="a1d54-133">Name</span></span>          | <span data-ttu-id="a1d54-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1d54-134">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="a1d54-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1d54-135">Authorization</span></span> | <span data-ttu-id="a1d54-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1d54-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="a1d54-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a1d54-138">Content-Type</span></span>  | <span data-ttu-id="a1d54-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1d54-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1d54-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d54-141">Request body</span></span>

<span data-ttu-id="a1d54-142">No corpo da solicitação, fornece uma representação JSON de um [objeto externalItem.](../resources/externalconnectors-externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="a1d54-142">In the request body, supply a JSON representation of an [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span> <span data-ttu-id="a1d54-143">A carga é limitada a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="a1d54-143">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="a1d54-144">Criando um externalItem</span><span class="sxs-lookup"><span data-stu-id="a1d54-144">Creating an externalItem</span></span>

<span data-ttu-id="a1d54-145">Ao criar `externalItem` um , os campos a seguir são necessários: e `acl` `properties` .</span><span class="sxs-lookup"><span data-stu-id="a1d54-145">When creating an `externalItem`, the following fields are required: `acl`, and `properties`.</span></span> <span data-ttu-id="a1d54-146">O `properties` objeto deve conter pelo menos uma propriedade.</span><span class="sxs-lookup"><span data-stu-id="a1d54-146">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="a1d54-147">Todas `DateTime` as propriedades de tipo devem estar no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="a1d54-147">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="a1d54-148">As propriedades em um `externalItem` devem usar especificadores de tipo na carga nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="a1d54-148">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="a1d54-149">Para `String` propriedades de tipo, se o valor contiver caracteres não ASCII.</span><span class="sxs-lookup"><span data-stu-id="a1d54-149">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="a1d54-150">Para todos os tipos de coleção.</span><span class="sxs-lookup"><span data-stu-id="a1d54-150">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="a1d54-151">Ao incluir uma propriedade do tipo `Collection(DateTime)` , você deve usar o especificador de tipo `Collection(DateTimeOffset)` .</span><span class="sxs-lookup"><span data-stu-id="a1d54-151">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

## <a name="response"></a><span data-ttu-id="a1d54-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1d54-152">Response</span></span>

<span data-ttu-id="a1d54-153">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="a1d54-153">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a1d54-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a1d54-154">Examples</span></span>

### <a name="example-create-a-custom-item"></a><span data-ttu-id="a1d54-155">Exemplo: Criar um item personalizado</span><span class="sxs-lookup"><span data-stu-id="a1d54-155">Example: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="a1d54-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d54-156">Request</span></span>

<span data-ttu-id="a1d54-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1d54-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1d54-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1d54-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections",
  "@odata.type": "microsoft.graph.externalConnectors.externalItem"
}-->

```http
PUT https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
Content-type: application/json

{
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
# <a name="c"></a>[<span data-ttu-id="a1d54-159">C#</span><span class="sxs-lookup"><span data-stu-id="a1d54-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1d54-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1d54-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1d54-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1d54-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="a1d54-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1d54-162">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="a1d54-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1d54-163">The following is an example of the response.</span></span>

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
