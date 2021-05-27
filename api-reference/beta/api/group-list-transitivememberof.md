---
title: Listar transitivo de grupo memberOf
description: Obter grupos e unidades administrativas de que o grupo é membro.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f2a1daf44989034c02abb780d3d53cdce9c6a166
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681479"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="e7130-103">Listar transitivo de grupo memberOf</span><span class="sxs-lookup"><span data-stu-id="e7130-103">List group transitive memberOf</span></span>

<span data-ttu-id="e7130-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7130-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7130-105">Obter grupos e unidades administrativas de que o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="e7130-105">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="e7130-106">Essa operação é transitiva e também incluirá todos os grupos dos que esses grupos são membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="e7130-106">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="e7130-107">Ao contrário de obter grupos Microsoft 365 usuários, isso retorna todos os tipos de grupos, não apenas Microsoft 365 grupos.</span><span class="sxs-lookup"><span data-stu-id="e7130-107">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7130-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7130-108">Permissions</span></span>

<span data-ttu-id="e7130-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7130-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e7130-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7130-111">Permission type</span></span> | <span data-ttu-id="e7130-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7130-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="e7130-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7130-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e7130-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e7130-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="e7130-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7130-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7130-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7130-116">Not supported.</span></span> |
| <span data-ttu-id="e7130-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7130-117">Application</span></span> | <span data-ttu-id="e7130-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7130-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e7130-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7130-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7130-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e7130-120">Optional query parameters</span></span>

<span data-ttu-id="e7130-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="e7130-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="e7130-122">O OData cast também está habilitado, por exemplo, você pode lançar para obter apenas os membros do grupo transitivo de um grupo.</span><span class="sxs-lookup"><span data-stu-id="e7130-122">OData cast is also enabled, for example, you can cast to get just the transitive group members of a group.</span></span> <span data-ttu-id="e7130-123">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="e7130-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="e7130-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="e7130-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="e7130-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="e7130-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7130-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7130-126">Request headers</span></span>

| <span data-ttu-id="e7130-127">Nome</span><span class="sxs-lookup"><span data-stu-id="e7130-127">Name</span></span> | <span data-ttu-id="e7130-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7130-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="e7130-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7130-129">Authorization</span></span>  | <span data-ttu-id="e7130-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7130-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7130-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="e7130-132">ConsistencyLevel</span></span> | <span data-ttu-id="e7130-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="e7130-133">eventual.</span></span> <span data-ttu-id="e7130-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="e7130-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="e7130-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="e7130-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7130-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7130-136">Request body</span></span>

<span data-ttu-id="e7130-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7130-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7130-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7130-138">Response</span></span>

<span data-ttu-id="e7130-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7130-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e7130-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e7130-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-transitive-member-of"></a><span data-ttu-id="e7130-141">Exemplo 1: Obter grupos e unidades administrativas de que o grupo é um membro transitivo</span><span class="sxs-lookup"><span data-stu-id="e7130-141">Example 1: Get groups and administrative units that the group is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="e7130-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7130-142">Request</span></span>

<span data-ttu-id="e7130-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7130-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e7130-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7130-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="e7130-145">C#</span><span class="sxs-lookup"><span data-stu-id="e7130-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7130-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7130-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7130-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7130-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7130-148">Java</span><span class="sxs-lookup"><span data-stu-id="e7130-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e7130-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7130-149">Response</span></span>

<span data-ttu-id="e7130-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7130-150">The following is an example of the response.</span></span>
><span data-ttu-id="e7130-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e7130-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="e7130-152">Exemplo 2: Obter apenas uma contagem de todas as associações transitivas</span><span class="sxs-lookup"><span data-stu-id="e7130-152">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="e7130-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7130-153">Request</span></span>

<span data-ttu-id="e7130-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7130-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="e7130-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7130-155">Response</span></span>

<span data-ttu-id="e7130-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7130-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="e7130-157">294</span><span class="sxs-lookup"><span data-stu-id="e7130-157">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="e7130-158">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação transitiva em grupos</span><span class="sxs-lookup"><span data-stu-id="e7130-158">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="e7130-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7130-159">Request</span></span>

<span data-ttu-id="e7130-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7130-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="e7130-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7130-161">Response</span></span>

<span data-ttu-id="e7130-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7130-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="e7130-163">294</span><span class="sxs-lookup"><span data-stu-id="e7130-163">294</span></span>


### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="e7130-164">Exemplo 4: use o OData cast e $search para obter associação em grupos com nomes de exibição que contêm as letras 'camada' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="e7130-164">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="e7130-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7130-165">Request</span></span>

<span data-ttu-id="e7130-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7130-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="e7130-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7130-167">Response</span></span>

<span data-ttu-id="e7130-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7130-168">The following is an example of the response.</span></span>
><span data-ttu-id="e7130-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e7130-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="e7130-170">Exemplo 5: Use o OData cast e $filter para obter associação com um nome de exibição que começa com "A" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="e7130-170">Example 5: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="e7130-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7130-171">Request</span></span>

<span data-ttu-id="e7130-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7130-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="e7130-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7130-173">Response</span></span>

<span data-ttu-id="e7130-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7130-174">The following is an example of the response.</span></span>
><span data-ttu-id="e7130-175">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e7130-175">**Note:** The response object shown here might be shortened for readability.</span></span>

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


