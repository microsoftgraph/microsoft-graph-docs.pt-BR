---
title: Listar transitivo de grupo memberOf
description: Obter grupos e unidades administrativas dos quais o grupo é membro.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: bf4e1365b392736a1856cb8c6284a7a4babc97dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990876"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="11e69-103">Listar transitivo de grupo memberOf</span><span class="sxs-lookup"><span data-stu-id="11e69-103">List group transitive memberOf</span></span>

<span data-ttu-id="11e69-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11e69-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11e69-105">Obter grupos e unidades administrativas dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="11e69-105">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="11e69-106">Essa operação é transitiva e também inclui todos os grupos dos quais esse grupo é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="11e69-106">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="11e69-107">Ao contrário de obter os grupos do Microsoft 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="11e69-107">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="11e69-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="11e69-108">Permissions</span></span>

<span data-ttu-id="11e69-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11e69-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11e69-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11e69-111">Permission type</span></span> | <span data-ttu-id="11e69-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11e69-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="11e69-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11e69-113">Delegated (work or school account)</span></span> | <span data-ttu-id="11e69-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="11e69-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="11e69-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11e69-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11e69-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11e69-116">Not supported.</span></span> |
| <span data-ttu-id="11e69-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11e69-117">Application</span></span> | <span data-ttu-id="11e69-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11e69-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="11e69-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11e69-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="11e69-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="11e69-120">Optional query parameters</span></span>

<span data-ttu-id="11e69-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="11e69-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="11e69-122">O elenco do OData também é habilitado, por exemplo, você pode converter para obter apenas os membros do grupo transitivo de um grupo.</span><span class="sxs-lookup"><span data-stu-id="11e69-122">OData cast is also enabled, for example, you can cast to get just the transitive group members of a group.</span></span> <span data-ttu-id="11e69-123">Você pode usar `$search`na propriedade**displayName**.</span><span class="sxs-lookup"><span data-stu-id="11e69-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="11e69-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="11e69-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="11e69-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="11e69-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11e69-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11e69-126">Request headers</span></span>

| <span data-ttu-id="11e69-127">Nome</span><span class="sxs-lookup"><span data-stu-id="11e69-127">Name</span></span> | <span data-ttu-id="11e69-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="11e69-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="11e69-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="11e69-129">Authorization</span></span>  | <span data-ttu-id="11e69-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11e69-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="11e69-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="11e69-132">ConsistencyLevel</span></span> | <span data-ttu-id="11e69-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="11e69-133">eventual.</span></span> <span data-ttu-id="11e69-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="11e69-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="11e69-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="11e69-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11e69-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11e69-136">Request body</span></span>

<span data-ttu-id="11e69-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11e69-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11e69-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e69-138">Response</span></span>

<span data-ttu-id="11e69-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11e69-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11e69-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="11e69-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-transitive-member-of"></a><span data-ttu-id="11e69-141">Exemplo 1: obter grupos e unidades administrativas dos quais o grupo é um membro transitiva</span><span class="sxs-lookup"><span data-stu-id="11e69-141">Example 1: Get groups and administrative units that the group is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="11e69-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11e69-142">Request</span></span>

<span data-ttu-id="11e69-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11e69-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11e69-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="11e69-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="11e69-145">C#</span><span class="sxs-lookup"><span data-stu-id="11e69-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11e69-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11e69-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11e69-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e69-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="11e69-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e69-148">Response</span></span>

<span data-ttu-id="11e69-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11e69-149">The following is an example of the response.</span></span>
><span data-ttu-id="11e69-150">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="11e69-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="11e69-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11e69-151">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="11e69-152">Exemplo 2: Obter apenas uma contagem de todas as associações transitivas</span><span class="sxs-lookup"><span data-stu-id="11e69-152">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="11e69-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11e69-153">Request</span></span>

<span data-ttu-id="11e69-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11e69-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="11e69-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="11e69-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="11e69-156">C#</span><span class="sxs-lookup"><span data-stu-id="11e69-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11e69-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11e69-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11e69-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e69-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="11e69-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e69-159">Response</span></span>

<span data-ttu-id="11e69-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11e69-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="11e69-161">294</span><span class="sxs-lookup"><span data-stu-id="11e69-161">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="11e69-162">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação transitiva em grupos</span><span class="sxs-lookup"><span data-stu-id="11e69-162">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="11e69-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11e69-163">Request</span></span>

<span data-ttu-id="11e69-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11e69-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="11e69-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="11e69-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="11e69-166">C#</span><span class="sxs-lookup"><span data-stu-id="11e69-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11e69-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11e69-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11e69-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e69-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="11e69-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e69-169">Response</span></span>

<span data-ttu-id="11e69-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11e69-170">The following is an example of the response.</span></span>

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

<span data-ttu-id="11e69-171">294</span><span class="sxs-lookup"><span data-stu-id="11e69-171">294</span></span>


### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="11e69-172">Exemplo 4: usar o $search e o elenco OData para obter associação em grupos com nomes de exibição que contenham as letras de ' camada ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="11e69-172">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="11e69-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11e69-173">Request</span></span>

<span data-ttu-id="11e69-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11e69-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="11e69-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="11e69-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="11e69-176">C#</span><span class="sxs-lookup"><span data-stu-id="11e69-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11e69-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11e69-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11e69-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e69-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="11e69-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e69-179">Response</span></span>

<span data-ttu-id="11e69-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11e69-180">The following is an example of the response.</span></span>
><span data-ttu-id="11e69-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11e69-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="11e69-183">Exemplo 5: usar a conversão OData e $filter para obter associação com um nome de exibição que comece com ' A ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="11e69-183">Example 5: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="11e69-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11e69-184">Request</span></span>

<span data-ttu-id="11e69-185">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11e69-185">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="11e69-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="11e69-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="11e69-187">C#</span><span class="sxs-lookup"><span data-stu-id="11e69-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11e69-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11e69-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11e69-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e69-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="11e69-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e69-190">Response</span></span>

<span data-ttu-id="11e69-191">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11e69-191">The following is an example of the response.</span></span>
><span data-ttu-id="11e69-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11e69-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


