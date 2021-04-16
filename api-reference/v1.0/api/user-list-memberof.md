---
title: Listar memberOf
description: 'Obtenha todos os grupos e funções de diretório dos quais o usuário é um membro direto. '
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: f608c8639556857df1c6065f976378eb7521ccf3
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836924"
---
# <a name="list-memberof"></a><span data-ttu-id="a9591-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="a9591-103">List memberOf</span></span>

<span data-ttu-id="a9591-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9591-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a9591-105">Obtenha os [grupos](../resources/group.md), [funções de diretório](../resources/directoryrole.md) e [unidades administrativas](../resources/administrativeunit.md) das quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="a9591-105">Get [groups](../resources/group.md), [directory roles](../resources/directoryrole.md), and [administrative units](../resources/administrativeunit.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a9591-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9591-106">Permissions</span></span>
<span data-ttu-id="a9591-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9591-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9591-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9591-109">Permission type</span></span>      | <span data-ttu-id="a9591-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9591-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9591-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9591-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a9591-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a9591-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a9591-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9591-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9591-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9591-114">Not supported.</span></span>    |
|<span data-ttu-id="a9591-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9591-115">Application</span></span> | <span data-ttu-id="a9591-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9591-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a9591-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9591-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a9591-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a9591-118">Optional query parameters</span></span>

<span data-ttu-id="a9591-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="a9591-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="a9591-120">A conversão OData também está habilitado, por exemplo, você pode convertê-la para obter apenas o directoryRoles do qual o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="a9591-120">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="a9591-121">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="a9591-121">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="a9591-122">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="a9591-122">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="a9591-123">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="a9591-123">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="a9591-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9591-124">Request headers</span></span>
| <span data-ttu-id="a9591-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9591-125">Header</span></span>       | <span data-ttu-id="a9591-126">Valor</span><span class="sxs-lookup"><span data-stu-id="a9591-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a9591-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9591-127">Authorization</span></span>  | <span data-ttu-id="a9591-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9591-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a9591-130">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="a9591-130">ConsistencyLevel</span></span> | <span data-ttu-id="a9591-131">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="a9591-131">eventual.</span></span> <span data-ttu-id="a9591-132">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="a9591-132">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="a9591-133">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="a9591-133">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9591-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9591-134">Request body</span></span>
<span data-ttu-id="a9591-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9591-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9591-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9591-136">Response</span></span>

<span data-ttu-id="a9591-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9591-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9591-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a9591-138">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="a9591-139">Exemplo 1: Obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro direto</span><span class="sxs-lookup"><span data-stu-id="a9591-139">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="a9591-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9591-140">Request</span></span>

<span data-ttu-id="a9591-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9591-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a9591-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9591-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="a9591-143">C#</span><span class="sxs-lookup"><span data-stu-id="a9591-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9591-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9591-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9591-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9591-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9591-146">Java</span><span class="sxs-lookup"><span data-stu-id="a9591-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a9591-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9591-147">Response</span></span>

<span data-ttu-id="a9591-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9591-148">The following is an example of the response.</span></span>

><span data-ttu-id="a9591-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9591-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="a9591-151">Exemplo 2: Obtenha apenas uma contagem de todos os grupos, funções de diretório e unidades administrativas dos quais o usuário é membro direto</span><span class="sxs-lookup"><span data-stu-id="a9591-151">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="a9591-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9591-152">Request</span></span>

<span data-ttu-id="a9591-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9591-153">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a9591-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9591-154">Response</span></span>

<span data-ttu-id="a9591-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9591-155">The following is an example of the response.</span></span>

><span data-ttu-id="a9591-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9591-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

17
```

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="a9591-158">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="a9591-158">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="a9591-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9591-159">Request</span></span>

<span data-ttu-id="a9591-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9591-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a9591-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9591-161">Response</span></span>

<span data-ttu-id="a9591-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9591-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

16
```

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="a9591-163">Exemplo 4: Utilize $search e conversão OData para obter associação em grupos com nomes de exibição que contenham as letras 'camada', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="a9591-163">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a9591-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9591-164">Request</span></span>

<span data-ttu-id="a9591-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9591-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a9591-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9591-166">Response</span></span>

<span data-ttu-id="a9591-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9591-167">The following is an example of the response.</span></span>

><span data-ttu-id="a9591-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9591-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="a9591-170">Exemplo 5: Utilize $filter e a conversão OData para obter grupos com um nome de exibição que começa com 'a' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="a9591-170">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a9591-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9591-171">Request</span></span>

<span data-ttu-id="a9591-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9591-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a9591-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9591-173">Response</span></span>

<span data-ttu-id="a9591-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9591-174">The following is an example of the response.</span></span>

><span data-ttu-id="a9591-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9591-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
