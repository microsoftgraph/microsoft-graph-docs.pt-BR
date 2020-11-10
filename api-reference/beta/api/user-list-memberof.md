---
title: Listar usuário memberOf
description: Obter grupos, funções de diretório e unidades administrativas dos quais o usuário é membro direto. Essa operação não é transitiva.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 6ce35974204f0a4d750c4cfa15b8f3c767bd02b2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979463"
---
# <a name="list-user-memberof"></a><span data-ttu-id="1c15b-104">Listar usuário memberOf</span><span class="sxs-lookup"><span data-stu-id="1c15b-104">List user memberOf</span></span>

<span data-ttu-id="1c15b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c15b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c15b-106">Obter grupos, funções de diretório e unidades administrativas dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="1c15b-106">Get groups, directory roles and administrative units that the user is a direct member of.</span></span> <span data-ttu-id="1c15b-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="1c15b-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c15b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c15b-108">Permissions</span></span>

<span data-ttu-id="1c15b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c15b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c15b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c15b-111">Permission type</span></span> | <span data-ttu-id="1c15b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c15b-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="1c15b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c15b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1c15b-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1c15b-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="1c15b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c15b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c15b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c15b-116">Not supported.</span></span> |
| <span data-ttu-id="1c15b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c15b-117">Application</span></span> | <span data-ttu-id="1c15b-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c15b-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c15b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c15b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c15b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c15b-120">Optional query parameters</span></span>

<span data-ttu-id="1c15b-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="1c15b-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="1c15b-122">A conversão OData também está habilitado, por exemplo, você pode convertê-la para obter apenas o directoryRoles do qual o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="1c15b-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="1c15b-123">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="1c15b-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="1c15b-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="1c15b-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="1c15b-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="1c15b-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c15b-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c15b-126">Request headers</span></span>

| <span data-ttu-id="1c15b-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c15b-127">Header</span></span> | <span data-ttu-id="1c15b-128">Valor</span><span class="sxs-lookup"><span data-stu-id="1c15b-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="1c15b-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c15b-129">Authorization</span></span>  | <span data-ttu-id="1c15b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c15b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c15b-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="1c15b-132">ConsistencyLevel</span></span> | <span data-ttu-id="1c15b-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="1c15b-133">eventual.</span></span> <span data-ttu-id="1c15b-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="1c15b-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="1c15b-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="1c15b-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c15b-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c15b-136">Request body</span></span>

<span data-ttu-id="1c15b-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c15b-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c15b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c15b-138">Response</span></span>

<span data-ttu-id="1c15b-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c15b-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c15b-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1c15b-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="1c15b-141">Exemplo 1: Obter grupos, funções de diretório e unidades administrativas das quais o usuário é membro direto</span><span class="sxs-lookup"><span data-stu-id="1c15b-141">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="1c15b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c15b-142">Request</span></span>

<span data-ttu-id="1c15b-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c15b-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1c15b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c15b-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="1c15b-145">C#</span><span class="sxs-lookup"><span data-stu-id="1c15b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c15b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c15b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c15b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c15b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c15b-148">Java</span><span class="sxs-lookup"><span data-stu-id="1c15b-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1c15b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c15b-149">Response</span></span>

<span data-ttu-id="1c15b-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c15b-150">The following is an example of the response.</span></span>
><span data-ttu-id="1c15b-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c15b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="1c15b-153">Exemplo 2: Obtenha apenas uma contagem de todos os grupos, funções de diretório e unidades administrativas dos quais o usuário é membro direto</span><span class="sxs-lookup"><span data-stu-id="1c15b-153">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="1c15b-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c15b-154">Request</span></span>

<span data-ttu-id="1c15b-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c15b-155">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1c15b-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c15b-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="1c15b-157">C#</span><span class="sxs-lookup"><span data-stu-id="1c15b-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c15b-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c15b-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c15b-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c15b-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c15b-160">Java</span><span class="sxs-lookup"><span data-stu-id="1c15b-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-memberof-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1c15b-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c15b-161">Response</span></span>

<span data-ttu-id="1c15b-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c15b-162">The following is an example of the response.</span></span>
><span data-ttu-id="1c15b-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c15b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="1c15b-165">893</span><span class="sxs-lookup"><span data-stu-id="1c15b-165">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="1c15b-166">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="1c15b-166">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="1c15b-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c15b-167">Request</span></span>

<span data-ttu-id="1c15b-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c15b-168">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1c15b-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c15b-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="1c15b-170">C#</span><span class="sxs-lookup"><span data-stu-id="1c15b-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c15b-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c15b-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c15b-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c15b-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c15b-173">Java</span><span class="sxs-lookup"><span data-stu-id="1c15b-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1c15b-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c15b-174">Response</span></span>

<span data-ttu-id="1c15b-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c15b-175">The following is an example of the response.</span></span>

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

<span data-ttu-id="1c15b-176">294</span><span class="sxs-lookup"><span data-stu-id="1c15b-176">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="1c15b-177">Exemplo 4: Utilize $search e conversão OData para obter associação em grupos com nomes de exibição que contenham as letras 'camada', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="1c15b-177">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1c15b-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c15b-178">Request</span></span>

<span data-ttu-id="1c15b-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c15b-179">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1c15b-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c15b-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="1c15b-181">C#</span><span class="sxs-lookup"><span data-stu-id="1c15b-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c15b-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c15b-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c15b-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c15b-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c15b-184">Java</span><span class="sxs-lookup"><span data-stu-id="1c15b-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1c15b-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c15b-185">Response</span></span>

<span data-ttu-id="1c15b-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c15b-186">The following is an example of the response.</span></span>
><span data-ttu-id="1c15b-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c15b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="1c15b-189">Exemplo 5: Utilize $filter e a conversão OData para obter grupos com um nome de exibição que começa com 'a' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="1c15b-189">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1c15b-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c15b-190">Request</span></span>

<span data-ttu-id="1c15b-191">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c15b-191">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1c15b-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c15b-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="1c15b-193">C#</span><span class="sxs-lookup"><span data-stu-id="1c15b-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c15b-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c15b-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c15b-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c15b-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c15b-196">Java</span><span class="sxs-lookup"><span data-stu-id="1c15b-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1c15b-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c15b-197">Response</span></span>

<span data-ttu-id="1c15b-198">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c15b-198">The following is an example of the response.</span></span>
><span data-ttu-id="1c15b-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c15b-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


