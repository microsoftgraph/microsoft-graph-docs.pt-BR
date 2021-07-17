---
title: Atualizar externalItem
description: Atualize as propriedades de um externalitem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 985580042972b5ab649592467ff18b3e574df6e5
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466971"
---
# <a name="update-externalitem"></a><span data-ttu-id="b79f2-103">Atualizar externalItem</span><span class="sxs-lookup"><span data-stu-id="b79f2-103">Update externalItem</span></span>

<span data-ttu-id="b79f2-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="b79f2-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b79f2-105">Atualize as propriedades de [um externalitem](../resources/externalconnectors-externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="b79f2-105">Update the properties of an [externalitem](../resources/externalconnectors-externalitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b79f2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b79f2-106">Permissions</span></span>

<span data-ttu-id="b79f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b79f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b79f2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b79f2-109">Permission type</span></span>                        | <span data-ttu-id="b79f2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b79f2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b79f2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b79f2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b79f2-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b79f2-112">Not supported.</span></span> |
| <span data-ttu-id="b79f2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b79f2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b79f2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b79f2-114">Not supported.</span></span> |
| <span data-ttu-id="b79f2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b79f2-115">Application</span></span>                            | <span data-ttu-id="b79f2-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b79f2-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b79f2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b79f2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="b79f2-118">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="b79f2-118">Path parameters</span></span>

