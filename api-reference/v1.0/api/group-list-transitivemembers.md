---
title: Listar membros transitivos de grupo
description: Obter uma lista dos membros do grupo. Um grupo pode ter usuários, dispositivos, contatos organizacionais e outros grupos como membros. Essa operação é transitiva e retorna uma lista simples de todos os membros aninhados.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: bd3d6d8bbb301d29458770458529446e560f3be1
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151633"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="0052c-105">Listar membros transitivos de grupo</span><span class="sxs-lookup"><span data-stu-id="0052c-105">List group transitive members</span></span>

<span data-ttu-id="0052c-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0052c-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0052c-107">Obter uma lista dos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="0052c-107">Get a list of the group's members.</span></span> <span data-ttu-id="0052c-108">Um grupo pode ter usuários, dispositivos, contatos organizacionais e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="0052c-108">A group can have users, devices, organizational contacts, and other groups as members.</span></span> <span data-ttu-id="0052c-109">Essa operação é transitiva e retorna uma lista simples de todos os membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="0052c-109">This operation is transitive and returns a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="0052c-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="0052c-110">Permissions</span></span>

<span data-ttu-id="0052c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0052c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0052c-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0052c-113">Permission type</span></span>      | <span data-ttu-id="0052c-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0052c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0052c-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0052c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0052c-116">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0052c-116">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="0052c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0052c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0052c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0052c-118">Not supported.</span></span>    |
|<span data-ttu-id="0052c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0052c-119">Application</span></span> | <span data-ttu-id="0052c-120">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0052c-120">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

><span data-ttu-id="0052c-121">**Observação:** Para listar os membros de um grupo de associação oculto, a *permissão Member.Read.Hidden* é necessária.</span><span class="sxs-lookup"><span data-stu-id="0052c-121">**Note:** To list the members of a hidden membership group, the *Member.Read.Hidden* permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0052c-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0052c-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0052c-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0052c-123">Optional query parameters</span></span>

