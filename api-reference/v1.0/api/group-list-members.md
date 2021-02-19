---
title: Listar membros
description: Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos organizacionais, dispositivos, entidades de serviço e outros grupos como membros.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a0d9c77bb6fd6bb7685fd13ae816ee5587c01f83
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272195"
---
# <a name="list-members"></a><span data-ttu-id="746ab-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="746ab-104">List members</span></span>

<span data-ttu-id="746ab-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="746ab-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="746ab-106">Obtenha uma lista dos membros diretos do grupo.</span><span class="sxs-lookup"><span data-stu-id="746ab-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="746ab-107">Um grupo pode ter usuários, contatos organizacionais, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="746ab-107">A group can have users, organizational contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="746ab-108">No momento, as entidades de serviço não estão listadas como membros de grupo devido à distribuição em estágios das entidades de serviço para o ponto de extremidade do Graph v 1.0.</span><span class="sxs-lookup"><span data-stu-id="746ab-108">Currently service principals are not listed as group members due to staged roll-out of service principals on Graph V1.0 endpoint.</span></span> <span data-ttu-id="746ab-109">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="746ab-109">This operation is not transitive.</span></span>

<span data-ttu-id="746ab-110">Quando um grupo contém mais de 100 membros, o Microsoft Graph retorna uma propriedade `@odata.nextLink` na resposta que contém um URL para a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="746ab-110">When a group contains more than 100 members, Microsoft Graph returns a `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="746ab-111">Se essa propriedade estiver presente, continue fazendo solicitações adicionais com o `@odata.nextLink` URL em cada resposta, até que todos os resultados sejam retornados, conforme descrito em [paginação de dados do Microsoft Graph no aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="746ab-111">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="746ab-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="746ab-112">Permissions</span></span>
<span data-ttu-id="746ab-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="746ab-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="746ab-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="746ab-115">Permission type</span></span>      | <span data-ttu-id="746ab-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="746ab-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="746ab-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="746ab-117">Delegated (work or school account)</span></span> | <span data-ttu-id="746ab-118">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="746ab-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="746ab-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="746ab-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="746ab-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="746ab-120">Not supported.</span></span>    |
|<span data-ttu-id="746ab-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="746ab-121">Application</span></span> | <span data-ttu-id="746ab-122">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="746ab-122">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="746ab-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="746ab-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="746ab-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="746ab-124">Optional query parameters</span></span>

<span data-ttu-id="746ab-125">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="746ab-125">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="746ab-126">A conversão OData também está habilitada, por exemplo, você pode converter para obter apenas os usuários que são membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="746ab-126">OData cast is also enabled, for example, you can cast to get just the users that are a member of the group.</span></span> <span data-ttu-id="746ab-127">Você pode usar `$search` nas propriedades **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="746ab-127">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="746ab-128">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="746ab-128">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="746ab-129">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="746ab-129">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="746ab-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="746ab-130">Request headers</span></span>

| <span data-ttu-id="746ab-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="746ab-131">Header</span></span>       | <span data-ttu-id="746ab-132">Valor</span><span class="sxs-lookup"><span data-stu-id="746ab-132">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="746ab-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="746ab-133">Authorization</span></span>  | <span data-ttu-id="746ab-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="746ab-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="746ab-136">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="746ab-136">ConsistencyLevel</span></span> | <span data-ttu-id="746ab-137">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="746ab-137">eventual.</span></span> <span data-ttu-id="746ab-138">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="746ab-138">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="746ab-139">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="746ab-139">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="746ab-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="746ab-140">Request body</span></span>
<span data-ttu-id="746ab-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="746ab-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="746ab-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="746ab-142">Response</span></span>
<span data-ttu-id="746ab-143">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="746ab-143">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="746ab-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="746ab-144">Examples</span></span>

### <a name="example-1-get-the-direct-membership-in-a-group"></a><span data-ttu-id="746ab-145">Exemplo 1: Obtenha a associação direta em um grupo</span><span class="sxs-lookup"><span data-stu-id="746ab-145">Example 1: Get the direct membership in a group</span></span>

#### <a name="request"></a><span data-ttu-id="746ab-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="746ab-146">Request</span></span>

<span data-ttu-id="746ab-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="746ab-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="746ab-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="746ab-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="746ab-149">C#</span><span class="sxs-lookup"><span data-stu-id="746ab-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="746ab-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="746ab-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="746ab-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="746ab-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="746ab-152">Java</span><span class="sxs-lookup"><span data-stu-id="746ab-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="746ab-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="746ab-153">Response</span></span>

<span data-ttu-id="746ab-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="746ab-154">The following is an example of the response.</span></span>

><span data-ttu-id="746ab-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="746ab-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "user1@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-membership"></a><span data-ttu-id="746ab-157">Exemplo 2: Obtenha apenas uma contagem de todos os membros</span><span class="sxs-lookup"><span data-stu-id="746ab-157">Example 2: Get only a count of all membership</span></span>

#### <a name="request"></a><span data-ttu-id="746ab-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="746ab-158">Request</span></span>

<span data-ttu-id="746ab-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="746ab-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="746ab-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="746ab-160">Response</span></span>

<span data-ttu-id="746ab-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="746ab-161">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`


### <a name="example-3-use-odata-cast-to-get-only-a-count-of-user-membership"></a><span data-ttu-id="746ab-162">Exemplo 3: Utilize a conversão OData para obter apenas uma contagem da associação do usuário</span><span class="sxs-lookup"><span data-stu-id="746ab-162">Example 3: Use OData cast to get only a count of user membership</span></span>

#### <a name="request"></a><span data-ttu-id="746ab-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="746ab-163">Request</span></span>

<span data-ttu-id="746ab-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="746ab-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_user_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members/microsoft.graph.user/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="746ab-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="746ab-165">Response</span></span>

<span data-ttu-id="746ab-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="746ab-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-4-use-searchand-odata-cast-to-get-user-membership-in-groups-with-display-names-that-contain-the-letters-pr-including-a-count-of-returned-objects"></a><span data-ttu-id="746ab-167">Exemplo 4: Utilize $ searchand conversão OData para obter a participação do usuário em grupos com nomes de exibição que contenham as letras 'Pr', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="746ab-167">Example 4: Use $searchand OData cast to get user membership in groups with display names that contain the letters 'Pr' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="746ab-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="746ab-168">Request</span></span>

<span data-ttu-id="746ab-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="746ab-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_pr_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members/microsoft.graph.user?$count=true&$orderby=displayName&$search="displayName:Pr"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="746ab-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="746ab-170">Response</span></span>

<span data-ttu-id="746ab-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="746ab-171">The following is an example of the response.</span></span>

><span data-ttu-id="746ab-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="746ab-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    },
    {
      "displayName":"Preston Morales",
      "id":"66666666-7777-8888-9999-000000000000"
    }
  ]
}
```

### <a name="example-5-use-filter-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="746ab-174">Exemplo 5: Utilize $filter para obter associação de grupo com um nome de exibição que começa com a letra 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="746ab-174">Example 5: Use $filter to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="746ab-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="746ab-175">Request</span></span>

<span data-ttu-id="746ab-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="746ab-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members?$count=true&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="746ab-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="746ab-177">Response</span></span>

<span data-ttu-id="746ab-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="746ab-178">The following is an example of the response.</span></span>

><span data-ttu-id="746ab-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="746ab-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
