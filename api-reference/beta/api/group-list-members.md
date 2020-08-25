---
title: Listar membros de grupo
description: Obtenha uma lista dos membros diretos do grupo.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 302d0aa62f078e4209ca59b3fbfcfbb94d692bd9
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872634"
---
# <a name="list-group-members"></a><span data-ttu-id="235b3-103">Listar membros de grupo</span><span class="sxs-lookup"><span data-stu-id="235b3-103">List group members</span></span>

<span data-ttu-id="235b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="235b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="235b3-105">Obtenha uma lista dos membros diretos do grupo.</span><span class="sxs-lookup"><span data-stu-id="235b3-105">Get a list of the group's direct members.</span></span> <span data-ttu-id="235b3-106">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="235b3-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="235b3-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="235b3-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="235b3-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="235b3-108">Permissions</span></span>

<span data-ttu-id="235b3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="235b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="235b3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="235b3-111">Permission type</span></span> | <span data-ttu-id="235b3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="235b3-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="235b3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="235b3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="235b3-114">User. ReadBasic. All, User. Read. All, Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="235b3-114">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="235b3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="235b3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="235b3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="235b3-116">Not supported.</span></span> |
| <span data-ttu-id="235b3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="235b3-117">Application</span></span> | <span data-ttu-id="235b3-118">Group. Read. All, User. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="235b3-118">Group.Read.All, User.Read.All, Directory.Read.All</span></span> |

> <span data-ttu-id="235b3-119">**Observação:** Para listar os membros de um grupo de associação oculto, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="235b3-119">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]
 
## <a name="http-request"></a><span data-ttu-id="235b3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="235b3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="235b3-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="235b3-121">Optional query parameters</span></span>

<span data-ttu-id="235b3-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="235b3-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="235b3-123">O elenco do OData também é habilitado, por exemplo, você pode transmitir para obter apenas os usuários que são membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="235b3-123">OData cast is also enabled, for example, you can cast to get just the users that are a member of the group.</span></span> <span data-ttu-id="235b3-124">Você pode usar `$search`na propriedade**displayName**.</span><span class="sxs-lookup"><span data-stu-id="235b3-124">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="235b3-125">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="235b3-125">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="235b3-126">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="235b3-126">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="235b3-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="235b3-127">Request headers</span></span>

| <span data-ttu-id="235b3-128">Nome</span><span class="sxs-lookup"><span data-stu-id="235b3-128">Name</span></span> | <span data-ttu-id="235b3-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="235b3-129">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="235b3-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="235b3-130">Authorization</span></span> | <span data-ttu-id="235b3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="235b3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="235b3-133">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="235b3-133">ConsistencyLevel</span></span> | <span data-ttu-id="235b3-134">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="235b3-134">eventual.</span></span> <span data-ttu-id="235b3-135">Esse cabeçalho e `$count` são necessários ao usar os `$search` parâmetros de consulta de conversão de,, `$filter` `$orderby` ou OData.</span><span class="sxs-lookup"><span data-stu-id="235b3-135">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="235b3-136">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="235b3-136">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="235b3-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="235b3-137">Request body</span></span>

<span data-ttu-id="235b3-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="235b3-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="235b3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="235b3-139">Response</span></span>

<span data-ttu-id="235b3-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="235b3-140">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="235b3-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="235b3-141">Examples</span></span>

### <a name="example-1-get-the-direct-membership-in-a-group"></a><span data-ttu-id="235b3-142">Exemplo 1: obter a associação direta em um grupo</span><span class="sxs-lookup"><span data-stu-id="235b3-142">Example 1: Get the direct membership in a group</span></span>

#### <a name="request"></a><span data-ttu-id="235b3-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="235b3-143">Request</span></span>

<span data-ttu-id="235b3-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="235b3-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="235b3-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="235b3-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="235b3-146">C#</span><span class="sxs-lookup"><span data-stu-id="235b3-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="235b3-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="235b3-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="235b3-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="235b3-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="235b3-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="235b3-149">Response</span></span>

