---
title: Listar transitivo de grupo memberOf
description: Obter grupos dos quais o grupo é membro.  Essa operação é transitiva e também inclui todos os grupos dos quais esse grupo é um membro aninhado. Ao contrário de obter os grupos do Microsoft 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos da Microsoft 365.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4c4227298ef0e6bcd7487786ef4454400bf8b083
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904900"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="e73fc-105">Listar transitivo de grupo memberOf</span><span class="sxs-lookup"><span data-stu-id="e73fc-105">List group transitive memberOf</span></span>

<span data-ttu-id="e73fc-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e73fc-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e73fc-107">Obter grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="e73fc-107">Get groups that the group is a member of.</span></span>  <span data-ttu-id="e73fc-108">Essa operação é transitiva e também inclui todos os grupos dos quais esse grupo é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="e73fc-108">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="e73fc-109">Ao contrário de obter os grupos do Microsoft 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e73fc-109">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="e73fc-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e73fc-110">Permissions</span></span>

<span data-ttu-id="e73fc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e73fc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e73fc-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e73fc-113">Permission type</span></span>      | <span data-ttu-id="e73fc-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e73fc-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e73fc-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e73fc-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e73fc-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e73fc-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e73fc-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e73fc-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e73fc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e73fc-118">Not supported.</span></span>    |
|<span data-ttu-id="e73fc-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e73fc-119">Application</span></span> | <span data-ttu-id="e73fc-120">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e73fc-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e73fc-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e73fc-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e73fc-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e73fc-122">Optional query parameters</span></span>

<span data-ttu-id="e73fc-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="e73fc-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="e73fc-124">O elenco do OData também é habilitado, por exemplo, você pode converter para obter apenas os membros do grupo transitivo de um grupo.</span><span class="sxs-lookup"><span data-stu-id="e73fc-124">OData cast is also enabled, for example, you can cast to get just the transitive group members of a group.</span></span> <span data-ttu-id="e73fc-125">Você pode usar `$search` nas propriedades **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="e73fc-125">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="e73fc-126">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="e73fc-126">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="e73fc-127">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="e73fc-127">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e73fc-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e73fc-128">Request headers</span></span>

| <span data-ttu-id="e73fc-129">Nome</span><span class="sxs-lookup"><span data-stu-id="e73fc-129">Name</span></span> | <span data-ttu-id="e73fc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e73fc-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="e73fc-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="e73fc-131">Authorization</span></span>  | <span data-ttu-id="e73fc-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e73fc-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e73fc-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="e73fc-134">ConsistencyLevel</span></span> | <span data-ttu-id="e73fc-135">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="e73fc-135">eventual.</span></span> <span data-ttu-id="e73fc-136">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="e73fc-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="e73fc-137">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="e73fc-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e73fc-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e73fc-138">Request body</span></span>
<span data-ttu-id="e73fc-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e73fc-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e73fc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e73fc-140">Response</span></span>
<span data-ttu-id="e73fc-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e73fc-141">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e73fc-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e73fc-142">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-transitive-member-of"></a><span data-ttu-id="e73fc-143">Exemplo 1: obter grupos e unidades administrativas dos quais o grupo é um membro transitiva</span><span class="sxs-lookup"><span data-stu-id="e73fc-143">Example 1: Get groups and administrative units that the group is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="e73fc-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e73fc-144">Request</span></span>

<span data-ttu-id="e73fc-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e73fc-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e73fc-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="e73fc-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="e73fc-147">C#</span><span class="sxs-lookup"><span data-stu-id="e73fc-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e73fc-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e73fc-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e73fc-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e73fc-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e73fc-150">Java</span><span class="sxs-lookup"><span data-stu-id="e73fc-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e73fc-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e73fc-151">Response</span></span>

<span data-ttu-id="e73fc-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e73fc-152">The following is an example of the response.</span></span>

><span data-ttu-id="e73fc-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e73fc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="e73fc-155">Exemplo 2: Obter apenas uma contagem de todas as associações transitivas</span><span class="sxs-lookup"><span data-stu-id="e73fc-155">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="e73fc-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e73fc-156">Request</span></span>

<span data-ttu-id="e73fc-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e73fc-157">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e73fc-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="e73fc-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="e73fc-159">C#</span><span class="sxs-lookup"><span data-stu-id="e73fc-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e73fc-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e73fc-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e73fc-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e73fc-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e73fc-162">Java</span><span class="sxs-lookup"><span data-stu-id="e73fc-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e73fc-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="e73fc-163">Response</span></span>

<span data-ttu-id="e73fc-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e73fc-164">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="e73fc-165">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação transitiva em grupos</span><span class="sxs-lookup"><span data-stu-id="e73fc-165">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="e73fc-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e73fc-166">Request</span></span>

<span data-ttu-id="e73fc-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e73fc-167">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e73fc-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="e73fc-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="e73fc-169">C#</span><span class="sxs-lookup"><span data-stu-id="e73fc-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e73fc-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e73fc-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e73fc-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e73fc-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e73fc-172">Java</span><span class="sxs-lookup"><span data-stu-id="e73fc-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e73fc-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="e73fc-173">Response</span></span>

<span data-ttu-id="e73fc-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e73fc-174">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="e73fc-175">Exemplo 4: usar o $search e o elenco OData para obter associação em grupos com nomes de exibição que contenham as letras de ' camada ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="e73fc-175">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="e73fc-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e73fc-176">Request</span></span>

<span data-ttu-id="e73fc-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e73fc-177">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e73fc-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="e73fc-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="e73fc-179">C#</span><span class="sxs-lookup"><span data-stu-id="e73fc-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e73fc-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e73fc-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e73fc-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e73fc-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e73fc-182">Java</span><span class="sxs-lookup"><span data-stu-id="e73fc-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e73fc-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="e73fc-183">Response</span></span>

<span data-ttu-id="e73fc-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e73fc-184">The following is an example of the response.</span></span>

><span data-ttu-id="e73fc-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e73fc-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="e73fc-187">Exemplo 5: usar a conversão OData e $filter para obter associação com um nome de exibição que comece com ' A ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="e73fc-187">Example 5: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="e73fc-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e73fc-188">Request</span></span>

<span data-ttu-id="e73fc-189">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e73fc-189">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e73fc-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="e73fc-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="e73fc-191">C#</span><span class="sxs-lookup"><span data-stu-id="e73fc-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e73fc-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e73fc-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e73fc-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e73fc-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e73fc-194">Java</span><span class="sxs-lookup"><span data-stu-id="e73fc-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e73fc-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="e73fc-195">Response</span></span>

<span data-ttu-id="e73fc-196">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e73fc-196">The following is an example of the response.</span></span>

><span data-ttu-id="e73fc-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e73fc-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "mail":"AADContoso_Users@contoso.com"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
