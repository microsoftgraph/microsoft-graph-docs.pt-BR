---
title: Listar membros de grupo
description: Obtenha uma lista dos membros diretos do grupo.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a07db7b2ebda91bdbce1d27bb034c50bc8d33902
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041530"
---
# <a name="list-group-members"></a><span data-ttu-id="01412-103">Listar membros de grupo</span><span class="sxs-lookup"><span data-stu-id="01412-103">List group members</span></span>

<span data-ttu-id="01412-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01412-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01412-105">Obtenha uma lista dos membros diretos do grupo.</span><span class="sxs-lookup"><span data-stu-id="01412-105">Get a list of the group's direct members.</span></span> <span data-ttu-id="01412-106">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="01412-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="01412-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="01412-107">This operation is not transitive.</span></span>

<span data-ttu-id="01412-108">Quando um grupo contém mais de 100 membros, o Microsoft Graph retorna uma propriedade `@odata.nextLink` na resposta que contém um URL para a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="01412-108">When a group contains more than 100 members, Microsoft Graph returns a `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="01412-109">Se essa propriedade estiver presente, continue fazendo solicitações adicionais com o `@odata.nextLink` URL em cada resposta, até que todos os resultados sejam retornados, conforme descrito em [paginação de dados do Microsoft Graph no aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="01412-109">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="01412-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="01412-110">Permissions</span></span>

<span data-ttu-id="01412-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01412-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01412-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01412-113">Permission type</span></span> | <span data-ttu-id="01412-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01412-114">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="01412-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01412-115">Delegated (work or school account)</span></span> | <span data-ttu-id="01412-116">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="01412-116">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |
| <span data-ttu-id="01412-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01412-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01412-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01412-118">Not supported.</span></span> |
| <span data-ttu-id="01412-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01412-119">Application</span></span> | <span data-ttu-id="01412-120">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="01412-120">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

> <span data-ttu-id="01412-121">**Observação:** Para listar os membros de um grupo de associação oculto, a permissão Member.Read.Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="01412-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]
 
## <a name="http-request"></a><span data-ttu-id="01412-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01412-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="01412-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="01412-123">Optional query parameters</span></span>

<span data-ttu-id="01412-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="01412-124">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="01412-125">A conversão OData também está habilitada, por exemplo, você pode converter para obter apenas os usuários que são membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="01412-125">OData cast is also enabled, for example, you can cast to get just the users that are a member of the group.</span></span> <span data-ttu-id="01412-126">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="01412-126">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="01412-127">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="01412-127">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="01412-128">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="01412-128">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01412-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01412-129">Request headers</span></span>

| <span data-ttu-id="01412-130">Nome</span><span class="sxs-lookup"><span data-stu-id="01412-130">Name</span></span> | <span data-ttu-id="01412-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="01412-131">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="01412-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="01412-132">Authorization</span></span> | <span data-ttu-id="01412-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01412-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01412-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="01412-135">ConsistencyLevel</span></span> | <span data-ttu-id="01412-136">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="01412-136">eventual.</span></span> <span data-ttu-id="01412-137">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="01412-137">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="01412-138">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="01412-138">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01412-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01412-139">Request body</span></span>

<span data-ttu-id="01412-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="01412-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01412-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="01412-141">Response</span></span>

<span data-ttu-id="01412-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01412-142">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01412-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="01412-143">Examples</span></span>

### <a name="example-1-get-the-direct-membership-in-a-group"></a><span data-ttu-id="01412-144">Exemplo 1: Obtenha a associação direta em um grupo</span><span class="sxs-lookup"><span data-stu-id="01412-144">Example 1: Get the direct membership in a group</span></span>

#### <a name="request"></a><span data-ttu-id="01412-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01412-145">Request</span></span>

<span data-ttu-id="01412-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01412-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01412-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="01412-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="01412-148">C#</span><span class="sxs-lookup"><span data-stu-id="01412-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01412-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01412-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01412-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01412-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01412-151">Java</span><span class="sxs-lookup"><span data-stu-id="01412-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="01412-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="01412-152">Response</span></span>

<span data-ttu-id="01412-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01412-153">The following is an example of the response.</span></span>
><span data-ttu-id="01412-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="01412-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-membership"></a><span data-ttu-id="01412-155">Exemplo 2: Obtenha apenas uma contagem de todos os membros</span><span class="sxs-lookup"><span data-stu-id="01412-155">Example 2: Get only a count of all membership</span></span>

#### <a name="request"></a><span data-ttu-id="01412-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01412-156">Request</span></span>

<span data-ttu-id="01412-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01412-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="01412-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="01412-158">Response</span></span>

<span data-ttu-id="01412-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01412-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="01412-160">893</span><span class="sxs-lookup"><span data-stu-id="01412-160">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-user-membership"></a><span data-ttu-id="01412-161">Exemplo 3: Utilize a conversão OData para obter apenas uma contagem da associação do usuário</span><span class="sxs-lookup"><span data-stu-id="01412-161">Example 3: Use OData cast to get only a count of user membership</span></span>

#### <a name="request"></a><span data-ttu-id="01412-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01412-162">Request</span></span>

<span data-ttu-id="01412-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01412-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_user_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="01412-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="01412-164">Response</span></span>

<span data-ttu-id="01412-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01412-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="01412-166">893</span><span class="sxs-lookup"><span data-stu-id="01412-166">893</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-user-membership-in-groups-with-display-names-that-contain-the-letters-pr-including-a-count-of-returned-objects"></a><span data-ttu-id="01412-167">Exemplo 4: use $search e OData cast para obter a associação do usuário em grupos com nomes de exibição que contêm as letras "Pr" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="01412-167">Example 4: Use $search and OData cast to get user membership in groups with display names that contain the letters 'Pr' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="01412-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01412-168">Request</span></span>

<span data-ttu-id="01412-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01412-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_pr_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user?$count=true&$orderby=displayName&$search="displayName:Pr"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="01412-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="01412-170">Response</span></span>

<span data-ttu-id="01412-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01412-171">The following is an example of the response.</span></span>
><span data-ttu-id="01412-172">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="01412-172">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-filter-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="01412-173">Exemplo 5: Utilize $filter para obter associação de grupo com um nome de exibição que começa com a letra 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="01412-173">Example 5: Use $filter to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="01412-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01412-174">Request</span></span>

<span data-ttu-id="01412-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01412-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members?$count=true&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="01412-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="01412-176">Response</span></span>

<span data-ttu-id="01412-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01412-177">The following is an example of the response.</span></span>
><span data-ttu-id="01412-178">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="01412-178">**Note:** The response object shown here might be shortened for readability.</span></span>

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


