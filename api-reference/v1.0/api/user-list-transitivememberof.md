---
title: Listar usuário transitivo memberOf
description: Obtenha grupos e funções de diretório dos quais o usuário é membro. Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o usuário é um membro aninhado.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 4ddc73c3cbe702759d12e3875b91e743decdbe8c
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904285"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="14045-104">Listar usuário transitivo memberOf</span><span class="sxs-lookup"><span data-stu-id="14045-104">List user transitive memberOf</span></span>

<span data-ttu-id="14045-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14045-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14045-106">Obtenha grupos e funções de diretório dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="14045-106">Get groups, directory roles that the user is a member of.</span></span> <span data-ttu-id="14045-107">Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o usuário é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="14045-107">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="14045-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="14045-108">Permissions</span></span>

<span data-ttu-id="14045-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14045-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14045-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14045-111">Permission type</span></span>      | <span data-ttu-id="14045-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14045-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14045-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14045-113">Delegated (work or school account)</span></span> | <span data-ttu-id="14045-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="14045-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="14045-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14045-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14045-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14045-116">Not supported.</span></span>    |
|<span data-ttu-id="14045-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14045-117">Application</span></span> | <span data-ttu-id="14045-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14045-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="14045-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14045-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14045-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="14045-120">Optional query parameters</span></span>

<span data-ttu-id="14045-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="14045-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="14045-122">O elenco do OData também é habilitado, por exemplo, você pode transmitir para obter apenas a associação transitiva em grupos.</span><span class="sxs-lookup"><span data-stu-id="14045-122">OData cast is also enabled, for example, you can cast to get just the transitive membership in groups.</span></span> <span data-ttu-id="14045-123">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="14045-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="14045-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="14045-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="14045-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="14045-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14045-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14045-126">Request headers</span></span>

| <span data-ttu-id="14045-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14045-127">Header</span></span>       | <span data-ttu-id="14045-128">Valor</span><span class="sxs-lookup"><span data-stu-id="14045-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="14045-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="14045-129">Authorization</span></span>  | <span data-ttu-id="14045-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14045-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="14045-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="14045-132">ConsistencyLevel</span></span> | <span data-ttu-id="14045-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="14045-133">eventual.</span></span> <span data-ttu-id="14045-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="14045-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="14045-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="14045-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14045-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14045-136">Request body</span></span>

<span data-ttu-id="14045-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14045-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14045-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="14045-138">Response</span></span>

<span data-ttu-id="14045-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14045-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14045-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="14045-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-member-of"></a><span data-ttu-id="14045-141">Exemplo 1: obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro</span><span class="sxs-lookup"><span data-stu-id="14045-141">Example 1: Get groups, directory roles, and administrative units that the user is a member of</span></span>

#### <a name="request"></a><span data-ttu-id="14045-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14045-142">Request</span></span>

<span data-ttu-id="14045-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14045-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="14045-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="14045-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="14045-145">C#</span><span class="sxs-lookup"><span data-stu-id="14045-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14045-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14045-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14045-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14045-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14045-148">Java</span><span class="sxs-lookup"><span data-stu-id="14045-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="14045-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="14045-149">Response</span></span>

<span data-ttu-id="14045-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14045-150">The following is an example of the response.</span></span>

><span data-ttu-id="14045-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14045-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
  "value":[
    {
      "@odata.type":"#microsoft.graph.group",
      "displayName":"All_Contoso_Licensing",
      "mailEnabled":true,
      "mailNickname":"ContosoMailNickName",
      "securityEnabled":true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership-in-groups-directory-roles-and-administrative-units"></a><span data-ttu-id="14045-153">Exemplo 2: obter apenas uma contagem de associação transitiva em grupos, funções de diretório e unidades administrativas</span><span class="sxs-lookup"><span data-stu-id="14045-153">Example 2: Get only a count of transitive membership in groups, directory roles, and administrative units</span></span>

#### <a name="request"></a><span data-ttu-id="14045-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14045-154">Request</span></span>

<span data-ttu-id="14045-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14045-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="14045-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="14045-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="14045-157">C#</span><span class="sxs-lookup"><span data-stu-id="14045-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14045-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14045-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14045-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14045-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14045-160">Java</span><span class="sxs-lookup"><span data-stu-id="14045-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="14045-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="14045-161">Response</span></span>

<span data-ttu-id="14045-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14045-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="14045-163">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação transitiva em grupos</span><span class="sxs-lookup"><span data-stu-id="14045-163">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="14045-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14045-164">Request</span></span>

<span data-ttu-id="14045-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14045-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="14045-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="14045-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="14045-167">C#</span><span class="sxs-lookup"><span data-stu-id="14045-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14045-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14045-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14045-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14045-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14045-170">Java</span><span class="sxs-lookup"><span data-stu-id="14045-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="14045-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="14045-171">Response</span></span>

<span data-ttu-id="14045-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14045-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
  } -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`588`

### <a name="example-4-use-search-and-odata-cast-to-get-transitive-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="14045-173">Exemplo 4: Use $search e a conversão OData para obter uma associação transitiva em grupos com nomes de exibição que contenham as letras "Tier", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="14045-173">Example 4: Use $search and OData cast to get transitive membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="14045-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14045-174">Request</span></span>

<span data-ttu-id="14045-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14045-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="14045-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="14045-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="14045-177">C#</span><span class="sxs-lookup"><span data-stu-id="14045-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14045-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14045-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14045-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14045-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14045-180">Java</span><span class="sxs-lookup"><span data-stu-id="14045-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="14045-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="14045-181">Response</span></span>

<span data-ttu-id="14045-182">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14045-182">The following is an example of the response.</span></span>

><span data-ttu-id="14045-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14045-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-transitive-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="14045-185">Exemplo 5: use $filter e o elenco OData para obter uma associação transitiva em grupos com um nome de exibição que começa com ' a ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="14045-185">Example 5: Use $filter and OData cast to get transitive membership in groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="14045-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14045-186">Request</span></span>

<span data-ttu-id="14045-187">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14045-187">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="14045-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="14045-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="14045-189">C#</span><span class="sxs-lookup"><span data-stu-id="14045-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14045-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14045-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14045-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14045-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14045-192">Java</span><span class="sxs-lookup"><span data-stu-id="14045-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="14045-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="14045-193">Response</span></span>

<span data-ttu-id="14045-194">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14045-194">The following is an example of the response.</span></span>

><span data-ttu-id="14045-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14045-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com",
      "mailEnabled":true,
      "mailNickname":"AADContoso_Users",
      "securityEnabled":true
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
