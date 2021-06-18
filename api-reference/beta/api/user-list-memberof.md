---
title: Listar usuário memberOf
description: Obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro direto. Essa operação não é transitiva.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: dc874763490136c62e851585aaba3df9c5be3f13
ms.sourcegitcommit: 2d0daa446c7b37ced1d214e0c6e18e2b8243bb09
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2021
ms.locfileid: "53010224"
---
# <a name="list-user-memberof"></a><span data-ttu-id="4a5fa-104">Listar usuário memberOf</span><span class="sxs-lookup"><span data-stu-id="4a5fa-104">List user memberOf</span></span>

<span data-ttu-id="4a5fa-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a5fa-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a5fa-106">Obtenha os [grupos](../resources/group.md), [funções de diretório](../resources/directoryrole.md) e [unidades administrativas](../resources/administrativeunit.md) das quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-106">Get [groups](../resources/group.md), [directory roles](../resources/directoryrole.md), and [administrative units](../resources/administrativeunit.md) that the user is a direct member of.</span></span> <span data-ttu-id="4a5fa-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a5fa-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a5fa-108">Permissions</span></span>

<span data-ttu-id="4a5fa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a5fa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a5fa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a5fa-111">Permission type</span></span> | <span data-ttu-id="4a5fa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a5fa-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="4a5fa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a5fa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4a5fa-114">GroupMember.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a5fa-114">GroupMember.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="4a5fa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a5fa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a5fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-116">Not supported.</span></span> |
| <span data-ttu-id="4a5fa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a5fa-117">Application</span></span> | <span data-ttu-id="4a5fa-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a5fa-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a5fa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a5fa-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a5fa-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4a5fa-120">Optional query parameters</span></span>

<span data-ttu-id="4a5fa-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="4a5fa-122">A conversão OData também está habilitado, por exemplo, você pode convertê-la para obter apenas o directoryRoles do qual o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="4a5fa-123">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="4a5fa-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="4a5fa-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a5fa-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a5fa-126">Request headers</span></span>

| <span data-ttu-id="4a5fa-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a5fa-127">Header</span></span> | <span data-ttu-id="4a5fa-128">Valor</span><span class="sxs-lookup"><span data-stu-id="4a5fa-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="4a5fa-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a5fa-129">Authorization</span></span>  | <span data-ttu-id="4a5fa-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a5fa-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="4a5fa-132">ConsistencyLevel</span></span> | <span data-ttu-id="4a5fa-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-133">eventual.</span></span> <span data-ttu-id="4a5fa-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="4a5fa-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a5fa-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a5fa-136">Request body</span></span>

<span data-ttu-id="4a5fa-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a5fa-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a5fa-138">Response</span></span>

<span data-ttu-id="4a5fa-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4a5fa-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4a5fa-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="4a5fa-141">Exemplo 1: Obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro direto</span><span class="sxs-lookup"><span data-stu-id="4a5fa-141">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="4a5fa-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a5fa-142">Request</span></span>

<span data-ttu-id="4a5fa-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4a5fa-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a5fa-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="4a5fa-145">C#</span><span class="sxs-lookup"><span data-stu-id="4a5fa-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a5fa-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a5fa-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a5fa-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a5fa-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a5fa-148">Java</span><span class="sxs-lookup"><span data-stu-id="4a5fa-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="4a5fa-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a5fa-149">Response</span></span>

<span data-ttu-id="4a5fa-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-150">The following is an example of the response.</span></span>
><span data-ttu-id="4a5fa-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "displayName": "All Users",
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="4a5fa-152">Exemplo 2: Obtenha apenas uma contagem de todos os grupos, funções de diretório e unidades administrativas dos quais o usuário é membro direto</span><span class="sxs-lookup"><span data-stu-id="4a5fa-152">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="4a5fa-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a5fa-153">Request</span></span>

<span data-ttu-id="4a5fa-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-154">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/$count
ConsistencyLevel: eventual

17
```

#### <a name="response"></a><span data-ttu-id="4a5fa-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a5fa-155">Response</span></span>

<span data-ttu-id="4a5fa-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-156">The following is an example of the response.</span></span>
><span data-ttu-id="4a5fa-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-157">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="4a5fa-158">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="4a5fa-158">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="4a5fa-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a5fa-159">Request</span></span>

<span data-ttu-id="4a5fa-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4a5fa-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a5fa-161">Response</span></span>

<span data-ttu-id="4a5fa-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

16
```

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="4a5fa-163">Exemplo 4: Utilize $search e conversão OData para obter associação em grupos com nomes de exibição que contenham as letras 'camada', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="4a5fa-163">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="4a5fa-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a5fa-164">Request</span></span>

<span data-ttu-id="4a5fa-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4a5fa-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a5fa-166">Response</span></span>

<span data-ttu-id="4a5fa-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-167">The following is an example of the response.</span></span>
><span data-ttu-id="4a5fa-168">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-168">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="4a5fa-169">Exemplo 5: Utilize $filter e a conversão OData para obter grupos com um nome de exibição que começa com 'a' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="4a5fa-169">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="4a5fa-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a5fa-170">Request</span></span>

<span data-ttu-id="4a5fa-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4a5fa-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a5fa-172">Response</span></span>

<span data-ttu-id="4a5fa-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-173">The following is an example of the response.</span></span>
><span data-ttu-id="4a5fa-174">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4a5fa-174">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


