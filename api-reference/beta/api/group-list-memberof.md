---
title: Grupo de lista memberOf
description: Obter grupos e unidades administrativas dos quais o grupo é membro direto.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 838b154f98a175cdbd50e0448c16b6fddc0ed382
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332936"
---
# <a name="list-group-memberof"></a><span data-ttu-id="7ab55-103">Grupo de lista memberOf</span><span class="sxs-lookup"><span data-stu-id="7ab55-103">List group memberOf</span></span>

<span data-ttu-id="7ab55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ab55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ab55-105">Obter grupos e unidades administrativas dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="7ab55-105">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="7ab55-p101">Essa operação não é transitiva. Ao contrário de obter os grupos do Office 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="7ab55-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7ab55-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ab55-108">Permissions</span></span>

<span data-ttu-id="7ab55-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ab55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7ab55-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ab55-111">Permission type</span></span> | <span data-ttu-id="7ab55-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ab55-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="7ab55-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ab55-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7ab55-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7ab55-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="7ab55-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ab55-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ab55-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ab55-116">Not supported.</span></span> |
| <span data-ttu-id="7ab55-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ab55-117">Application</span></span> | <span data-ttu-id="7ab55-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ab55-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ab55-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ab55-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7ab55-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7ab55-120">Optional query parameters</span></span>

<span data-ttu-id="7ab55-121">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search` , `$count` e `$filter` .</span><span class="sxs-lookup"><span data-stu-id="7ab55-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="7ab55-122">A conversão OData também é habilitada, por exemplo, você pode transmitir para obter apenas os grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="7ab55-122">OData cast is also enabled, for example, you can cast to get just the groups the group is a member of.</span></span> <span data-ttu-id="7ab55-123">Você pode usar `$search` na propriedade **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="7ab55-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="7ab55-124">Quando os itens são adicionados ou atualizados para esse recurso, eles são especialmente indexados para uso com os `$count` `$search` parâmetros de consulta e.</span><span class="sxs-lookup"><span data-stu-id="7ab55-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="7ab55-125">Pode haver um ligeiro atraso entre a adição ou atualização de um item e quando ele está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="7ab55-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ab55-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ab55-126">Request headers</span></span>

| <span data-ttu-id="7ab55-127">Nome</span><span class="sxs-lookup"><span data-stu-id="7ab55-127">Name</span></span> | <span data-ttu-id="7ab55-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ab55-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="7ab55-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ab55-129">Authorization</span></span>  | <span data-ttu-id="7ab55-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ab55-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ab55-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="7ab55-132">ConsistencyLevel</span></span> | <span data-ttu-id="7ab55-133">ocorra.</span><span class="sxs-lookup"><span data-stu-id="7ab55-133">eventual.</span></span> <span data-ttu-id="7ab55-134">Esse cabeçalho e `$count` são necessários ao usar os `$search` parâmetros de consulta de conversão de,, `$filter` `$orderby` ou OData.</span><span class="sxs-lookup"><span data-stu-id="7ab55-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="7ab55-135">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="7ab55-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ab55-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ab55-136">Request body</span></span>

<span data-ttu-id="7ab55-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ab55-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ab55-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ab55-138">Response</span></span>

<span data-ttu-id="7ab55-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ab55-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7ab55-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7ab55-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-direct-member-of"></a><span data-ttu-id="7ab55-141">Exemplo 1: obter grupos e unidades administrativas dos quais o grupo é membro direto</span><span class="sxs-lookup"><span data-stu-id="7ab55-141">Example 1: Get groups and administrative units that the group is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="7ab55-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ab55-142">Request</span></span>

<span data-ttu-id="7ab55-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ab55-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ab55-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ab55-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="7ab55-145">C#</span><span class="sxs-lookup"><span data-stu-id="7ab55-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ab55-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ab55-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ab55-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ab55-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7ab55-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ab55-148">Response</span></span>

<span data-ttu-id="7ab55-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ab55-149">The following is an example of the response.</span></span>
><span data-ttu-id="7ab55-150">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7ab55-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7ab55-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ab55-151">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="7ab55-152">Exemplo 2: obter apenas uma contagem de todas as associações</span><span class="sxs-lookup"><span data-stu-id="7ab55-152">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="7ab55-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ab55-153">Request</span></span>

<span data-ttu-id="7ab55-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ab55-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7ab55-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ab55-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="7ab55-156">C#</span><span class="sxs-lookup"><span data-stu-id="7ab55-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ab55-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ab55-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ab55-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ab55-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7ab55-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ab55-159">Response</span></span>

<span data-ttu-id="7ab55-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ab55-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="7ab55-161">394</span><span class="sxs-lookup"><span data-stu-id="7ab55-161">394</span></span>


### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="7ab55-162">Exemplo 3: usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="7ab55-162">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="7ab55-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ab55-163">Request</span></span>

<span data-ttu-id="7ab55-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ab55-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7ab55-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ab55-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="7ab55-166">C#</span><span class="sxs-lookup"><span data-stu-id="7ab55-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-group-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ab55-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ab55-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-group-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ab55-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ab55-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-group-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7ab55-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ab55-169">Response</span></span>

<span data-ttu-id="7ab55-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ab55-170">The following is an example of the response.</span></span>

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

<span data-ttu-id="7ab55-171">394</span><span class="sxs-lookup"><span data-stu-id="7ab55-171">394</span></span>

### <a name="example-4-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="7ab55-172">Exemplo 4: usar a conversão OData e $search para obter associação com nomes de exibição que contenham as letras "vídeo" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="7ab55-172">Example 4: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7ab55-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ab55-173">Request</span></span>

<span data-ttu-id="7ab55-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ab55-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7ab55-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ab55-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="7ab55-176">C#</span><span class="sxs-lookup"><span data-stu-id="7ab55-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-video-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ab55-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ab55-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-video-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ab55-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ab55-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-video-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7ab55-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ab55-179">Response</span></span>

<span data-ttu-id="7ab55-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ab55-180">The following is an example of the response.</span></span>
><span data-ttu-id="7ab55-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ab55-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="7ab55-183">Exemplo 5: usar a conversão OData e $filter para obter associação com um nome de exibição que comece com a letra "A" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="7ab55-183">Example 5: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7ab55-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ab55-184">Request</span></span>

<span data-ttu-id="7ab55-185">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ab55-185">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7ab55-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ab55-186">Response</span></span>

<span data-ttu-id="7ab55-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ab55-187">The following is an example of the response.</span></span>
><span data-ttu-id="7ab55-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ab55-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
