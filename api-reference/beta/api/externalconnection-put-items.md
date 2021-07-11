---
title: Criar externalItem
description: Crie um novo externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 170c3fb87903e6f2f66fe910d80ca8f4a6e87b50
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366789"
---
# <a name="create-externalitem"></a><span data-ttu-id="7e008-103">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="7e008-103">Create externalItem</span></span>

<span data-ttu-id="7e008-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e008-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e008-105">Crie um novo [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="7e008-105">Create a new [externalItem](../resources/externalitem.md).</span></span>

<span data-ttu-id="7e008-106">Essa API pode ser usada para criar um item personalizado.</span><span class="sxs-lookup"><span data-stu-id="7e008-106">This API can be used to create a custom item.</span></span> <span data-ttu-id="7e008-107">Especifique o tipo que você está criando incluindo `@odata.type` a propriedade no corpo JSON.</span><span class="sxs-lookup"><span data-stu-id="7e008-107">Specify the type you are creating by including the `@odata.type` property in the JSON body.</span></span> <span data-ttu-id="7e008-108">O [externalConnection que contém](../resources/externalconnection.md) deve ter um [esquema](../resources/schema.md) registrado do tipo correspondente.</span><span class="sxs-lookup"><span data-stu-id="7e008-108">The containing [externalConnection](../resources/externalconnection.md) must have a [schema](../resources/schema.md) registered of the corresponding type.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e008-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e008-109">Permissions</span></span>

<span data-ttu-id="7e008-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e008-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e008-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e008-112">Permission type</span></span>                        | <span data-ttu-id="7e008-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e008-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7e008-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e008-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e008-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e008-115">Not supported.</span></span> |
| <span data-ttu-id="7e008-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e008-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e008-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e008-117">Not supported.</span></span> |
| <span data-ttu-id="7e008-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e008-118">Application</span></span>                            | <span data-ttu-id="7e008-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e008-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e008-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e008-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="7e008-121">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="7e008-121">Path parameters</span></span>

| <span data-ttu-id="7e008-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7e008-122">Parameter</span></span>     | <span data-ttu-id="7e008-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e008-123">Type</span></span>   | <span data-ttu-id="7e008-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e008-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="7e008-125">connection-id</span><span class="sxs-lookup"><span data-stu-id="7e008-125">connection-id</span></span> | <span data-ttu-id="7e008-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e008-126">string</span></span> | <span data-ttu-id="7e008-127">A `id` propriedade do [externalConnection que](../resources/externalconnection.md) contém</span><span class="sxs-lookup"><span data-stu-id="7e008-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="7e008-128">item-id</span><span class="sxs-lookup"><span data-stu-id="7e008-128">item-id</span></span>       | <span data-ttu-id="7e008-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e008-129">string</span></span> | <span data-ttu-id="7e008-130">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="7e008-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> <span data-ttu-id="7e008-131">Se nenhum item já existir com `id` isso, um novo item será criado.</span><span class="sxs-lookup"><span data-stu-id="7e008-131">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="7e008-132">Se um item já existir com isso `id` , ele será substituído pelo objeto enviado no corpo.</span><span class="sxs-lookup"><span data-stu-id="7e008-132">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7e008-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e008-133">Request headers</span></span>

| <span data-ttu-id="7e008-134">Nome</span><span class="sxs-lookup"><span data-stu-id="7e008-134">Name</span></span>          | <span data-ttu-id="7e008-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e008-135">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="7e008-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e008-136">Authorization</span></span> | <span data-ttu-id="7e008-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e008-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="7e008-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e008-139">Content-Type</span></span>  | <span data-ttu-id="7e008-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e008-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e008-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e008-142">Request body</span></span>

<span data-ttu-id="7e008-143">No corpo da solicitação, fornece uma representação JSON de um [objeto externalItem.](../resources/externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="7e008-143">In the request body, supply a JSON representation of an [externalItem](../resources/externalitem.md) object.</span></span> <span data-ttu-id="7e008-144">A carga é limitada a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="7e008-144">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="7e008-145">Criando um externalItem</span><span class="sxs-lookup"><span data-stu-id="7e008-145">Creating an externalItem</span></span>

<span data-ttu-id="7e008-146">Ao criar `externalItem` um , os campos a seguir são necessários: , e `@odata.type` `acl` `properties` .</span><span class="sxs-lookup"><span data-stu-id="7e008-146">When creating an `externalItem`, the following fields are required: `@odata.type`, `acl`, and `properties`.</span></span> <span data-ttu-id="7e008-147">O `properties` objeto deve conter pelo menos uma propriedade.</span><span class="sxs-lookup"><span data-stu-id="7e008-147">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="7e008-148">Todas `DateTime` as propriedades de tipo devem estar no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="7e008-148">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="7e008-149">As propriedades em um `externalItem` devem usar especificadores de tipo na carga nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="7e008-149">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="7e008-150">Para `String` propriedades de tipo, se o valor contiver caracteres não ASCII.</span><span class="sxs-lookup"><span data-stu-id="7e008-150">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="7e008-151">Para todos os tipos de coleção.</span><span class="sxs-lookup"><span data-stu-id="7e008-151">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="7e008-152">Ao incluir uma propriedade do tipo `Collection(DateTime)` , você deve usar o especificador de tipo `Collection(DateTimeOffset)` .</span><span class="sxs-lookup"><span data-stu-id="7e008-152">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

## <a name="response"></a><span data-ttu-id="7e008-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e008-153">Response</span></span>

<span data-ttu-id="7e008-154">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="7e008-154">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7e008-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7e008-155">Examples</span></span>

### <a name="example-create-a-custom-item"></a><span data-ttu-id="7e008-156">Exemplo: Criar um item personalizado</span><span class="sxs-lookup"><span data-stu-id="7e008-156">Example: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="7e008-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e008-157">Request</span></span>

<span data-ttu-id="7e008-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e008-158">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e008-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e008-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
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
# <a name="c"></a>[<span data-ttu-id="7e008-160">C#</span><span class="sxs-lookup"><span data-stu-id="7e008-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e008-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e008-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e008-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e008-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="7e008-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e008-163">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="7e008-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7e008-164">The following is an example of the response.</span></span>

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
