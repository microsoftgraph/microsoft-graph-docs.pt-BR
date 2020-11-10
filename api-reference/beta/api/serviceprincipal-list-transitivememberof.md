---
title: Listar memberOf transitivos de servicePrincipal
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 314d36c467fc5215706cbeb763353c6e03acd154
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973647"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="81108-103">Listar memberOf transitivos de servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="81108-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="81108-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81108-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81108-105">Obtenha os grupos e funções de diretório dos quais essa [servicePrincipal](../resources/serviceprincipal.md) é membro.</span><span class="sxs-lookup"><span data-stu-id="81108-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="81108-106">Essa operação é transitiva e incluirá todos os grupos dos quais essa entidade de serviço é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="81108-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="81108-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="81108-107">Permissions</span></span>
<span data-ttu-id="81108-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81108-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81108-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81108-110">Permission type</span></span>      | <span data-ttu-id="81108-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81108-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81108-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81108-112">Delegated (work or school account)</span></span> | <span data-ttu-id="81108-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81108-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="81108-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81108-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81108-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81108-115">Not supported.</span></span>    |
|<span data-ttu-id="81108-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81108-116">Application</span></span> | <span data-ttu-id="81108-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81108-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="81108-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81108-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="81108-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="81108-119">Optional query parameters</span></span>
<span data-ttu-id="81108-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="81108-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="81108-121">A conversão OData também está habilitado, por exemplo, você pode convertê-la para obter apenas o directoryRoles do qual o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="81108-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="81108-122">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="81108-122">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="81108-123">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="81108-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="81108-124">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="81108-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81108-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81108-125">Request headers</span></span>

| <span data-ttu-id="81108-126">Nome</span><span class="sxs-lookup"><span data-stu-id="81108-126">Name</span></span>       | <span data-ttu-id="81108-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="81108-127">Type</span></span> | <span data-ttu-id="81108-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="81108-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="81108-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="81108-129">Authorization</span></span>  | <span data-ttu-id="81108-130">string</span><span class="sxs-lookup"><span data-stu-id="81108-130">string</span></span>  | <span data-ttu-id="81108-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81108-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81108-133">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="81108-133">ConsistencyLevel</span></span> | <span data-ttu-id="81108-134">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="81108-134">eventual.</span></span> <span data-ttu-id="81108-135">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="81108-135">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="81108-136">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="81108-136">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81108-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81108-137">Request body</span></span>
<span data-ttu-id="81108-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81108-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81108-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="81108-139">Response</span></span>

<span data-ttu-id="81108-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81108-140">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81108-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="81108-141">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-transitive-member-of"></a><span data-ttu-id="81108-142">Exemplo 1: Obter os grupos e funções de diretório dos quais essa entidade de serviço é membro transitivo</span><span class="sxs-lookup"><span data-stu-id="81108-142">Example 1: Get groups and directory roles that the service principal is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="81108-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81108-143">Request</span></span>

<span data-ttu-id="81108-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81108-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="81108-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="81108-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="81108-146">C#</span><span class="sxs-lookup"><span data-stu-id="81108-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-tranitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81108-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81108-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-tranitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81108-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81108-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-tranitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81108-149">Java</span><span class="sxs-lookup"><span data-stu-id="81108-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-tranitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="81108-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="81108-150">Response</span></span>

<span data-ttu-id="81108-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81108-151">The following is an example of the response.</span></span> 
> <span data-ttu-id="81108-152">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="81108-152">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="81108-153">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81108-153">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="81108-154">Exemplo 2: Obter apenas uma contagem de todas as associações transitivas</span><span class="sxs-lookup"><span data-stu-id="81108-154">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="81108-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81108-155">Request</span></span>

<span data-ttu-id="81108-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81108-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="81108-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="81108-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="81108-158">C#</span><span class="sxs-lookup"><span data-stu-id="81108-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81108-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81108-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81108-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81108-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81108-161">Java</span><span class="sxs-lookup"><span data-stu-id="81108-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="81108-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="81108-162">Response</span></span>

<span data-ttu-id="81108-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81108-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="81108-164">294</span><span class="sxs-lookup"><span data-stu-id="81108-164">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="81108-165">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação transitiva em grupos</span><span class="sxs-lookup"><span data-stu-id="81108-165">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="81108-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81108-166">Request</span></span>

<span data-ttu-id="81108-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81108-167">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="81108-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="81108-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="81108-169">C#</span><span class="sxs-lookup"><span data-stu-id="81108-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81108-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81108-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81108-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81108-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81108-172">Java</span><span class="sxs-lookup"><span data-stu-id="81108-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="81108-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="81108-173">Response</span></span>

<span data-ttu-id="81108-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81108-174">The following is an example of the response.</span></span>

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

<span data-ttu-id="81108-175">294</span><span class="sxs-lookup"><span data-stu-id="81108-175">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="81108-176">Exemplo 4: Utilizar $search e conversão OData para obter associação de grupo com nomes de exibição que contenham as letras 'Vídeo', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="81108-176">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="81108-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81108-177">Request</span></span>

<span data-ttu-id="81108-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81108-178">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="81108-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="81108-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="81108-180">C#</span><span class="sxs-lookup"><span data-stu-id="81108-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81108-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81108-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81108-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81108-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81108-183">Java</span><span class="sxs-lookup"><span data-stu-id="81108-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="81108-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="81108-184">Response</span></span>

<span data-ttu-id="81108-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81108-185">The following is an example of the response.</span></span>
><span data-ttu-id="81108-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81108-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="81108-188">Exemplo 5: Usar $filter e conversão OData para obter associação de grupo com um nome de exibição que começa com 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="81108-188">Example 5: Use $filter and OData cast to get group membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="81108-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81108-189">Request</span></span>

<span data-ttu-id="81108-190">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81108-190">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="81108-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="81108-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="81108-192">C#</span><span class="sxs-lookup"><span data-stu-id="81108-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81108-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81108-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81108-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81108-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81108-195">Java</span><span class="sxs-lookup"><span data-stu-id="81108-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="81108-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="81108-196">Response</span></span>

<span data-ttu-id="81108-197">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81108-197">The following is an example of the response.</span></span>
><span data-ttu-id="81108-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81108-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


