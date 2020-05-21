---
title: Listar usuário membro
description: Obter grupos, funções de diretório e unidades administrativas dos quais o usuário é membro direto. Essa operação não é transitiva.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ccb9c085cd9481514d2227c8eb133027cc4f463b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336471"
---
# <a name="list-user-memberof"></a><span data-ttu-id="db9dd-104">Listar usuário membro</span><span class="sxs-lookup"><span data-stu-id="db9dd-104">List user memberOf</span></span>

<span data-ttu-id="db9dd-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db9dd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db9dd-106">Obter grupos, funções de diretório e unidades administrativas dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="db9dd-106">Get groups, directory roles and administrative units that the user is a direct member of.</span></span> <span data-ttu-id="db9dd-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="db9dd-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="db9dd-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="db9dd-108">Permissions</span></span>

<span data-ttu-id="db9dd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db9dd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db9dd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db9dd-111">Permission type</span></span> | <span data-ttu-id="db9dd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db9dd-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="db9dd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db9dd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="db9dd-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="db9dd-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="db9dd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db9dd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db9dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db9dd-116">Not supported.</span></span> |
| <span data-ttu-id="db9dd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db9dd-117">Application</span></span> | <span data-ttu-id="db9dd-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db9dd-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db9dd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db9dd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db9dd-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="db9dd-120">Optional query parameters</span></span>

<span data-ttu-id="db9dd-121">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search` , `$count` e `$filter` .</span><span class="sxs-lookup"><span data-stu-id="db9dd-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="db9dd-122">A conversão OData também é habilitada, por exemplo, você pode transmitir para obter apenas o directoryRoles do usuário é um membro.</span><span class="sxs-lookup"><span data-stu-id="db9dd-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="db9dd-123">Você pode usar `$search` na propriedade **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="db9dd-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="db9dd-124">Quando os itens são adicionados ou atualizados para esse recurso, eles são especialmente indexados para uso com os `$count` `$search` parâmetros de consulta e.</span><span class="sxs-lookup"><span data-stu-id="db9dd-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="db9dd-125">Pode haver um ligeiro atraso entre a adição ou atualização de um item e quando ele está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="db9dd-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db9dd-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db9dd-126">Request headers</span></span>

| <span data-ttu-id="db9dd-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db9dd-127">Header</span></span> | <span data-ttu-id="db9dd-128">Valor</span><span class="sxs-lookup"><span data-stu-id="db9dd-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="db9dd-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="db9dd-129">Authorization</span></span>  | <span data-ttu-id="db9dd-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db9dd-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db9dd-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="db9dd-132">ConsistencyLevel</span></span> | <span data-ttu-id="db9dd-133">ocorra.</span><span class="sxs-lookup"><span data-stu-id="db9dd-133">eventual.</span></span> <span data-ttu-id="db9dd-134">Esse cabeçalho e `$count` são necessários ao usar os `$search` parâmetros de consulta de conversão de,, `$filter` `$orderby` ou OData.</span><span class="sxs-lookup"><span data-stu-id="db9dd-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="db9dd-135">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="db9dd-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db9dd-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db9dd-136">Request body</span></span>

<span data-ttu-id="db9dd-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db9dd-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db9dd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="db9dd-138">Response</span></span>

<span data-ttu-id="db9dd-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db9dd-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db9dd-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="db9dd-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="db9dd-141">Exemplo 1: obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro direto</span><span class="sxs-lookup"><span data-stu-id="db9dd-141">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="db9dd-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db9dd-142">Request</span></span>

<span data-ttu-id="db9dd-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db9dd-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="db9dd-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="db9dd-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="db9dd-145">C#</span><span class="sxs-lookup"><span data-stu-id="db9dd-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db9dd-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db9dd-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db9dd-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db9dd-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="db9dd-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="db9dd-148">Response</span></span>

<span data-ttu-id="db9dd-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db9dd-149">The following is an example of the response.</span></span>
><span data-ttu-id="db9dd-150">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="db9dd-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="db9dd-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db9dd-151">All the properties will be returned from an actual call.</span></span>

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
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "displayName": "All Users",
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="db9dd-152">Exemplo 2: obter apenas uma contagem de todos os grupos, funções de diretório e unidades administrativas das quais o usuário é membro direto</span><span class="sxs-lookup"><span data-stu-id="db9dd-152">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="db9dd-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db9dd-153">Request</span></span>

<span data-ttu-id="db9dd-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db9dd-154">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="db9dd-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="db9dd-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="db9dd-156">C#</span><span class="sxs-lookup"><span data-stu-id="db9dd-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db9dd-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db9dd-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db9dd-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db9dd-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="db9dd-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="db9dd-159">Response</span></span>

<span data-ttu-id="db9dd-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db9dd-160">The following is an example of the response.</span></span>
><span data-ttu-id="db9dd-161">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="db9dd-161">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="db9dd-162">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db9dd-162">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="db9dd-163">893</span><span class="sxs-lookup"><span data-stu-id="db9dd-163">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="db9dd-164">Exemplo 3: usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="db9dd-164">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="db9dd-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db9dd-165">Request</span></span>

<span data-ttu-id="db9dd-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db9dd-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="db9dd-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="db9dd-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="db9dd-168">C#</span><span class="sxs-lookup"><span data-stu-id="db9dd-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db9dd-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db9dd-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db9dd-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db9dd-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="db9dd-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="db9dd-171">Response</span></span>

<span data-ttu-id="db9dd-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db9dd-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="db9dd-173">294</span><span class="sxs-lookup"><span data-stu-id="db9dd-173">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="db9dd-174">Exemplo 4: Use $search e a conversão OData para obter associação em grupos com nomes de exibição que contenham as letras "Tier", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="db9dd-174">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="db9dd-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db9dd-175">Request</span></span>

<span data-ttu-id="db9dd-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db9dd-176">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="db9dd-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="db9dd-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="db9dd-178">C#</span><span class="sxs-lookup"><span data-stu-id="db9dd-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db9dd-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db9dd-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db9dd-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db9dd-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="db9dd-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="db9dd-181">Response</span></span>

<span data-ttu-id="db9dd-182">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db9dd-182">The following is an example of the response.</span></span>
><span data-ttu-id="db9dd-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db9dd-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="db9dd-185">Exemplo 5: use $filter e a conversão OData para obter grupos com um nome de exibição que comece com ' a ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="db9dd-185">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="db9dd-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db9dd-186">Request</span></span>

<span data-ttu-id="db9dd-187">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db9dd-187">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="db9dd-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="db9dd-188">Response</span></span>

<span data-ttu-id="db9dd-189">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db9dd-189">The following is an example of the response.</span></span>
><span data-ttu-id="db9dd-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db9dd-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
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
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
