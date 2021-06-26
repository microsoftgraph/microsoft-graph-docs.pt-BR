---
title: Listar membros transitivos de grupo
description: Obter uma lista dos membros do grupo.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 752483696ea527a760fe6c5d97bd0932cb41078c
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151479"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="5685f-103">Listar membros transitivos de grupo</span><span class="sxs-lookup"><span data-stu-id="5685f-103">List group transitive members</span></span>

<span data-ttu-id="5685f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5685f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5685f-105">Obter uma lista dos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="5685f-105">Get a list of the group's members.</span></span> <span data-ttu-id="5685f-106">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="5685f-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="5685f-107">Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="5685f-107">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="5685f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5685f-108">Permissions</span></span>

<span data-ttu-id="5685f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5685f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5685f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5685f-111">Permission type</span></span> | <span data-ttu-id="5685f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5685f-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="5685f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5685f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5685f-114">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5685f-114">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="5685f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5685f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5685f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5685f-116">Not supported.</span></span> |
| <span data-ttu-id="5685f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5685f-117">Application</span></span> | <span data-ttu-id="5685f-118">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5685f-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

> <span data-ttu-id="5685f-119">**Observação:** Para listar os membros de um grupo de associação oculto, a *permissão Member.Read.Hidden* é necessária.</span><span class="sxs-lookup"><span data-stu-id="5685f-119">**Note:** To list the members of a hidden membership group, the *Member.Read.Hidden* permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="5685f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5685f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5685f-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5685f-121">Optional query parameters</span></span>

<span data-ttu-id="5685f-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="5685f-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="5685f-123">Você pode usar `$search` nas propriedades **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="5685f-123">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="5685f-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="5685f-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="5685f-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="5685f-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="5685f-126">Para filtrar os resultados no tipo OData, como `microsoft.graph.user` ou , você deve usar os `microsoft.graph.group` [parâmetros de consulta avançados](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="5685f-126">To filter the results on the OData type, such as `microsoft.graph.user` or `microsoft.graph.group`, you must use the [advanced query parameters](/graph/aad-advanced-queries).</span></span> <span data-ttu-id="5685f-127">Ou seja, o header **ConsistencyLevel** definido como `eventual` e a cadeia de `$count=true` caracteres de consulta.</span><span class="sxs-lookup"><span data-stu-id="5685f-127">That is, the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5685f-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5685f-128">Request headers</span></span>

| <span data-ttu-id="5685f-129">Nome</span><span class="sxs-lookup"><span data-stu-id="5685f-129">Name</span></span> | <span data-ttu-id="5685f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5685f-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="5685f-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="5685f-131">Authorization</span></span>  | <span data-ttu-id="5685f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5685f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5685f-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="5685f-134">ConsistencyLevel</span></span> | <span data-ttu-id="5685f-135">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="5685f-135">eventual.</span></span> <span data-ttu-id="5685f-136">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="5685f-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="5685f-137">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="5685f-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5685f-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5685f-138">Request body</span></span>

<span data-ttu-id="5685f-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5685f-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5685f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5685f-140">Response</span></span>

<span data-ttu-id="5685f-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5685f-141">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5685f-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5685f-142">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="5685f-143">Exemplo 1: Obter a associação transitiva de um grupo</span><span class="sxs-lookup"><span data-stu-id="5685f-143">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="5685f-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5685f-144">Request</span></span>

<span data-ttu-id="5685f-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5685f-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5685f-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5685f-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="5685f-147">C#</span><span class="sxs-lookup"><span data-stu-id="5685f-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5685f-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5685f-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5685f-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5685f-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5685f-150">Java</span><span class="sxs-lookup"><span data-stu-id="5685f-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5685f-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="5685f-151">Response</span></span>

<span data-ttu-id="5685f-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5685f-152">The following is an example of the response.</span></span>

><span data-ttu-id="5685f-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5685f-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="5685f-154">Exemplo 2: Obter apenas uma contagem de associação transitiva</span><span class="sxs-lookup"><span data-stu-id="5685f-154">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="5685f-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5685f-155">Request</span></span>

<span data-ttu-id="5685f-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5685f-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5685f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="5685f-157">Response</span></span>

<span data-ttu-id="5685f-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5685f-158">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

```

`893`


### <a name="example-3-use-the-microsoftgraphgroup-odata-cast-to-get-only-members-that-are-groups"></a><span data-ttu-id="5685f-159">Exemplo 3: Use o odata microsoft.graph.group para obter apenas membros que são grupos</span><span class="sxs-lookup"><span data-stu-id="5685f-159">Example 3: Use the microsoft.graph.group OData cast to get only members that are groups</span></span>

#### <a name="request"></a><span data-ttu-id="5685f-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5685f-160">Request</span></span>

<span data-ttu-id="5685f-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5685f-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_odataCast"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitivemembers/microsoft.graph.group?$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5685f-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="5685f-162">Response</span></span>

<span data-ttu-id="5685f-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5685f-163">The following is an example of the response.</span></span>

><span data-ttu-id="5685f-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5685f-164">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups",
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

### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="5685f-165">Exemplo 4: use o OData cast e $search para obter associação em grupos com nomes de exibição que contêm as letras 'camada' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="5685f-165">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="5685f-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5685f-166">Request</span></span>

<span data-ttu-id="5685f-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5685f-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5685f-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="5685f-168">Response</span></span>

<span data-ttu-id="5685f-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5685f-169">The following is an example of the response.</span></span>
><span data-ttu-id="5685f-170">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5685f-170">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="5685f-171">Exemplo 5: use o OData cast e $filter para obter a associação do usuário em grupos com um nome de exibição que começa com 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="5685f-171">Example 5: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="5685f-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5685f-172">Request</span></span>

<span data-ttu-id="5685f-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5685f-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5685f-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="5685f-174">Response</span></span>

<span data-ttu-id="5685f-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5685f-175">The following is an example of the response.</span></span>
><span data-ttu-id="5685f-176">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5685f-176">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


