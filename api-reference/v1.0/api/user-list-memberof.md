---
title: Listar memberOf
description: 'Obtenha todos os grupos e funções de diretório dos quais o usuário é um membro direto. '
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: f0d4c3f45cc45700b64b54a87e5043c1356ea660
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905839"
---
# <a name="list-memberof"></a><span data-ttu-id="2df8d-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="2df8d-103">List memberOf</span></span>

<span data-ttu-id="2df8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2df8d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2df8d-105">Obtenha [grupos](../resources/group.md) e [funções de diretório](../resources/directoryrole.md) dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="2df8d-105">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2df8d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2df8d-106">Permissions</span></span>
<span data-ttu-id="2df8d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2df8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df8d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2df8d-109">Permission type</span></span>      | <span data-ttu-id="2df8d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2df8d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2df8d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2df8d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2df8d-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2df8d-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2df8d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2df8d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2df8d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2df8d-114">Not supported.</span></span>    |
|<span data-ttu-id="2df8d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2df8d-115">Application</span></span> | <span data-ttu-id="2df8d-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2df8d-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="2df8d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2df8d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2df8d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2df8d-118">Optional query parameters</span></span>

<span data-ttu-id="2df8d-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="2df8d-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="2df8d-120">A conversão OData também está habilitado, por exemplo, você pode convertê-la para obter apenas o directoryRoles do qual o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="2df8d-120">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="2df8d-121">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="2df8d-121">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="2df8d-122">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="2df8d-122">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="2df8d-123">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="2df8d-123">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="2df8d-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2df8d-124">Request headers</span></span>
| <span data-ttu-id="2df8d-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2df8d-125">Header</span></span>       | <span data-ttu-id="2df8d-126">Valor</span><span class="sxs-lookup"><span data-stu-id="2df8d-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2df8d-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="2df8d-127">Authorization</span></span>  | <span data-ttu-id="2df8d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2df8d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2df8d-130">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="2df8d-130">ConsistencyLevel</span></span> | <span data-ttu-id="2df8d-131">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="2df8d-131">eventual.</span></span> <span data-ttu-id="2df8d-132">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="2df8d-132">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="2df8d-133">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="2df8d-133">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2df8d-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2df8d-134">Request body</span></span>
<span data-ttu-id="2df8d-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2df8d-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2df8d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df8d-136">Response</span></span>

<span data-ttu-id="2df8d-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2df8d-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2df8d-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2df8d-138">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="2df8d-139">Exemplo 1: Obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro direto</span><span class="sxs-lookup"><span data-stu-id="2df8d-139">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="2df8d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2df8d-140">Request</span></span>

<span data-ttu-id="2df8d-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2df8d-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2df8d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="2df8d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="2df8d-143">C#</span><span class="sxs-lookup"><span data-stu-id="2df8d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2df8d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2df8d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2df8d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2df8d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2df8d-146">Java</span><span class="sxs-lookup"><span data-stu-id="2df8d-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2df8d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df8d-147">Response</span></span>

<span data-ttu-id="2df8d-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2df8d-148">The following is an example of the response.</span></span>

><span data-ttu-id="2df8d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2df8d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="2df8d-151">Exemplo 2: Obtenha apenas uma contagem de todos os grupos, funções de diretório e unidades administrativas dos quais o usuário é membro direto</span><span class="sxs-lookup"><span data-stu-id="2df8d-151">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="2df8d-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2df8d-152">Request</span></span>

<span data-ttu-id="2df8d-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2df8d-153">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2df8d-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="2df8d-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="2df8d-155">C#</span><span class="sxs-lookup"><span data-stu-id="2df8d-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2df8d-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2df8d-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2df8d-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2df8d-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2df8d-158">Java</span><span class="sxs-lookup"><span data-stu-id="2df8d-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-memberof-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2df8d-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df8d-159">Response</span></span>

<span data-ttu-id="2df8d-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2df8d-160">The following is an example of the response.</span></span>

><span data-ttu-id="2df8d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2df8d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="2df8d-163">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="2df8d-163">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="2df8d-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2df8d-164">Request</span></span>

<span data-ttu-id="2df8d-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2df8d-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2df8d-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="2df8d-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="2df8d-167">C#</span><span class="sxs-lookup"><span data-stu-id="2df8d-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2df8d-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2df8d-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2df8d-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2df8d-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2df8d-170">Java</span><span class="sxs-lookup"><span data-stu-id="2df8d-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2df8d-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df8d-171">Response</span></span>

<span data-ttu-id="2df8d-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2df8d-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="2df8d-173">Exemplo 4: Utilize $search e conversão OData para obter associação em grupos com nomes de exibição que contenham as letras 'camada', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="2df8d-173">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="2df8d-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2df8d-174">Request</span></span>

<span data-ttu-id="2df8d-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2df8d-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2df8d-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="2df8d-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="2df8d-177">C#</span><span class="sxs-lookup"><span data-stu-id="2df8d-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2df8d-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2df8d-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2df8d-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2df8d-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2df8d-180">Java</span><span class="sxs-lookup"><span data-stu-id="2df8d-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2df8d-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df8d-181">Response</span></span>

<span data-ttu-id="2df8d-182">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2df8d-182">The following is an example of the response.</span></span>

><span data-ttu-id="2df8d-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2df8d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="2df8d-185">Exemplo 5: Utilize $filter e a conversão OData para obter grupos com um nome de exibição que começa com 'a' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="2df8d-185">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="2df8d-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2df8d-186">Request</span></span>

<span data-ttu-id="2df8d-187">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2df8d-187">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2df8d-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="2df8d-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="2df8d-189">C#</span><span class="sxs-lookup"><span data-stu-id="2df8d-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2df8d-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2df8d-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2df8d-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2df8d-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2df8d-192">Java</span><span class="sxs-lookup"><span data-stu-id="2df8d-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2df8d-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df8d-193">Response</span></span>

<span data-ttu-id="2df8d-194">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2df8d-194">The following is an example of the response.</span></span>

><span data-ttu-id="2df8d-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2df8d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
