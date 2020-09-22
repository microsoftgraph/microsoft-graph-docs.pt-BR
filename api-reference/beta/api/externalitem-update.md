---
title: Atualizar externalitem
description: Atualizar as propriedades de um externalitem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 411d64b5ec6afdd5f994c64faceb4e5fc9a2c637
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192207"
---
# <a name="update-externalitem"></a><span data-ttu-id="454c0-103">Atualizar externalitem</span><span class="sxs-lookup"><span data-stu-id="454c0-103">Update externalitem</span></span>

<span data-ttu-id="454c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="454c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="454c0-105">Atualizar as propriedades de um [externalitem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="454c0-105">Update the properties of an [externalitem](../resources/externalitem.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="454c0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="454c0-106">Permissions</span></span>

<span data-ttu-id="454c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="454c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="454c0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="454c0-109">Permission type</span></span>                        | <span data-ttu-id="454c0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="454c0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="454c0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="454c0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="454c0-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="454c0-112">Not supported.</span></span> |
| <span data-ttu-id="454c0-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="454c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="454c0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="454c0-114">Not supported.</span></span> |
| <span data-ttu-id="454c0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="454c0-115">Application</span></span>                            | <span data-ttu-id="454c0-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="454c0-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="454c0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="454c0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="454c0-118">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="454c0-118">Path parameters</span></span>

| <span data-ttu-id="454c0-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="454c0-119">Parameter</span></span>     | <span data-ttu-id="454c0-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="454c0-120">Type</span></span>   | <span data-ttu-id="454c0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="454c0-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="454c0-122">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="454c0-122">connection-id</span></span> | <span data-ttu-id="454c0-123">string</span><span class="sxs-lookup"><span data-stu-id="454c0-123">string</span></span> | <span data-ttu-id="454c0-124">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="454c0-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="454c0-125">item-id</span><span class="sxs-lookup"><span data-stu-id="454c0-125">item-id</span></span>       | <span data-ttu-id="454c0-126">string</span><span class="sxs-lookup"><span data-stu-id="454c0-126">string</span></span> | <span data-ttu-id="454c0-127">A propriedade fornecida pelo desenvolvedor `id` do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="454c0-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="454c0-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="454c0-128">Request headers</span></span>

| <span data-ttu-id="454c0-129">Nome</span><span class="sxs-lookup"><span data-stu-id="454c0-129">Name</span></span>          | <span data-ttu-id="454c0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="454c0-130">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="454c0-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="454c0-131">Authorization</span></span> | <span data-ttu-id="454c0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="454c0-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="454c0-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="454c0-134">Content-Type</span></span>  | <span data-ttu-id="454c0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="454c0-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="454c0-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="454c0-137">Request body</span></span>

<span data-ttu-id="454c0-138">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="454c0-138">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="454c0-139">Propriedades existentes (exceto propriedades dentro do `properties` objeto) que não estão incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base nas alterações de outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="454c0-139">Existing properties (excluding properties inside the `properties` object) that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="454c0-140">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="454c0-140">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="454c0-141">As propriedades a seguir podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="454c0-141">The following properties can be updated.</span></span>

| <span data-ttu-id="454c0-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="454c0-142">Property</span></span>   | <span data-ttu-id="454c0-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="454c0-143">Type</span></span>                                  | <span data-ttu-id="454c0-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="454c0-144">Description</span></span>               |
|:-----------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="454c0-145">ACL</span><span class="sxs-lookup"><span data-stu-id="454c0-145">acl</span></span>        | <span data-ttu-id="454c0-146">coleção [ACL](../resources/acl.md)</span><span class="sxs-lookup"><span data-stu-id="454c0-146">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="454c0-147">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="454c0-147">An array of access control entries.</span></span> <span data-ttu-id="454c0-148">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="454c0-148">Each entry specifies the access granted to a user or group.</span></span> |
| <span data-ttu-id="454c0-149">conteúdo</span><span class="sxs-lookup"><span data-stu-id="454c0-149">content</span></span>    | [<span data-ttu-id="454c0-150">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="454c0-150">externalItemContent</span></span>](../resources/externalitemcontent.md) | <span data-ttu-id="454c0-151">Uma representação de texto simples do conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="454c0-151">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="454c0-152">O texto nessa propriedade é indexado de texto completo.</span><span class="sxs-lookup"><span data-stu-id="454c0-152">The text in this property is full-text indexed.</span></span> |
| <span data-ttu-id="454c0-153">properties</span><span class="sxs-lookup"><span data-stu-id="454c0-153">properties</span></span> | <span data-ttu-id="454c0-154">Objeto</span><span class="sxs-lookup"><span data-stu-id="454c0-154">Object</span></span>                                | <span data-ttu-id="454c0-155">Um recipiente de propriedades com as propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="454c0-155">A property bag with the properties of the item.</span></span> <span data-ttu-id="454c0-156">As propriedades devem estar em conformidade com o [esquema](../resources/schema.md) definido para o [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="454c0-156">The properties MUST conform to the [schema](../resources/schema.md) defined for the [externalConnection](../resources/externalconnection.md).</span></span> |

### <a name="updating-the-acl-collection"></a><span data-ttu-id="454c0-157">Atualizando a coleção ACL</span><span class="sxs-lookup"><span data-stu-id="454c0-157">Updating the acl collection</span></span>

<span data-ttu-id="454c0-158">Se a `acl` propriedade for incluída em uma solicitação Update, a coleção ACL existente será substituída pela coleção incluída na solicitação.</span><span class="sxs-lookup"><span data-stu-id="454c0-158">If the `acl` property is included in an update request, the existing ACL collection is overwritten with the collection included in the request.</span></span>

### <a name="updating-the-properties-object"></a><span data-ttu-id="454c0-159">Atualizando o objeto Properties</span><span class="sxs-lookup"><span data-stu-id="454c0-159">Updating the properties object</span></span>

<span data-ttu-id="454c0-160">Se a `properties` propriedade for incluída em uma solicitação Update, o conjunto de propriedades existente será substituído pelo valor incluído na solicitação.</span><span class="sxs-lookup"><span data-stu-id="454c0-160">If the `properties` property is included in an update request, the existing property bag is overwritten with the value included in the request.</span></span>

## <a name="response"></a><span data-ttu-id="454c0-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="454c0-161">Response</span></span>

<span data-ttu-id="454c0-162">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [externalItem](../resources/externalitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="454c0-162">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="454c0-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="454c0-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="454c0-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="454c0-164">Request</span></span>

<span data-ttu-id="454c0-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="454c0-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="454c0-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="454c0-166">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="454c0-167">C#</span><span class="sxs-lookup"><span data-stu-id="454c0-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="454c0-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="454c0-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="454c0-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="454c0-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="454c0-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="454c0-170">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="454c0-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="454c0-171">The following is an example of the response.</span></span>

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


