---
title: Atualizar externalitem
description: Atualize as propriedades de um externalitem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c862a6139f4f24a9207e7387913ec0fc5b04e8e6
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366784"
---
# <a name="update-externalitem"></a><span data-ttu-id="df1ed-103">Atualizar externalitem</span><span class="sxs-lookup"><span data-stu-id="df1ed-103">Update externalitem</span></span>

<span data-ttu-id="df1ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df1ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df1ed-105">Atualize as propriedades de [um externalitem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="df1ed-105">Update the properties of an [externalitem](../resources/externalitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df1ed-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df1ed-106">Permissions</span></span>

<span data-ttu-id="df1ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df1ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df1ed-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df1ed-109">Permission type</span></span>                        | <span data-ttu-id="df1ed-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df1ed-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="df1ed-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df1ed-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="df1ed-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df1ed-112">Not supported.</span></span> |
| <span data-ttu-id="df1ed-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df1ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df1ed-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df1ed-114">Not supported.</span></span> |
| <span data-ttu-id="df1ed-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df1ed-115">Application</span></span>                            | <span data-ttu-id="df1ed-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df1ed-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df1ed-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df1ed-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="df1ed-118">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="df1ed-118">Path parameters</span></span>

| <span data-ttu-id="df1ed-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="df1ed-119">Parameter</span></span>     | <span data-ttu-id="df1ed-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="df1ed-120">Type</span></span>   | <span data-ttu-id="df1ed-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="df1ed-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="df1ed-122">connection-id</span><span class="sxs-lookup"><span data-stu-id="df1ed-122">connection-id</span></span> | <span data-ttu-id="df1ed-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df1ed-123">string</span></span> | <span data-ttu-id="df1ed-124">A `id` propriedade do [externalConnection que](../resources/externalconnection.md) contém</span><span class="sxs-lookup"><span data-stu-id="df1ed-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="df1ed-125">item-id</span><span class="sxs-lookup"><span data-stu-id="df1ed-125">item-id</span></span>       | <span data-ttu-id="df1ed-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df1ed-126">string</span></span> | <span data-ttu-id="df1ed-127">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="df1ed-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="df1ed-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df1ed-128">Request headers</span></span>

| <span data-ttu-id="df1ed-129">Nome</span><span class="sxs-lookup"><span data-stu-id="df1ed-129">Name</span></span>          | <span data-ttu-id="df1ed-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="df1ed-130">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="df1ed-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="df1ed-131">Authorization</span></span> | <span data-ttu-id="df1ed-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df1ed-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="df1ed-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df1ed-134">Content-Type</span></span>  | <span data-ttu-id="df1ed-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df1ed-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df1ed-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df1ed-137">Request body</span></span>

<span data-ttu-id="df1ed-138">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="df1ed-138">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="df1ed-139">As propriedades existentes (excluindo propriedades dentro do objeto) que não estão incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base em alterações em outros valores `properties` de propriedade.</span><span class="sxs-lookup"><span data-stu-id="df1ed-139">Existing properties (excluding properties inside the `properties` object) that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="df1ed-140">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="df1ed-140">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="df1ed-141">As propriedades a seguir podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="df1ed-141">The following properties can be updated.</span></span>

| <span data-ttu-id="df1ed-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df1ed-142">Property</span></span>   | <span data-ttu-id="df1ed-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="df1ed-143">Type</span></span>                                  | <span data-ttu-id="df1ed-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="df1ed-144">Description</span></span>               |
|:-----------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="df1ed-145">acl</span><span class="sxs-lookup"><span data-stu-id="df1ed-145">acl</span></span>        | <span data-ttu-id="df1ed-146">[Coleção acl](../resources/acl.md)</span><span class="sxs-lookup"><span data-stu-id="df1ed-146">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="df1ed-147">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="df1ed-147">An array of access control entries.</span></span> <span data-ttu-id="df1ed-148">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="df1ed-148">Each entry specifies the access granted to a user or group.</span></span> |
| <span data-ttu-id="df1ed-149">conteúdo</span><span class="sxs-lookup"><span data-stu-id="df1ed-149">content</span></span>    | [<span data-ttu-id="df1ed-150">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="df1ed-150">externalItemContent</span></span>](../resources/externalitemcontent.md) | <span data-ttu-id="df1ed-151">Uma representação em texto sem texto do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="df1ed-151">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="df1ed-152">O texto nesta propriedade é indexado em texto completo.</span><span class="sxs-lookup"><span data-stu-id="df1ed-152">The text in this property is full-text indexed.</span></span> |
| <span data-ttu-id="df1ed-153">properties</span><span class="sxs-lookup"><span data-stu-id="df1ed-153">properties</span></span> | <span data-ttu-id="df1ed-154">Objeto</span><span class="sxs-lookup"><span data-stu-id="df1ed-154">Object</span></span>                                | <span data-ttu-id="df1ed-155">Um pacote de propriedades com as propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="df1ed-155">A property bag with the properties of the item.</span></span> <span data-ttu-id="df1ed-156">As propriedades DEVEM estar em conformidade [com o esquema](../resources/schema.md) definido para [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="df1ed-156">The properties MUST conform to the [schema](../resources/schema.md) defined for the [externalConnection](../resources/externalconnection.md).</span></span> |

### <a name="updating-the-acl-collection"></a><span data-ttu-id="df1ed-157">Atualizando a coleção acl</span><span class="sxs-lookup"><span data-stu-id="df1ed-157">Updating the acl collection</span></span>

<span data-ttu-id="df1ed-158">Se a propriedade for incluída em uma solicitação de atualização, a coleção ACL existente será substituída com a `acl` coleção incluída na solicitação.</span><span class="sxs-lookup"><span data-stu-id="df1ed-158">If the `acl` property is included in an update request, the existing ACL collection is overwritten with the collection included in the request.</span></span>

### <a name="updating-the-properties-object"></a><span data-ttu-id="df1ed-159">Atualizando o objeto properties</span><span class="sxs-lookup"><span data-stu-id="df1ed-159">Updating the properties object</span></span>

<span data-ttu-id="df1ed-160">Se a propriedade for incluída em uma solicitação de atualização, o pacote de propriedades existente será substituído com o `properties` valor incluído na solicitação.</span><span class="sxs-lookup"><span data-stu-id="df1ed-160">If the `properties` property is included in an update request, the existing property bag is overwritten with the value included in the request.</span></span>

## <a name="response"></a><span data-ttu-id="df1ed-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="df1ed-161">Response</span></span>

<span data-ttu-id="df1ed-162">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto externalItem](../resources/externalitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df1ed-162">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df1ed-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="df1ed-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df1ed-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df1ed-164">Request</span></span>

<span data-ttu-id="df1ed-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df1ed-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="df1ed-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="df1ed-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_externalitem"
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
# <a name="c"></a>[<span data-ttu-id="df1ed-167">C#</span><span class="sxs-lookup"><span data-stu-id="df1ed-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df1ed-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df1ed-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df1ed-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df1ed-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df1ed-170">Java</span><span class="sxs-lookup"><span data-stu-id="df1ed-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-externalitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="df1ed-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="df1ed-171">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="df1ed-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df1ed-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "TSP228082938",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
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


