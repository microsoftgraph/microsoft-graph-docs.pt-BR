---
title: Listar memberOf
description: 'Obtenha grupos dos quais um grupo é um membro direto. '
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5709c1470fdd54647785d236325236dcc7803168
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048719"
---
# <a name="list-memberof"></a><span data-ttu-id="64a24-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="64a24-103">List memberOf</span></span>

<span data-ttu-id="64a24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64a24-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64a24-105">Obtenha grupos dos quais um grupo é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="64a24-105">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="64a24-p101">Essa operação não é transitiva. Ao contrário de obter Grupos do Microsoft 365 de um usuário, retorna todos os tipos de grupos, não apenas grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="64a24-p101">This operation is not transitive. Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="64a24-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="64a24-108">Permissions</span></span>
<span data-ttu-id="64a24-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64a24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64a24-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64a24-111">Permission type</span></span>      | <span data-ttu-id="64a24-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64a24-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64a24-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64a24-113">Delegated (work or school account)</span></span> | <span data-ttu-id="64a24-114">GroupMember.Read.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="64a24-114">GroupMember.Read.All, Group.Read.All</span></span>    |
|<span data-ttu-id="64a24-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64a24-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64a24-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64a24-116">Not supported.</span></span>    |
|<span data-ttu-id="64a24-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64a24-117">Application</span></span> | <span data-ttu-id="64a24-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="64a24-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="64a24-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64a24-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64a24-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="64a24-120">Optional query parameters</span></span>

<span data-ttu-id="64a24-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="64a24-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="64a24-122">A conversão OData também está habilitada, por exemplo, você pode lançar para obter apenas os grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="64a24-122">OData cast is also enabled, for example, you can cast to get just the groups the group is a member of.</span></span> <span data-ttu-id="64a24-123">Você pode usar `$search` nas propriedades **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="64a24-123">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="64a24-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="64a24-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="64a24-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="64a24-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64a24-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64a24-126">Request headers</span></span>

| <span data-ttu-id="64a24-127">Nome</span><span class="sxs-lookup"><span data-stu-id="64a24-127">Name</span></span> | <span data-ttu-id="64a24-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="64a24-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="64a24-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="64a24-129">Authorization</span></span>  | <span data-ttu-id="64a24-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64a24-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64a24-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="64a24-132">ConsistencyLevel</span></span> | <span data-ttu-id="64a24-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="64a24-133">eventual.</span></span> <span data-ttu-id="64a24-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="64a24-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="64a24-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="64a24-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64a24-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64a24-136">Request body</span></span>
<span data-ttu-id="64a24-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64a24-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64a24-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="64a24-138">Response</span></span>
<span data-ttu-id="64a24-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64a24-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64a24-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="64a24-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-direct-member-of"></a><span data-ttu-id="64a24-141">Exemplo 1: Obter grupos e unidades administrativas das quais o grupo é membro direto</span><span class="sxs-lookup"><span data-stu-id="64a24-141">Example 1: Get groups and administrative units that the group is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="64a24-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64a24-142">Request</span></span>

<span data-ttu-id="64a24-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64a24-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64a24-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="64a24-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="64a24-145">C#</span><span class="sxs-lookup"><span data-stu-id="64a24-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64a24-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64a24-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64a24-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64a24-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64a24-148">Java</span><span class="sxs-lookup"><span data-stu-id="64a24-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="64a24-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="64a24-149">Response</span></span>

<span data-ttu-id="64a24-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64a24-150">The following is an example of the response.</span></span>

><span data-ttu-id="64a24-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="64a24-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="64a24-152">Exemplo 2: Obter apenas uma contagem de todas as associações</span><span class="sxs-lookup"><span data-stu-id="64a24-152">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="64a24-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64a24-153">Request</span></span>

<span data-ttu-id="64a24-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64a24-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="64a24-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="64a24-155">Response</span></span>

<span data-ttu-id="64a24-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64a24-156">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`394`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="64a24-157">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="64a24-157">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="64a24-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64a24-158">Request</span></span>

<span data-ttu-id="64a24-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64a24-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="64a24-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="64a24-160">Response</span></span>

<span data-ttu-id="64a24-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64a24-161">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`394`

### <a name="example-4-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="64a24-162">Exemplo 4: Utilize a conversão OData e $search para obter associação com nomes de exibição que contenham as letras 'Vídeo', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="64a24-162">Example 4: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="64a24-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64a24-163">Request</span></span>

<span data-ttu-id="64a24-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64a24-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="64a24-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="64a24-165">Response</span></span>

<span data-ttu-id="64a24-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64a24-166">The following is an example of the response.</span></span>

><span data-ttu-id="64a24-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="64a24-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="64a24-168">Exemplo 5: Utilize a conversão OData e $filter para obter associação com um nome de exibição que começa com a letra 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="64a24-168">Example 5: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="64a24-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64a24-169">Request</span></span>

<span data-ttu-id="64a24-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64a24-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="64a24-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="64a24-171">Response</span></span>

<span data-ttu-id="64a24-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64a24-172">The following is an example of the response.</span></span>

><span data-ttu-id="64a24-173">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="64a24-173">**Note:** The response object shown here might be shortened for readability.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
