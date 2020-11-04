---
title: Listar memberOf transitivos de servicePrincipal
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 1ef5bc7adf566bb617b3c1fadd3a76f20ca11f38
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905617"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="a72b2-103">Listar memberOf transitivos de servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="a72b2-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="a72b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a72b2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a72b2-105">Obtenha os grupos e funções de diretório dos quais essa [servicePrincipal](../resources/serviceprincipal.md) é membro.</span><span class="sxs-lookup"><span data-stu-id="a72b2-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="a72b2-106">Essa operação é transitiva e incluirá todos os grupos dos quais essa entidade de serviço é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="a72b2-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="a72b2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a72b2-107">Permissions</span></span>
<span data-ttu-id="a72b2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a72b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a72b2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a72b2-110">Permission type</span></span>      | <span data-ttu-id="a72b2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a72b2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a72b2-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a72b2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a72b2-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a72b2-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a72b2-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a72b2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a72b2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a72b2-115">Not supported.</span></span>    |
|<span data-ttu-id="a72b2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a72b2-116">Application</span></span> | <span data-ttu-id="a72b2-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a72b2-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a72b2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a72b2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a72b2-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a72b2-119">Optional query parameters</span></span>

<span data-ttu-id="a72b2-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="a72b2-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="a72b2-121">A conversão OData também está habilitado, por exemplo, você pode convertê-la para obter apenas o directoryRoles do qual o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="a72b2-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="a72b2-122">Você pode usar `$search` nas propriedades **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="a72b2-122">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="a72b2-123">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="a72b2-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="a72b2-124">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="a72b2-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a72b2-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a72b2-125">Request headers</span></span>
| <span data-ttu-id="a72b2-126">Nome</span><span class="sxs-lookup"><span data-stu-id="a72b2-126">Name</span></span>           | <span data-ttu-id="a72b2-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a72b2-127">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="a72b2-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="a72b2-128">Authorization</span></span>  | <span data-ttu-id="a72b2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a72b2-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a72b2-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="a72b2-131">ConsistencyLevel</span></span> | <span data-ttu-id="a72b2-132">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="a72b2-132">eventual.</span></span> <span data-ttu-id="a72b2-133">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="a72b2-133">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="a72b2-134">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="a72b2-134">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a72b2-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a72b2-135">Request body</span></span>
<span data-ttu-id="a72b2-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a72b2-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a72b2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a72b2-137">Response</span></span>

<span data-ttu-id="a72b2-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a72b2-138">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a72b2-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a72b2-139">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-transitive-member-of"></a><span data-ttu-id="a72b2-140">Exemplo 1: Obter os grupos e funções de diretório dos quais essa entidade de serviço é membro transitivo</span><span class="sxs-lookup"><span data-stu-id="a72b2-140">Example 1: Get groups and directory roles that the service principal is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="a72b2-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a72b2-141">Request</span></span>

<span data-ttu-id="a72b2-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a72b2-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a72b2-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="a72b2-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="a72b2-144">C#</span><span class="sxs-lookup"><span data-stu-id="a72b2-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-tranitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a72b2-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a72b2-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-tranitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a72b2-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a72b2-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-tranitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a72b2-147">Java</span><span class="sxs-lookup"><span data-stu-id="a72b2-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-tranitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a72b2-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a72b2-148">Response</span></span>

<span data-ttu-id="a72b2-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a72b2-149">The following is an example of the response.</span></span> 

> <span data-ttu-id="a72b2-150">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a72b2-150">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a72b2-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a72b2-151">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="a72b2-152">Exemplo 2: Obter apenas uma contagem de todas as associações transitivas</span><span class="sxs-lookup"><span data-stu-id="a72b2-152">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="a72b2-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a72b2-153">Request</span></span>

<span data-ttu-id="a72b2-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a72b2-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a72b2-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="a72b2-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="a72b2-156">C#</span><span class="sxs-lookup"><span data-stu-id="a72b2-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a72b2-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a72b2-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a72b2-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a72b2-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a72b2-159">Java</span><span class="sxs-lookup"><span data-stu-id="a72b2-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a72b2-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="a72b2-160">Response</span></span>

<span data-ttu-id="a72b2-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a72b2-161">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="a72b2-162">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação transitiva em grupos</span><span class="sxs-lookup"><span data-stu-id="a72b2-162">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="a72b2-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a72b2-163">Request</span></span>

<span data-ttu-id="a72b2-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a72b2-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a72b2-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="a72b2-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="a72b2-166">C#</span><span class="sxs-lookup"><span data-stu-id="a72b2-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a72b2-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a72b2-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a72b2-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a72b2-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a72b2-169">Java</span><span class="sxs-lookup"><span data-stu-id="a72b2-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a72b2-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="a72b2-170">Response</span></span>

<span data-ttu-id="a72b2-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a72b2-171">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="a72b2-172">Exemplo 4: Utilizar $search e conversão OData para obter associação de grupo com nomes de exibição que contenham as letras 'Vídeo', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="a72b2-172">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a72b2-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a72b2-173">Request</span></span>

<span data-ttu-id="a72b2-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a72b2-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a72b2-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="a72b2-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="a72b2-176">C#</span><span class="sxs-lookup"><span data-stu-id="a72b2-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a72b2-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a72b2-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a72b2-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a72b2-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a72b2-179">Java</span><span class="sxs-lookup"><span data-stu-id="a72b2-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a72b2-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="a72b2-180">Response</span></span>

<span data-ttu-id="a72b2-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a72b2-181">The following is an example of the response.</span></span>

><span data-ttu-id="a72b2-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a72b2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "displayName":"Contoso Videos",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="a72b2-184">Exemplo 5: Usar $filter e conversão OData para obter associação de grupo com um nome de exibição que começa com 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="a72b2-184">Example 5: Use $filter and OData cast to get group membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a72b2-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a72b2-185">Request</span></span>

<span data-ttu-id="a72b2-186">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a72b2-186">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a72b2-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="a72b2-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="a72b2-188">C#</span><span class="sxs-lookup"><span data-stu-id="a72b2-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a72b2-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a72b2-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a72b2-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a72b2-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a72b2-191">Java</span><span class="sxs-lookup"><span data-stu-id="a72b2-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a72b2-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="a72b2-192">Response</span></span>

<span data-ttu-id="a72b2-193">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a72b2-193">The following is an example of the response.</span></span>

><span data-ttu-id="a72b2-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a72b2-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