| <span data-ttu-id="b79f2-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b79f2-119">Parameter</span></span>     | <span data-ttu-id="b79f2-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b79f2-120">Type</span></span>   | <span data-ttu-id="b79f2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b79f2-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="b79f2-122">connection-id</span><span class="sxs-lookup"><span data-stu-id="b79f2-122">connection-id</span></span> | <span data-ttu-id="b79f2-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b79f2-123">string</span></span> | <span data-ttu-id="b79f2-124">A `id` propriedade do [externalConnection que](../resources/externalconnectors-externalconnection.md) contém</span><span class="sxs-lookup"><span data-stu-id="b79f2-124">The `id` property of the containing [externalConnection](../resources/externalconnectors-externalconnection.md)</span></span> |
| <span data-ttu-id="b79f2-125">item-id</span><span class="sxs-lookup"><span data-stu-id="b79f2-125">item-id</span></span>       | <span data-ttu-id="b79f2-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b79f2-126">string</span></span> | <span data-ttu-id="b79f2-127">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalconnectors-externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="b79f2-127">The developer-provided `id` property of the [externalItem](../resources/externalconnectors-externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b79f2-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b79f2-128">Request headers</span></span>

| <span data-ttu-id="b79f2-129">Nome</span><span class="sxs-lookup"><span data-stu-id="b79f2-129">Name</span></span>          | <span data-ttu-id="b79f2-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b79f2-130">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="b79f2-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="b79f2-131">Authorization</span></span> | <span data-ttu-id="b79f2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b79f2-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b79f2-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b79f2-134">Content-Type</span></span>  | <span data-ttu-id="b79f2-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b79f2-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b79f2-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b79f2-137">Request body</span></span>

<span data-ttu-id="b79f2-138">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b79f2-138">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b79f2-139">As propriedades existentes (excluindo propriedades dentro do objeto) que não estão incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base em alterações em outros valores `properties` de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b79f2-139">Existing properties (excluding properties inside the `properties` object) that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b79f2-140">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b79f2-140">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="b79f2-141">As propriedades a seguir podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="b79f2-141">The following properties can be updated.</span></span>

| <span data-ttu-id="b79f2-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b79f2-142">Property</span></span>   | <span data-ttu-id="b79f2-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="b79f2-143">Type</span></span>                                  | <span data-ttu-id="b79f2-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="b79f2-144">Description</span></span>               |
|:-----------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="b79f2-145">acl</span><span class="sxs-lookup"><span data-stu-id="b79f2-145">acl</span></span>        | <span data-ttu-id="b79f2-146">[Coleção microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md)</span><span class="sxs-lookup"><span data-stu-id="b79f2-146">[microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md) collection</span></span> | <span data-ttu-id="b79f2-147">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="b79f2-147">An array of access control entries.</span></span> <span data-ttu-id="b79f2-148">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="b79f2-148">Each entry specifies the access granted to a user or group.</span></span> |
| <span data-ttu-id="b79f2-149">conteúdo</span><span class="sxs-lookup"><span data-stu-id="b79f2-149">content</span></span>    | [<span data-ttu-id="b79f2-150">microsoft.graph.externalConnectors.externalItemContent</span><span class="sxs-lookup"><span data-stu-id="b79f2-150">microsoft.graph.externalConnectors.externalItemContent</span></span>](../resources/externalconnectors-externalitemcontent.md) | <span data-ttu-id="b79f2-151">Uma representação em texto sem texto do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="b79f2-151">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="b79f2-152">O texto nesta propriedade é indexado em texto completo.</span><span class="sxs-lookup"><span data-stu-id="b79f2-152">The text in this property is full-text indexed.</span></span> |
| <span data-ttu-id="b79f2-153">properties</span><span class="sxs-lookup"><span data-stu-id="b79f2-153">properties</span></span> | <span data-ttu-id="b79f2-154">Objeto</span><span class="sxs-lookup"><span data-stu-id="b79f2-154">Object</span></span>                                | <span data-ttu-id="b79f2-155">Um pacote de propriedades com as propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="b79f2-155">A property bag with the properties of the item.</span></span> <span data-ttu-id="b79f2-156">As propriedades DEVEM estar em conformidade [com o esquema](../resources/externalconnectors-schema.md) definido para [externalConnection](../resources/externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="b79f2-156">The properties MUST conform to the [schema](../resources/externalconnectors-schema.md) defined for the [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span> |

### <a name="updating-the-acl-collection"></a><span data-ttu-id="b79f2-157">Atualizando a coleção acl</span><span class="sxs-lookup"><span data-stu-id="b79f2-157">Updating the acl collection</span></span>

<span data-ttu-id="b79f2-158">Se a propriedade for incluída em uma solicitação de atualização, a coleção ACL existente será substituída com a `acl` coleção incluída na solicitação.</span><span class="sxs-lookup"><span data-stu-id="b79f2-158">If the `acl` property is included in an update request, the existing ACL collection is overwritten with the collection included in the request.</span></span>

### <a name="updating-the-properties-object"></a><span data-ttu-id="b79f2-159">Atualizando o objeto properties</span><span class="sxs-lookup"><span data-stu-id="b79f2-159">Updating the properties object</span></span>

<span data-ttu-id="b79f2-160">Se a propriedade for incluída em uma solicitação de atualização, o pacote de propriedades existente será substituído com o `properties` valor incluído na solicitação.</span><span class="sxs-lookup"><span data-stu-id="b79f2-160">If the `properties` property is included in an update request, the existing property bag is overwritten with the value included in the request.</span></span>

## <a name="response"></a><span data-ttu-id="b79f2-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="b79f2-161">Response</span></span>

<span data-ttu-id="b79f2-162">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto externalItem](../resources/externalconnectors-externalitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b79f2-162">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalconnectors-externalitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b79f2-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b79f2-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b79f2-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b79f2-164">Request</span></span>

<span data-ttu-id="b79f2-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b79f2-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b79f2-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="b79f2-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_externalitem",
  "@odata.type": "microsoft.graph.externalConnectors.acl"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="b79f2-167">C#</span><span class="sxs-lookup"><span data-stu-id="b79f2-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b79f2-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b79f2-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b79f2-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b79f2-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b79f2-170">Java</span><span class="sxs-lookup"><span data-stu-id="b79f2-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-externalitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="b79f2-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="b79f2-171">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="b79f2-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b79f2-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "TSP228082938",
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "@odata.type": "microsoft.graph.externalConnectors.externalItemContent",
    "value": "<h1>Error in payment gateway</h1><p>Error details...</p>",
    "type": "html"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update externalitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: update_externalitem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->


