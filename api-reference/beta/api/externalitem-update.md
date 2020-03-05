---
title: Atualizar externalitem
description: Atualizar as propriedades de um externalitem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: ff3237204310365eb8945a739bd423668494f786
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421995"
---
# <a name="update-externalitem"></a><span data-ttu-id="9fef2-103">Atualizar externalitem</span><span class="sxs-lookup"><span data-stu-id="9fef2-103">Update externalitem</span></span>

<span data-ttu-id="9fef2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9fef2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fef2-105">Atualizar as propriedades de um [externalitem](../resources/externalitem.md) ou [externalfile](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="9fef2-105">Update the properties of an [externalitem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="9fef2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9fef2-106">Permissions</span></span>

<span data-ttu-id="9fef2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fef2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9fef2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fef2-109">Permission type</span></span>                        | <span data-ttu-id="9fef2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9fef2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9fef2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fef2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9fef2-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fef2-112">Not supported.</span></span> |
| <span data-ttu-id="9fef2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fef2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fef2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fef2-114">Not supported.</span></span> |
| <span data-ttu-id="9fef2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fef2-115">Application</span></span>                            | <span data-ttu-id="9fef2-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fef2-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fef2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fef2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="9fef2-118">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="9fef2-118">Path parameters</span></span>

| <span data-ttu-id="9fef2-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9fef2-119">Parameter</span></span>     | <span data-ttu-id="9fef2-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fef2-120">Type</span></span>   | <span data-ttu-id="9fef2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fef2-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="9fef2-122">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="9fef2-122">connection-id</span></span> | <span data-ttu-id="9fef2-123">string</span><span class="sxs-lookup"><span data-stu-id="9fef2-123">string</span></span> | <span data-ttu-id="9fef2-124">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="9fef2-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="9fef2-125">item-id</span><span class="sxs-lookup"><span data-stu-id="9fef2-125">item-id</span></span>       | <span data-ttu-id="9fef2-126">string</span><span class="sxs-lookup"><span data-stu-id="9fef2-126">string</span></span> | <span data-ttu-id="9fef2-127">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalitem.md) ou do [externalfile](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="9fef2-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9fef2-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fef2-128">Request headers</span></span>

| <span data-ttu-id="9fef2-129">Nome</span><span class="sxs-lookup"><span data-stu-id="9fef2-129">Name</span></span>          | <span data-ttu-id="9fef2-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fef2-130">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="9fef2-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fef2-131">Authorization</span></span> | <span data-ttu-id="9fef2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fef2-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="9fef2-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9fef2-134">Content-Type</span></span>  | <span data-ttu-id="9fef2-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fef2-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fef2-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fef2-137">Request body</span></span>

<span data-ttu-id="9fef2-138">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="9fef2-138">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9fef2-139">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="9fef2-139">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9fef2-140">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9fef2-140">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="9fef2-141">As propriedades a seguir podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="9fef2-141">The following properties can be updated.</span></span>

> [!NOTE]
> <span data-ttu-id="9fef2-142">Durante a visualização apenas, `acl` a propriedade pode ser atualizada via patch.</span><span class="sxs-lookup"><span data-stu-id="9fef2-142">During the preview only the `acl` property can be updated via PATCH.</span></span> <span data-ttu-id="9fef2-143">Para atualizar outras propriedades, use um [Put para substituir o item existente por um novo item](externalconnection-put-items.md).</span><span class="sxs-lookup"><span data-stu-id="9fef2-143">In order to update other properties, use a [PUT to overwrite the existing item with a new item](externalconnection-put-items.md).</span></span>

### <a name="externalitem-properties"></a><span data-ttu-id="9fef2-144">Propriedades externalItem</span><span class="sxs-lookup"><span data-stu-id="9fef2-144">externalItem properties</span></span>

| <span data-ttu-id="9fef2-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fef2-145">Property</span></span> | <span data-ttu-id="9fef2-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fef2-146">Type</span></span>                                  | <span data-ttu-id="9fef2-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fef2-147">Description</span></span>               |
|:---------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="9fef2-148">ACL</span><span class="sxs-lookup"><span data-stu-id="9fef2-148">acl</span></span>      | <span data-ttu-id="9fef2-149">coleção [ACL](../resources/acl.md)</span><span class="sxs-lookup"><span data-stu-id="9fef2-149">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="9fef2-150">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="9fef2-150">An array of access control entries.</span></span> <span data-ttu-id="9fef2-151">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="9fef2-151">Each entry specifies the access granted to a user or group.</span></span> |

### <a name="externalfile-properties"></a><span data-ttu-id="9fef2-152">Propriedades de externalfile</span><span class="sxs-lookup"><span data-stu-id="9fef2-152">externalFile properties</span></span>

| <span data-ttu-id="9fef2-153">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fef2-153">Property</span></span> | <span data-ttu-id="9fef2-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fef2-154">Type</span></span>                                  | <span data-ttu-id="9fef2-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fef2-155">Description</span></span>               |
|:---------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="9fef2-156">ACL</span><span class="sxs-lookup"><span data-stu-id="9fef2-156">acl</span></span>      | <span data-ttu-id="9fef2-157">coleção [ACL](../resources/acl.md)</span><span class="sxs-lookup"><span data-stu-id="9fef2-157">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="9fef2-158">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="9fef2-158">An array of access control entries.</span></span> <span data-ttu-id="9fef2-159">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="9fef2-159">Each entry specifies the access granted to a user or group.</span></span> |

## <a name="response"></a><span data-ttu-id="9fef2-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fef2-160">Response</span></span>

<span data-ttu-id="9fef2-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [externalItem](../resources/externalitem.md) ou [externalfile](../resources/externalfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fef2-161">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9fef2-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9fef2-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9fef2-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fef2-163">Request</span></span>

<span data-ttu-id="9fef2-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fef2-164">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9fef2-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fef2-165">HTTP</span></span>](#tab/http)
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
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "grant",
      "identitySource": "Azure Active Directory"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="9fef2-166">C#</span><span class="sxs-lookup"><span data-stu-id="9fef2-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9fef2-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fef2-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9fef2-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fef2-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="9fef2-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fef2-169">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="9fef2-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9fef2-170">The following is an example of the response.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update externalitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
