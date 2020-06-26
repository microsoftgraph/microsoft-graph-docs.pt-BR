---
title: Lista de grupos transitivos transitivos
description: Obter grupos e unidades administrativas dos quais o grupo é membro.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 81504242e1f5fed670cc783dfc500c4502272ffc
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895829"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="a932f-103">Lista de grupos transitivos transitivos</span><span class="sxs-lookup"><span data-stu-id="a932f-103">List group transitive memberOf</span></span>

<span data-ttu-id="a932f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a932f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a932f-105">Obter grupos e unidades administrativas dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="a932f-105">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="a932f-106">Essa operação é transitiva e também inclui todos os grupos dos quais esse grupo é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="a932f-106">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="a932f-107">Ao contrário de obter os grupos do Microsoft 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a932f-107">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="a932f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a932f-108">Permissions</span></span>

<span data-ttu-id="a932f-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a932f-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a932f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a932f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a932f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a932f-111">Permission type</span></span> | <span data-ttu-id="a932f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a932f-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="a932f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a932f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a932f-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a932f-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="a932f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a932f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a932f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a932f-116">Not supported.</span></span> |
| <span data-ttu-id="a932f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a932f-117">Application</span></span> | <span data-ttu-id="a932f-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a932f-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a932f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a932f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a932f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a932f-120">Optional query parameters</span></span>

<span data-ttu-id="a932f-121">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search` , `$count` e `$filter` .</span><span class="sxs-lookup"><span data-stu-id="a932f-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="a932f-122">O elenco do OData também é habilitado, por exemplo, você pode converter para obter apenas os membros do grupo transitivo de um grupo.</span><span class="sxs-lookup"><span data-stu-id="a932f-122">OData cast is also enabled, for example, you can cast to get just the transitive group members of a group.</span></span> <span data-ttu-id="a932f-123">Você pode usar `$search` na propriedade **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="a932f-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="a932f-124">Quando os itens são adicionados ou atualizados para esse recurso, eles são especialmente indexados para uso com os `$count` `$search` parâmetros de consulta e.</span><span class="sxs-lookup"><span data-stu-id="a932f-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="a932f-125">Pode haver um ligeiro atraso entre a adição ou atualização de um item e quando ele está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="a932f-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a932f-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a932f-126">Request headers</span></span>

| <span data-ttu-id="a932f-127">Nome</span><span class="sxs-lookup"><span data-stu-id="a932f-127">Name</span></span> | <span data-ttu-id="a932f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a932f-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="a932f-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="a932f-129">Authorization</span></span>  | <span data-ttu-id="a932f-130">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="a932f-130">Bearer {token}.</span></span> <span data-ttu-id="a932f-131">Required.</span><span class="sxs-lookup"><span data-stu-id="a932f-131">Required.</span></span> |
| <span data-ttu-id="a932f-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="a932f-132">ConsistencyLevel</span></span> | <span data-ttu-id="a932f-133">ocorra.</span><span class="sxs-lookup"><span data-stu-id="a932f-133">eventual.</span></span> <span data-ttu-id="a932f-134">Esse cabeçalho e `$count` são necessários ao usar os `$search` parâmetros de consulta de conversão de,, `$filter` `$orderby` ou OData.</span><span class="sxs-lookup"><span data-stu-id="a932f-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="a932f-135">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="a932f-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a932f-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a932f-136">Request body</span></span>

<span data-ttu-id="a932f-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a932f-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a932f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a932f-138">Response</span></span>

<span data-ttu-id="a932f-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a932f-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a932f-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a932f-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-transitive-member-of"></a><span data-ttu-id="a932f-141">Exemplo 1: obter grupos e unidades administrativas dos quais o grupo é um membro transitiva</span><span class="sxs-lookup"><span data-stu-id="a932f-141">Example 1: Get groups and administrative units that the group is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="a932f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a932f-142">Request</span></span>

<span data-ttu-id="a932f-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a932f-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a932f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a932f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="a932f-145">C#</span><span class="sxs-lookup"><span data-stu-id="a932f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a932f-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a932f-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a932f-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a932f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a932f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a932f-148">Response</span></span>

<span data-ttu-id="a932f-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a932f-149">The following is an example of the response.</span></span>
><span data-ttu-id="a932f-150">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a932f-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a932f-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a932f-151">All the properties will be returned from an actual call.</span></span>

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
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com",
      "mailEnabled": true,
      "mailNickname": "ContosoGroup1",
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="a932f-152">Exemplo 2: obter apenas uma contagem de todas as associações transitivas</span><span class="sxs-lookup"><span data-stu-id="a932f-152">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="a932f-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a932f-153">Request</span></span>

<span data-ttu-id="a932f-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a932f-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a932f-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="a932f-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="a932f-156">C#</span><span class="sxs-lookup"><span data-stu-id="a932f-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a932f-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a932f-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a932f-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a932f-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a932f-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="a932f-159">Response</span></span>

<span data-ttu-id="a932f-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a932f-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="a932f-161">294</span><span class="sxs-lookup"><span data-stu-id="a932f-161">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="a932f-162">Exemplo 3: usar a conversão OData para obter apenas uma contagem de associação transitiva em grupos</span><span class="sxs-lookup"><span data-stu-id="a932f-162">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="a932f-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a932f-163">Request</span></span>

<span data-ttu-id="a932f-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a932f-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a932f-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="a932f-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="a932f-166">C#</span><span class="sxs-lookup"><span data-stu-id="a932f-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a932f-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a932f-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a932f-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a932f-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a932f-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="a932f-169">Response</span></span>

<span data-ttu-id="a932f-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a932f-170">The following is an example of the response.</span></span>

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

<span data-ttu-id="a932f-171">294</span><span class="sxs-lookup"><span data-stu-id="a932f-171">294</span></span>


### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="a932f-172">Exemplo 4: usar o $search e o elenco OData para obter associação em grupos com nomes de exibição que contenham as letras de ' camada ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="a932f-172">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a932f-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a932f-173">Request</span></span>

<span data-ttu-id="a932f-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a932f-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a932f-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="a932f-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="a932f-176">C#</span><span class="sxs-lookup"><span data-stu-id="a932f-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a932f-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a932f-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a932f-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a932f-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a932f-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="a932f-179">Response</span></span>

<span data-ttu-id="a932f-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a932f-180">The following is an example of the response.</span></span>
><span data-ttu-id="a932f-181">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="a932f-181">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a932f-182">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a932f-182">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="a932f-183">Exemplo 5: usar a conversão OData e $filter para obter associação com um nome de exibição que comece com ' A ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="a932f-183">Example 5: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a932f-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a932f-184">Request</span></span>

<span data-ttu-id="a932f-185">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a932f-185">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a932f-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="a932f-186">Response</span></span>

<span data-ttu-id="a932f-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a932f-187">The following is an example of the response.</span></span>
><span data-ttu-id="a932f-188">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="a932f-188">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a932f-189">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a932f-189">All the properties will be returned from an actual call.</span></span>

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
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
