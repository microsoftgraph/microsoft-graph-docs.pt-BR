---
title: Listar grupo memberOf
description: Obter grupos e unidades administrativas dos quais o grupo é membro direto.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 79f69deaf2783d01f6fb49e58f46f3e5e3440eaf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954088"
---
# <a name="list-group-memberof"></a><span data-ttu-id="a9630-103">Listar grupo memberOf</span><span class="sxs-lookup"><span data-stu-id="a9630-103">List group memberOf</span></span>

<span data-ttu-id="a9630-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9630-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9630-105">Obter grupos e unidades administrativas dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="a9630-105">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="a9630-p101">Essa operação não é transitiva. Ao contrário de obter Grupos do Microsoft 365 de um usuário, retorna todos os tipos de grupos, não apenas grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a9630-p101">This operation is not transitive. Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a9630-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9630-108">Permissions</span></span>

<span data-ttu-id="a9630-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9630-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9630-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9630-111">Permission type</span></span> | <span data-ttu-id="a9630-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9630-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="a9630-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9630-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a9630-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a9630-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="a9630-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9630-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9630-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9630-116">Not supported.</span></span> |
| <span data-ttu-id="a9630-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9630-117">Application</span></span> | <span data-ttu-id="a9630-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9630-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9630-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9630-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9630-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a9630-120">Optional query parameters</span></span>

<span data-ttu-id="a9630-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="a9630-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="a9630-122">A conversão OData também está habilitada, por exemplo, você pode lançar para obter apenas os grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="a9630-122">OData cast is also enabled, for example, you can cast to get just the groups the group is a member of.</span></span> <span data-ttu-id="a9630-123">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="a9630-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="a9630-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="a9630-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="a9630-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="a9630-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9630-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9630-126">Request headers</span></span>

| <span data-ttu-id="a9630-127">Nome</span><span class="sxs-lookup"><span data-stu-id="a9630-127">Name</span></span> | <span data-ttu-id="a9630-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9630-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="a9630-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9630-129">Authorization</span></span>  | <span data-ttu-id="a9630-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9630-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a9630-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="a9630-132">ConsistencyLevel</span></span> | <span data-ttu-id="a9630-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="a9630-133">eventual.</span></span> <span data-ttu-id="a9630-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="a9630-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="a9630-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="a9630-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9630-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9630-136">Request body</span></span>

<span data-ttu-id="a9630-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9630-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9630-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9630-138">Response</span></span>

<span data-ttu-id="a9630-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9630-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9630-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a9630-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-direct-member-of"></a><span data-ttu-id="a9630-141">Exemplo 1: Obter grupos e unidades administrativas das quais o grupo é membro direto</span><span class="sxs-lookup"><span data-stu-id="a9630-141">Example 1: Get groups and administrative units that the group is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="a9630-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9630-142">Request</span></span>

<span data-ttu-id="a9630-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9630-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9630-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9630-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="a9630-145">C#</span><span class="sxs-lookup"><span data-stu-id="a9630-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9630-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9630-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9630-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9630-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9630-148">Java</span><span class="sxs-lookup"><span data-stu-id="a9630-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a9630-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9630-149">Response</span></span>

<span data-ttu-id="a9630-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9630-150">The following is an example of the response.</span></span>
><span data-ttu-id="a9630-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9630-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="a9630-153">Exemplo 2: Obter apenas uma contagem de todas as associações</span><span class="sxs-lookup"><span data-stu-id="a9630-153">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="a9630-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9630-154">Request</span></span>

<span data-ttu-id="a9630-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9630-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a9630-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9630-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="a9630-157">C#</span><span class="sxs-lookup"><span data-stu-id="a9630-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9630-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9630-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9630-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9630-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9630-160">Java</span><span class="sxs-lookup"><span data-stu-id="a9630-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a9630-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9630-161">Response</span></span>

<span data-ttu-id="a9630-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9630-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="a9630-163">394</span><span class="sxs-lookup"><span data-stu-id="a9630-163">394</span></span>


### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="a9630-164">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="a9630-164">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="a9630-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9630-165">Request</span></span>

<span data-ttu-id="a9630-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9630-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a9630-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9630-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="a9630-168">C#</span><span class="sxs-lookup"><span data-stu-id="a9630-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-group-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9630-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9630-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-group-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9630-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9630-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-group-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9630-171">Java</span><span class="sxs-lookup"><span data-stu-id="a9630-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-group-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a9630-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9630-172">Response</span></span>

<span data-ttu-id="a9630-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9630-173">The following is an example of the response.</span></span>

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

<span data-ttu-id="a9630-174">394</span><span class="sxs-lookup"><span data-stu-id="a9630-174">394</span></span>

### <a name="example-4-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="a9630-175">Exemplo 4: Utilize a conversão OData e $search para obter associação com nomes de exibição que contenham as letras 'Vídeo', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="a9630-175">Example 4: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a9630-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9630-176">Request</span></span>

<span data-ttu-id="a9630-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9630-177">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a9630-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9630-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="a9630-179">C#</span><span class="sxs-lookup"><span data-stu-id="a9630-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-video-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9630-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9630-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-video-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9630-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9630-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-video-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a9630-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9630-182">Response</span></span>

<span data-ttu-id="a9630-183">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9630-183">The following is an example of the response.</span></span>
><span data-ttu-id="a9630-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9630-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.count":1396,
  "value":[
    {
      "displayName":"SFA Videos",
      "mail":"SFAVideos@service.contoso.com",
      "mailNickname":"SFAVideos"
    }
  ]
}
```

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="a9630-186">Exemplo 5: Utilize a conversão OData e $filter para obter associação com um nome de exibição que começa com a letra 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="a9630-186">Example 5: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a9630-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9630-187">Request</span></span>

<span data-ttu-id="a9630-188">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9630-188">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a9630-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9630-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="a9630-190">C#</span><span class="sxs-lookup"><span data-stu-id="a9630-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9630-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9630-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9630-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9630-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9630-193">Java</span><span class="sxs-lookup"><span data-stu-id="a9630-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a9630-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9630-194">Response</span></span>

<span data-ttu-id="a9630-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9630-195">The following is an example of the response.</span></span>
><span data-ttu-id="a9630-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9630-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


