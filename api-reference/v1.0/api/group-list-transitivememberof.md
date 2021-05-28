---
title: Listar transitivo de grupo memberOf
description: Obter grupos dos que o grupo é membro.  Essa operação é transitiva e também incluirá todos os grupos dos que esses grupos são membros aninhados. Ao contrário de obter grupos Microsoft 365 usuários, isso retorna todos os tipos de grupos, não apenas Microsoft 365 grupos.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 738c100738d6eb0b4b2eb49e3b57a32c7f00bb32
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680595"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="85e05-105">Listar transitivo de grupo memberOf</span><span class="sxs-lookup"><span data-stu-id="85e05-105">List group transitive memberOf</span></span>

<span data-ttu-id="85e05-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85e05-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85e05-107">Obter grupos dos que o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="85e05-107">Get groups that the group is a member of.</span></span>  <span data-ttu-id="85e05-108">Essa operação é transitiva e também incluirá todos os grupos dos que esses grupos são membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="85e05-108">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="85e05-109">Ao contrário de obter grupos Microsoft 365 usuários, isso retorna todos os tipos de grupos, não apenas Microsoft 365 grupos.</span><span class="sxs-lookup"><span data-stu-id="85e05-109">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="85e05-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="85e05-110">Permissions</span></span>

<span data-ttu-id="85e05-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85e05-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85e05-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85e05-113">Permission type</span></span>      | <span data-ttu-id="85e05-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85e05-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85e05-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85e05-115">Delegated (work or school account)</span></span> | <span data-ttu-id="85e05-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="85e05-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="85e05-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85e05-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85e05-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85e05-118">Not supported.</span></span>    |
|<span data-ttu-id="85e05-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85e05-119">Application</span></span> | <span data-ttu-id="85e05-120">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85e05-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="85e05-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85e05-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85e05-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="85e05-122">Optional query parameters</span></span>

<span data-ttu-id="85e05-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="85e05-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="85e05-124">O OData cast também está habilitado, por exemplo, você pode lançar para obter apenas os membros do grupo transitivo de um grupo.</span><span class="sxs-lookup"><span data-stu-id="85e05-124">OData cast is also enabled, for example, you can cast to get just the transitive group members of a group.</span></span> <span data-ttu-id="85e05-125">Você pode usar `$search` nas propriedades **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="85e05-125">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="85e05-126">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="85e05-126">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="85e05-127">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="85e05-127">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85e05-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85e05-128">Request headers</span></span>

| <span data-ttu-id="85e05-129">Nome</span><span class="sxs-lookup"><span data-stu-id="85e05-129">Name</span></span> | <span data-ttu-id="85e05-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="85e05-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="85e05-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="85e05-131">Authorization</span></span>  | <span data-ttu-id="85e05-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85e05-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85e05-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="85e05-134">ConsistencyLevel</span></span> | <span data-ttu-id="85e05-135">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="85e05-135">eventual.</span></span> <span data-ttu-id="85e05-136">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="85e05-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="85e05-137">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="85e05-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85e05-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85e05-138">Request body</span></span>
<span data-ttu-id="85e05-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85e05-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85e05-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="85e05-140">Response</span></span>
<span data-ttu-id="85e05-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85e05-141">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85e05-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="85e05-142">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-transitive-member-of"></a><span data-ttu-id="85e05-143">Exemplo 1: Obter grupos e unidades administrativas de que o grupo é um membro transitivo</span><span class="sxs-lookup"><span data-stu-id="85e05-143">Example 1: Get groups and administrative units that the group is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="85e05-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85e05-144">Request</span></span>

<span data-ttu-id="85e05-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="85e05-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85e05-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="85e05-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="85e05-147">C#</span><span class="sxs-lookup"><span data-stu-id="85e05-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85e05-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85e05-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85e05-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85e05-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85e05-150">Java</span><span class="sxs-lookup"><span data-stu-id="85e05-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="85e05-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="85e05-151">Response</span></span>

<span data-ttu-id="85e05-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85e05-152">The following is an example of the response.</span></span>

><span data-ttu-id="85e05-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="85e05-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="85e05-154">Exemplo 2: Obter apenas uma contagem de todas as associações transitivas</span><span class="sxs-lookup"><span data-stu-id="85e05-154">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="85e05-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85e05-155">Request</span></span>

<span data-ttu-id="85e05-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="85e05-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="85e05-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="85e05-157">Response</span></span>

<span data-ttu-id="85e05-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85e05-158">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="85e05-159">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação transitiva em grupos</span><span class="sxs-lookup"><span data-stu-id="85e05-159">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="85e05-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85e05-160">Request</span></span>

<span data-ttu-id="85e05-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="85e05-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="85e05-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="85e05-162">Response</span></span>

<span data-ttu-id="85e05-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85e05-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="85e05-164">Exemplo 4: use o OData cast e $search para obter associação em grupos com nomes de exibição que contêm as letras 'camada' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="85e05-164">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="85e05-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85e05-165">Request</span></span>

<span data-ttu-id="85e05-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="85e05-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="85e05-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="85e05-167">Response</span></span>

<span data-ttu-id="85e05-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85e05-168">The following is an example of the response.</span></span>

><span data-ttu-id="85e05-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="85e05-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="85e05-170">Exemplo 5: Use o OData cast e $filter para obter associação com um nome de exibição que começa com "A" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="85e05-170">Example 5: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="85e05-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85e05-171">Request</span></span>

<span data-ttu-id="85e05-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="85e05-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="85e05-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="85e05-173">Response</span></span>

<span data-ttu-id="85e05-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85e05-174">The following is an example of the response.</span></span>

><span data-ttu-id="85e05-175">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="85e05-175">**Note:** The response object shown here might be shortened for readability.</span></span>

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
