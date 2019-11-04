---
title: Atualizar externalitem
description: Atualizar as propriedades de um externalitem.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 1135d889142b66e4ce980244a7f3e6020246228c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938636"
---
# <a name="update-externalitem"></a><span data-ttu-id="7a9b6-103">Atualizar externalitem</span><span class="sxs-lookup"><span data-stu-id="7a9b6-103">Update externalitem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a9b6-104">Atualizar as propriedades de um [externalitem](../resources/externalitem.md) ou [externalfile](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="7a9b6-104">Update the properties of an [externalitem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7a9b6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a9b6-105">Permissions</span></span>

<span data-ttu-id="7a9b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a9b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7a9b6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a9b6-108">Permission type</span></span>                        | <span data-ttu-id="7a9b6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a9b6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7a9b6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a9b6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a9b6-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-111">Not supported.</span></span> |
| <span data-ttu-id="7a9b6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a9b6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a9b6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-113">Not supported.</span></span> |
| <span data-ttu-id="7a9b6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a9b6-114">Application</span></span>                            | <span data-ttu-id="7a9b6-115">ExternalItem. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7a9b6-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a9b6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a9b6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="7a9b6-117">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="7a9b6-117">Path parameters</span></span>

| <span data-ttu-id="7a9b6-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7a9b6-118">Parameter</span></span>     | <span data-ttu-id="7a9b6-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a9b6-119">Type</span></span>   | <span data-ttu-id="7a9b6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a9b6-120">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="7a9b6-121">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="7a9b6-121">connection-id</span></span> | <span data-ttu-id="7a9b6-122">string</span><span class="sxs-lookup"><span data-stu-id="7a9b6-122">string</span></span> | <span data-ttu-id="7a9b6-123">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="7a9b6-123">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="7a9b6-124">item-id</span><span class="sxs-lookup"><span data-stu-id="7a9b6-124">item-id</span></span>       | <span data-ttu-id="7a9b6-125">string</span><span class="sxs-lookup"><span data-stu-id="7a9b6-125">string</span></span> | <span data-ttu-id="7a9b6-126">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalitem.md) ou do [externalfile](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="7a9b6-126">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7a9b6-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a9b6-127">Request headers</span></span>

| <span data-ttu-id="7a9b6-128">Nome</span><span class="sxs-lookup"><span data-stu-id="7a9b6-128">Name</span></span>          | <span data-ttu-id="7a9b6-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a9b6-129">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="7a9b6-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a9b6-130">Authorization</span></span> | <span data-ttu-id="7a9b6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="7a9b6-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a9b6-133">Content-Type</span></span>  | <span data-ttu-id="7a9b6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a9b6-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a9b6-136">Request body</span></span>

<span data-ttu-id="7a9b6-137">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-137">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7a9b6-138">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-138">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7a9b6-139">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-139">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="7a9b6-140">As propriedades a seguir podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-140">The following properties can be updated.</span></span>

> [!NOTE]
> <span data-ttu-id="7a9b6-141">Durante a visualização apenas, `acl` a propriedade pode ser atualizada via patch.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-141">During the preview only the `acl` property can be updated via PATCH.</span></span> <span data-ttu-id="7a9b6-142">Para atualizar outras propriedades, use um [Put para substituir o item existente por um novo item](externalconnection-put-items.md).</span><span class="sxs-lookup"><span data-stu-id="7a9b6-142">In order to update other properties, use a [PUT to overwrite the existing item with a new item](externalconnection-put-items.md).</span></span>

### <a name="externalitem-properties"></a><span data-ttu-id="7a9b6-143">Propriedades externalItem</span><span class="sxs-lookup"><span data-stu-id="7a9b6-143">externalItem properties</span></span>

| <span data-ttu-id="7a9b6-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a9b6-144">Property</span></span> | <span data-ttu-id="7a9b6-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a9b6-145">Type</span></span>                                  | <span data-ttu-id="7a9b6-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a9b6-146">Description</span></span>               |
|:---------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="7a9b6-147">ACL</span><span class="sxs-lookup"><span data-stu-id="7a9b6-147">acl</span></span>      | <span data-ttu-id="7a9b6-148">coleção [ACL](../resources/acl.md)</span><span class="sxs-lookup"><span data-stu-id="7a9b6-148">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="7a9b6-149">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-149">An array of access control entries.</span></span> <span data-ttu-id="7a9b6-150">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-150">Each entry specifies the access granted to a user or group.</span></span> |

### <a name="externalfile-properties"></a><span data-ttu-id="7a9b6-151">Propriedades de externalfile</span><span class="sxs-lookup"><span data-stu-id="7a9b6-151">externalFile properties</span></span>

| <span data-ttu-id="7a9b6-152">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a9b6-152">Property</span></span> | <span data-ttu-id="7a9b6-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a9b6-153">Type</span></span>                                  | <span data-ttu-id="7a9b6-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a9b6-154">Description</span></span>               |
|:---------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="7a9b6-155">ACL</span><span class="sxs-lookup"><span data-stu-id="7a9b6-155">acl</span></span>      | <span data-ttu-id="7a9b6-156">coleção [ACL](../resources/acl.md)</span><span class="sxs-lookup"><span data-stu-id="7a9b6-156">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="7a9b6-157">Uma matriz de entradas de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-157">An array of access control entries.</span></span> <span data-ttu-id="7a9b6-158">Cada entrada especifica o acesso concedido a um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-158">Each entry specifies the access granted to a user or group.</span></span> |

## <a name="response"></a><span data-ttu-id="7a9b6-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a9b6-159">Response</span></span>

<span data-ttu-id="7a9b6-160">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [externalItem](../resources/externalitem.md) ou [externalfile](../resources/externalfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-160">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a9b6-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7a9b6-161">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a9b6-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a9b6-162">Request</span></span>

<span data-ttu-id="7a9b6-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-163">The following is an example of the request.</span></span>
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

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="7a9b6-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a9b6-164">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="7a9b6-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7a9b6-165">The following is an example of the response.</span></span>

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
