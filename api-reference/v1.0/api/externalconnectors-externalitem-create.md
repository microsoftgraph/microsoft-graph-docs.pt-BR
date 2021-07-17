---
title: Criar externalItem
description: Crie um novo externalItem.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: eba04bf339eeed41f9fe59831773d413bbed3111
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467182"
---
# <a name="create-externalitem"></a><span data-ttu-id="79b2a-103">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="79b2a-103">Create externalItem</span></span>

<span data-ttu-id="79b2a-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="79b2a-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="79b2a-105">Crie um novo [objeto externalItem.](../resources/externalconnectors-externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="79b2a-105">Create a new [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="79b2a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="79b2a-106">Permissions</span></span>
<span data-ttu-id="79b2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79b2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79b2a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79b2a-109">Permission type</span></span>|<span data-ttu-id="79b2a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79b2a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79b2a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79b2a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="79b2a-112">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="79b2a-112">Not applicable</span></span>|
|<span data-ttu-id="79b2a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79b2a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79b2a-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="79b2a-114">Not applicable</span></span>|
|<span data-ttu-id="79b2a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79b2a-115">Application</span></span>| <span data-ttu-id="79b2a-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79b2a-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79b2a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79b2a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /connections/{connectionsId}/items
```

## <a name="request-headers"></a><span data-ttu-id="79b2a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79b2a-118">Request headers</span></span>
|<span data-ttu-id="79b2a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="79b2a-119">Name</span></span>|<span data-ttu-id="79b2a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="79b2a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="79b2a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="79b2a-121">Authorization</span></span>|<span data-ttu-id="79b2a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79b2a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="79b2a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79b2a-124">Content-Type</span></span>|<span data-ttu-id="79b2a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79b2a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79b2a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79b2a-127">Request body</span></span>
<span data-ttu-id="79b2a-128">No corpo da solicitação, fornece uma representação JSON do [objeto externalItem.](../resources/externalconnectors-externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="79b2a-128">In the request body, supply a JSON representation of the [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span>

<span data-ttu-id="79b2a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [externalItem](../resources/externalconnectors-externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="79b2a-129">The following table shows the properties that are required when you create the [externalItem](../resources/externalconnectors-externalitem.md).</span></span>

|<span data-ttu-id="79b2a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79b2a-130">Property</span></span>|<span data-ttu-id="79b2a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="79b2a-131">Type</span></span>| <span data-ttu-id="79b2a-132">Obrigatório (Y/N)</span><span class="sxs-lookup"><span data-stu-id="79b2a-132">Required (Y/N)</span></span> | <span data-ttu-id="79b2a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="79b2a-133">Description</span></span>|
|:---|:---|:---|:---|
|<span data-ttu-id="79b2a-134">id</span><span class="sxs-lookup"><span data-stu-id="79b2a-134">id</span></span>|<span data-ttu-id="79b2a-135">String</span><span class="sxs-lookup"><span data-stu-id="79b2a-135">String</span></span>|<span data-ttu-id="79b2a-136">Y</span><span class="sxs-lookup"><span data-stu-id="79b2a-136">Y</span></span>|<span data-ttu-id="79b2a-137">A ID do item</span><span class="sxs-lookup"><span data-stu-id="79b2a-137">The item ID</span></span>|
|<span data-ttu-id="79b2a-138">properties</span><span class="sxs-lookup"><span data-stu-id="79b2a-138">properties</span></span>|[<span data-ttu-id="79b2a-139">microsoft.graph.externalConnectors.properties</span><span class="sxs-lookup"><span data-stu-id="79b2a-139">microsoft.graph.externalConnectors.properties</span></span>](../resources/externalconnectors-properties.md)|<span data-ttu-id="79b2a-140">Y</span><span class="sxs-lookup"><span data-stu-id="79b2a-140">Y</span></span>|<span data-ttu-id="79b2a-141">As propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="79b2a-141">The item properties.</span></span> <span data-ttu-id="79b2a-142">O `properties` objeto deve conter pelo menos uma propriedade.</span><span class="sxs-lookup"><span data-stu-id="79b2a-142">The `properties` object must contain at least one property.</span></span> <span data-ttu-id="79b2a-143">Todas `DateTime` as propriedades de tipo devem estar no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="79b2a-143">All `DateTime` type properties must be in ISO 8601 format.</span></span>|
|<span data-ttu-id="79b2a-144">conteúdo</span><span class="sxs-lookup"><span data-stu-id="79b2a-144">content</span></span>|[<span data-ttu-id="79b2a-145">microsoft.graph.externalConnectors.externalItemContent</span><span class="sxs-lookup"><span data-stu-id="79b2a-145">microsoft.graph.externalConnectors.externalItemContent</span></span>](../resources/externalconnectors-externalitemcontent.md)|<span data-ttu-id="79b2a-146">N</span><span class="sxs-lookup"><span data-stu-id="79b2a-146">N</span></span>|<span data-ttu-id="79b2a-147">O conteúdo do item externo</span><span class="sxs-lookup"><span data-stu-id="79b2a-147">The external item content</span></span>|
|<span data-ttu-id="79b2a-148">acl</span><span class="sxs-lookup"><span data-stu-id="79b2a-148">acl</span></span>|<span data-ttu-id="79b2a-149">[Coleção microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md)</span><span class="sxs-lookup"><span data-stu-id="79b2a-149">[microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md) collection</span></span>|<span data-ttu-id="79b2a-150">Y</span><span class="sxs-lookup"><span data-stu-id="79b2a-150">Y</span></span>|<span data-ttu-id="79b2a-151">A lista de controles de acesso</span><span class="sxs-lookup"><span data-stu-id="79b2a-151">The access control list</span></span>|

<span data-ttu-id="79b2a-152">As propriedades em um `externalItem` devem usar especificadores de tipo na carga nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="79b2a-152">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="79b2a-153">Para `String` propriedades de tipo, se o valor contiver caracteres não ASCII.</span><span class="sxs-lookup"><span data-stu-id="79b2a-153">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="79b2a-154">Para todos os tipos de coleção.</span><span class="sxs-lookup"><span data-stu-id="79b2a-154">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="79b2a-155">Ao incluir uma propriedade do tipo `Collection(DateTime)` , você deve usar o especificador de tipo `Collection(DateTimeOffset)` .</span><span class="sxs-lookup"><span data-stu-id="79b2a-155">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

## <a name="response"></a><span data-ttu-id="79b2a-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="79b2a-156">Response</span></span> 

<span data-ttu-id="79b2a-157">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="79b2a-157">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="79b2a-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="79b2a-158">Examples</span></span>

### <a name="example-create-a-custom-item"></a><span data-ttu-id="79b2a-159">Exemplo: Criar um item personalizado</span><span class="sxs-lookup"><span data-stu-id="79b2a-159">Example: Create a custom item</span></span>

### <a name="request"></a><span data-ttu-id="79b2a-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79b2a-160">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_externalConnections"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant"
    },
    {
      "type": "externalGroup",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny"
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


### <a name="response"></a><span data-ttu-id="79b2a-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="79b2a-161">Response</span></span>

<span data-ttu-id="79b2a-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79b2a-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

