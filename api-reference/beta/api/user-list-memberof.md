---
title: Listar usuário memberOf
description: Obter grupos, funções de diretório e unidades administrativas dos quais o usuário é membro direto. Essa operação não é transitiva.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 0c5b1e89bcc234894c83abee9ac52ab2ff0fa0b3
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873290"
---
# <a name="list-user-memberof"></a><span data-ttu-id="ccab0-104">Listar usuário memberOf</span><span class="sxs-lookup"><span data-stu-id="ccab0-104">List user memberOf</span></span>

<span data-ttu-id="ccab0-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccab0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccab0-106">Obter grupos, funções de diretório e unidades administrativas dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="ccab0-106">Get groups, directory roles and administrative units that the user is a direct member of.</span></span> <span data-ttu-id="ccab0-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="ccab0-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccab0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ccab0-108">Permissions</span></span>

<span data-ttu-id="ccab0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccab0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ccab0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccab0-111">Permission type</span></span> | <span data-ttu-id="ccab0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ccab0-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="ccab0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccab0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ccab0-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ccab0-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="ccab0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccab0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccab0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccab0-116">Not supported.</span></span> |
| <span data-ttu-id="ccab0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccab0-117">Application</span></span> | <span data-ttu-id="ccab0-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccab0-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccab0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccab0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ccab0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ccab0-120">Optional query parameters</span></span>

<span data-ttu-id="ccab0-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ccab0-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="ccab0-122">A conversão OData também é habilitada, por exemplo, você pode transmitir para obter apenas o directoryRoles do usuário é um membro.</span><span class="sxs-lookup"><span data-stu-id="ccab0-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="ccab0-123">Você pode usar `$search`na propriedade**displayName**.</span><span class="sxs-lookup"><span data-stu-id="ccab0-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="ccab0-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="ccab0-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="ccab0-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="ccab0-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccab0-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccab0-126">Request headers</span></span>

| <span data-ttu-id="ccab0-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ccab0-127">Header</span></span> | <span data-ttu-id="ccab0-128">Valor</span><span class="sxs-lookup"><span data-stu-id="ccab0-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="ccab0-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccab0-129">Authorization</span></span>  | <span data-ttu-id="ccab0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccab0-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ccab0-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="ccab0-132">ConsistencyLevel</span></span> | <span data-ttu-id="ccab0-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="ccab0-133">eventual.</span></span> <span data-ttu-id="ccab0-134">Esse cabeçalho e `$count` são necessários ao usar os `$search` parâmetros de consulta de conversão de,, `$filter` `$orderby` ou OData.</span><span class="sxs-lookup"><span data-stu-id="ccab0-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="ccab0-135">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="ccab0-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccab0-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccab0-136">Request body</span></span>

<span data-ttu-id="ccab0-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ccab0-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccab0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccab0-138">Response</span></span>

<span data-ttu-id="ccab0-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccab0-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ccab0-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ccab0-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="ccab0-141">Exemplo 1: obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro direto</span><span class="sxs-lookup"><span data-stu-id="ccab0-141">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="ccab0-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccab0-142">Request</span></span>

<span data-ttu-id="ccab0-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccab0-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ccab0-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccab0-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="ccab0-145">C#</span><span class="sxs-lookup"><span data-stu-id="ccab0-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccab0-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccab0-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccab0-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccab0-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ccab0-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccab0-148">Response</span></span>

<span data-ttu-id="ccab0-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ccab0-149">The following is an example of the response.</span></span>
><span data-ttu-id="ccab0-150">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ccab0-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ccab0-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ccab0-151">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="ccab0-152">Exemplo 2: obter apenas uma contagem de todos os grupos, funções de diretório e unidades administrativas das quais o usuário é membro direto</span><span class="sxs-lookup"><span data-stu-id="ccab0-152">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="ccab0-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccab0-153">Request</span></span>

<span data-ttu-id="ccab0-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccab0-154">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ccab0-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccab0-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ccab0-156">C#</span><span class="sxs-lookup"><span data-stu-id="ccab0-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccab0-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccab0-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccab0-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccab0-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ccab0-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccab0-159">Response</span></span>

<span data-ttu-id="ccab0-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ccab0-160">The following is an example of the response.</span></span>
><span data-ttu-id="ccab0-161">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ccab0-161">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ccab0-162">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ccab0-162">All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="ccab0-163">893</span><span class="sxs-lookup"><span data-stu-id="ccab0-163">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="ccab0-164">Exemplo 3: usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="ccab0-164">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="ccab0-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccab0-165">Request</span></span>

<span data-ttu-id="ccab0-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccab0-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ccab0-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccab0-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ccab0-168">C#</span><span class="sxs-lookup"><span data-stu-id="ccab0-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccab0-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccab0-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccab0-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccab0-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ccab0-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccab0-171">Response</span></span>

<span data-ttu-id="ccab0-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ccab0-172">The following is an example of the response.</span></span>

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

<span data-ttu-id="ccab0-173">294</span><span class="sxs-lookup"><span data-stu-id="ccab0-173">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="ccab0-174">Exemplo 4: Use $search e a conversão OData para obter associação em grupos com nomes de exibição que contenham as letras "Tier", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="ccab0-174">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ccab0-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccab0-175">Request</span></span>

<span data-ttu-id="ccab0-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccab0-176">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ccab0-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccab0-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ccab0-178">C#</span><span class="sxs-lookup"><span data-stu-id="ccab0-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccab0-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccab0-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccab0-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccab0-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ccab0-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccab0-181">Response</span></span>

<span data-ttu-id="ccab0-182">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ccab0-182">The following is an example of the response.</span></span>
><span data-ttu-id="ccab0-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ccab0-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="ccab0-185">Exemplo 5: use $filter e a conversão OData para obter grupos com um nome de exibição que comece com ' a ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="ccab0-185">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ccab0-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccab0-186">Request</span></span>

<span data-ttu-id="ccab0-187">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccab0-187">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ccab0-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccab0-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ccab0-189">C#</span><span class="sxs-lookup"><span data-stu-id="ccab0-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccab0-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccab0-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccab0-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccab0-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ccab0-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccab0-192">Response</span></span>

<span data-ttu-id="ccab0-193">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ccab0-193">The following is an example of the response.</span></span>
><span data-ttu-id="ccab0-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ccab0-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
