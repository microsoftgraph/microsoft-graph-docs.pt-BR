---
title: Listar os memberOf transitivos de servicePrincipalName
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: fa3885224c44294d147fbf0ca15ce23492c4ee1b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336772"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="8001f-103">Listar os memberOf transitivos de servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="8001f-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="8001f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8001f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8001f-105">Obtenha os grupos e funções de diretório dos quais esse [servicePrincipalName](../resources/serviceprincipal.md) é um membro.</span><span class="sxs-lookup"><span data-stu-id="8001f-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="8001f-106">Essa operação é transitiva e inclui todos os grupos dos quais essa entidade de serviço é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="8001f-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="8001f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8001f-107">Permissions</span></span>
<span data-ttu-id="8001f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8001f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8001f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8001f-110">Permission type</span></span>      | <span data-ttu-id="8001f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8001f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8001f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8001f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8001f-113">Application. Read. All, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="8001f-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8001f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8001f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8001f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8001f-115">Not supported.</span></span>    |
|<span data-ttu-id="8001f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8001f-116">Application</span></span> | <span data-ttu-id="8001f-117">Application. Read. All, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8001f-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="8001f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8001f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8001f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8001f-119">Optional query parameters</span></span>
<span data-ttu-id="8001f-120">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search` , `$count` e `$filter` .</span><span class="sxs-lookup"><span data-stu-id="8001f-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="8001f-121">A conversão OData também é habilitada, por exemplo, você pode transmitir para obter apenas o directoryRoles do usuário é um membro.</span><span class="sxs-lookup"><span data-stu-id="8001f-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="8001f-122">Você pode usar `$search` na propriedade **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="8001f-122">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="8001f-123">Quando os itens são adicionados ou atualizados para esse recurso, eles são especialmente indexados para uso com os `$count` `$search` parâmetros de consulta e.</span><span class="sxs-lookup"><span data-stu-id="8001f-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="8001f-124">Pode haver um ligeiro atraso entre a adição ou atualização de um item e quando ele está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="8001f-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8001f-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8001f-125">Request headers</span></span>

| <span data-ttu-id="8001f-126">Nome</span><span class="sxs-lookup"><span data-stu-id="8001f-126">Name</span></span>       | <span data-ttu-id="8001f-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8001f-127">Type</span></span> | <span data-ttu-id="8001f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8001f-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8001f-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="8001f-129">Authorization</span></span>  | <span data-ttu-id="8001f-130">string</span><span class="sxs-lookup"><span data-stu-id="8001f-130">string</span></span>  | <span data-ttu-id="8001f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8001f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8001f-133">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="8001f-133">ConsistencyLevel</span></span> | <span data-ttu-id="8001f-134">ocorra.</span><span class="sxs-lookup"><span data-stu-id="8001f-134">eventual.</span></span> <span data-ttu-id="8001f-135">Esse cabeçalho e `$count` são necessários ao usar os `$search` parâmetros de consulta de conversão de,, `$filter` `$orderby` ou OData.</span><span class="sxs-lookup"><span data-stu-id="8001f-135">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="8001f-136">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="8001f-136">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8001f-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8001f-137">Request body</span></span>
<span data-ttu-id="8001f-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8001f-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8001f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8001f-139">Response</span></span>

<span data-ttu-id="8001f-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8001f-140">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8001f-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8001f-141">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-transitive-member-of"></a><span data-ttu-id="8001f-142">Exemplo 1: obter grupos e funções de diretório de que a entidade de serviço é um membro transitiva de</span><span class="sxs-lookup"><span data-stu-id="8001f-142">Example 1: Get groups and directory roles that the service principal is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="8001f-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8001f-143">Request</span></span>

<span data-ttu-id="8001f-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8001f-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8001f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="8001f-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="8001f-146">C#</span><span class="sxs-lookup"><span data-stu-id="8001f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-tranitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8001f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8001f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-tranitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8001f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8001f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-tranitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8001f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="8001f-149">Response</span></span>

<span data-ttu-id="8001f-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8001f-150">The following is an example of the response.</span></span> 
> <span data-ttu-id="8001f-151">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="8001f-151">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8001f-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8001f-152">All of the properties will be returned from an actual call.</span></span>

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
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="8001f-153">Exemplo 2: obter apenas uma contagem de todas as associações transitivas</span><span class="sxs-lookup"><span data-stu-id="8001f-153">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="8001f-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8001f-154">Request</span></span>

<span data-ttu-id="8001f-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8001f-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8001f-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="8001f-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="8001f-157">C#</span><span class="sxs-lookup"><span data-stu-id="8001f-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8001f-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8001f-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8001f-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8001f-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8001f-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="8001f-160">Response</span></span>

<span data-ttu-id="8001f-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8001f-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="8001f-162">294</span><span class="sxs-lookup"><span data-stu-id="8001f-162">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="8001f-163">Exemplo 3: usar a conversão OData para obter apenas uma contagem de associação transitiva em grupos</span><span class="sxs-lookup"><span data-stu-id="8001f-163">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="8001f-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8001f-164">Request</span></span>

<span data-ttu-id="8001f-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8001f-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8001f-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="8001f-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="8001f-167">C#</span><span class="sxs-lookup"><span data-stu-id="8001f-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8001f-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8001f-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8001f-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8001f-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8001f-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="8001f-170">Response</span></span>

<span data-ttu-id="8001f-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8001f-171">The following is an example of the response.</span></span>

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

<span data-ttu-id="8001f-172">294</span><span class="sxs-lookup"><span data-stu-id="8001f-172">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="8001f-173">Exemplo 4: Use $search e a conversão OData para obter Associação de grupo com nomes de exibição que contenham as letras "vídeo", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="8001f-173">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8001f-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8001f-174">Request</span></span>

<span data-ttu-id="8001f-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8001f-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8001f-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="8001f-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="8001f-177">C#</span><span class="sxs-lookup"><span data-stu-id="8001f-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8001f-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8001f-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8001f-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8001f-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8001f-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="8001f-180">Response</span></span>

<span data-ttu-id="8001f-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8001f-181">The following is an example of the response.</span></span>
><span data-ttu-id="8001f-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8001f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "displayName":"Contoso Videos",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="8001f-184">Exemplo 5: use $filter e a conversão OData para obter a associação de grupo com um nome de exibição que comece com ' A ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="8001f-184">Example 5: Use $filter and OData cast to get group membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8001f-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8001f-185">Request</span></span>

<span data-ttu-id="8001f-186">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8001f-186">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8001f-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="8001f-187">Response</span></span>

<span data-ttu-id="8001f-188">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8001f-188">The following is an example of the response.</span></span>
><span data-ttu-id="8001f-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8001f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List servicePrincipal transitiveMemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