<span data-ttu-id="235b3-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="235b3-150">The following is an example of the response.</span></span>
><span data-ttu-id="235b3-151">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="235b3-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="235b3-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="235b3-152">All the properties will be returned from an actual call.</span></span>

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
      "mailNickname": "Contoso1",
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-membership"></a><span data-ttu-id="235b3-153">Exemplo 2: obter apenas uma contagem de todas as associações</span><span class="sxs-lookup"><span data-stu-id="235b3-153">Example 2: Get only a count of all membership</span></span>

#### <a name="request"></a><span data-ttu-id="235b3-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="235b3-154">Request</span></span>

<span data-ttu-id="235b3-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="235b3-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="235b3-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="235b3-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="235b3-157">C#</span><span class="sxs-lookup"><span data-stu-id="235b3-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="235b3-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="235b3-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="235b3-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="235b3-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="235b3-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="235b3-160">Response</span></span>

<span data-ttu-id="235b3-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="235b3-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="235b3-162">893</span><span class="sxs-lookup"><span data-stu-id="235b3-162">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-user-membership"></a><span data-ttu-id="235b3-163">Exemplo 3: usar a conversão OData para obter apenas uma contagem de membros do usuário</span><span class="sxs-lookup"><span data-stu-id="235b3-163">Example 3: Use OData cast to get only a count of user membership</span></span>

#### <a name="request"></a><span data-ttu-id="235b3-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="235b3-164">Request</span></span>

<span data-ttu-id="235b3-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="235b3-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="235b3-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="235b3-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_user_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="235b3-167">C#</span><span class="sxs-lookup"><span data-stu-id="235b3-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-user-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="235b3-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="235b3-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-user-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="235b3-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="235b3-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-user-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="235b3-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="235b3-170">Response</span></span>

<span data-ttu-id="235b3-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="235b3-171">The following is an example of the response.</span></span>

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

<span data-ttu-id="235b3-172">893</span><span class="sxs-lookup"><span data-stu-id="235b3-172">893</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-user-membership-in-groups-with-display-names-that-contain-the-letters-pr-including-a-count-of-returned-objects"></a><span data-ttu-id="235b3-173">Exemplo 4: Use $search e a conversão OData para obter a associação do usuário em grupos com nomes para exibição que contenham as letras "PR", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="235b3-173">Example 4: Use $search and OData cast to get user membership in groups with display names that contain the letters 'Pr' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="235b3-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="235b3-174">Request</span></span>

<span data-ttu-id="235b3-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="235b3-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="235b3-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="235b3-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_pr_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user?$count=true&$orderby=displayName&$search="displayName:Pr"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="235b3-177">C#</span><span class="sxs-lookup"><span data-stu-id="235b3-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-pr-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="235b3-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="235b3-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-pr-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="235b3-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="235b3-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-pr-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="235b3-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="235b3-180">Response</span></span>

<span data-ttu-id="235b3-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="235b3-181">The following is an example of the response.</span></span>
><span data-ttu-id="235b3-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="235b3-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Joseph Price",
      "id":"11111111-2222-3333-4444-555555555555"
    },
    {
      "displayName":"Preston Morales",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="235b3-184">Exemplo 5: use $filter para obter a associação de grupo com um nome de exibição que comece com a letra "A", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="235b3-184">Example 5: Use $filter to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="235b3-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="235b3-185">Request</span></span>

<span data-ttu-id="235b3-186">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="235b3-186">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="235b3-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="235b3-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members?$count=true&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="235b3-188">C#</span><span class="sxs-lookup"><span data-stu-id="235b3-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="235b3-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="235b3-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="235b3-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="235b3-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="235b3-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="235b3-191">Response</span></span>

<span data-ttu-id="235b3-192">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="235b3-192">The following is an example of the response.</span></span>
><span data-ttu-id="235b3-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="235b3-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