<span data-ttu-id="0052c-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="0052c-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="0052c-125">Você pode usar `$search` nas propriedades **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="0052c-125">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="0052c-126">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="0052c-126">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="0052c-127">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="0052c-127">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="0052c-128">Para filtrar os resultados no tipo OData, como `microsoft.graph.user` ou , você deve usar os `microsoft.graph.group` [parâmetros de consulta avançados](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="0052c-128">To filter the results on the OData type, such as `microsoft.graph.user` or `microsoft.graph.group`, you must use the [advanced query parameters](/graph/aad-advanced-queries).</span></span> <span data-ttu-id="0052c-129">Ou seja, o header **ConsistencyLevel** definido como `eventual` e a cadeia de `$count=true` caracteres de consulta.</span><span class="sxs-lookup"><span data-stu-id="0052c-129">That is, the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0052c-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0052c-130">Request headers</span></span>

| <span data-ttu-id="0052c-131">Nome</span><span class="sxs-lookup"><span data-stu-id="0052c-131">Name</span></span> | <span data-ttu-id="0052c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0052c-132">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="0052c-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="0052c-133">Authorization</span></span>  | <span data-ttu-id="0052c-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0052c-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0052c-136">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="0052c-136">ConsistencyLevel</span></span> | <span data-ttu-id="0052c-137">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="0052c-137">eventual.</span></span> <span data-ttu-id="0052c-138">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="0052c-138">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="0052c-139">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="0052c-139">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0052c-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0052c-140">Request body</span></span>

<span data-ttu-id="0052c-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0052c-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0052c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0052c-142">Response</span></span>

<span data-ttu-id="0052c-143">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0052c-143">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0052c-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0052c-144">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="0052c-145">Exemplo 1: Obter a associação transitiva de um grupo</span><span class="sxs-lookup"><span data-stu-id="0052c-145">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="0052c-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0052c-146">Request</span></span>

<span data-ttu-id="0052c-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0052c-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0052c-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="0052c-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="0052c-149">C#</span><span class="sxs-lookup"><span data-stu-id="0052c-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0052c-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0052c-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0052c-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0052c-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0052c-152">Java</span><span class="sxs-lookup"><span data-stu-id="0052c-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0052c-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0052c-153">Response</span></span>

<span data-ttu-id="0052c-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0052c-154">The following is an example of the response.</span></span>

><span data-ttu-id="0052c-155">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0052c-155">**Note**: The response object shown here might be shortened for readability.</span></span>

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
      "@odata.type": "#microsoft.graph.user",
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="0052c-156">Exemplo 2: Obter apenas uma contagem de associação transitiva</span><span class="sxs-lookup"><span data-stu-id="0052c-156">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="0052c-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0052c-157">Request</span></span>

<span data-ttu-id="0052c-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0052c-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0052c-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="0052c-159">Response</span></span>

<span data-ttu-id="0052c-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0052c-160">The following is an example of the response.</span></span>

><span data-ttu-id="0052c-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0052c-161">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

```

`893`

### <a name="example-3-use-the-microsoftgraphgroup-odata-cast-to-get-only-members-that-are-groups"></a><span data-ttu-id="0052c-162">Exemplo 3: Use o odata microsoft.graph.group para obter apenas membros que são grupos</span><span class="sxs-lookup"><span data-stu-id="0052c-162">Example 3: Use the microsoft.graph.group OData cast to get only members that are groups</span></span>

#### <a name="request"></a><span data-ttu-id="0052c-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0052c-163">Request</span></span>

<span data-ttu-id="0052c-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0052c-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_odataCast"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitivemembers/microsoft.graph.group?$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0052c-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="0052c-165">Response</span></span>

<span data-ttu-id="0052c-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0052c-166">The following is an example of the response.</span></span>

><span data-ttu-id="0052c-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0052c-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.count": 2,
  "value": [
    {
      "@odata.id": "https://graph.microsoft.com/v2/927c6607-8060-4f4a-a5f8-34964ac78d70/directoryObjects/4d0ef681-e88f-42a3-a2db-e6bf1e249e10/Microsoft.DirectoryServices.Group",
      "id": "4d0ef681-e88f-42a3-a2db-e6bf1e249e10",
      "organizationId": "927c6607-8060-4f4a-a5f8-34964ac78d70",
      "description": null,
      "displayName": "Executives",
      "groupTypes": [],
      "mail": "Executives@contoso.com",
      "mailEnabled": true,
      "mailNickname": "Executives",
    },
    {
      "@odata.id": "https://graph.microsoft.com/v2/927c6607-8060-4f4a-a5f8-34964ac78d70/directoryObjects/d9fb0c47-c783-40a1-bce1-53b52ada51fc/Microsoft.DirectoryServices.Group",
      "id": "d9fb0c47-c783-40a1-bce1-53b52ada51fc",
      "organizationId": "927c6607-8060-4f4a-a5f8-34964ac78d70",
      "displayName": "Project Falcon",
      "groupTypes": [],
      "mail": "Falcon@contoso.com",
      "mailEnabled": true,
      "mailNickname": "Falcon",
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="0052c-168">Exemplo 4: use o OData cast e $search para obter associação em grupos com nomes de exibição que contêm as letras 'camada' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="0052c-168">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0052c-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0052c-169">Request</span></span>

<span data-ttu-id="0052c-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0052c-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0052c-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="0052c-171">Response</span></span>

<span data-ttu-id="0052c-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0052c-172">The following is an example of the response.</span></span>

><span data-ttu-id="0052c-173">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0052c-173">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Joseph Price",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```


### <a name="example-5-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="0052c-174">Exemplo 5: use o OData cast e $filter para obter a associação do usuário em grupos com um nome de exibição que começa com 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="0052c-174">Example 5: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0052c-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0052c-175">Request</span></span>

<span data-ttu-id="0052c-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0052c-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0052c-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="0052c-177">Response</span></span>

<span data-ttu-id="0052c-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0052c-178">The following is an example of the response.</span></span>

><span data-ttu-id="0052c-179">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0052c-179">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
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
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
