---
title: Listar o servicePrincipalName memberOf
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro direto. Essa operação não é transitiva.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 2d36c6b57fc5b73b0faec50d73de67a575aed811
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383109"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="ddf3b-104">Listar o servicePrincipalName memberOf</span><span class="sxs-lookup"><span data-stu-id="ddf3b-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="ddf3b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddf3b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddf3b-106">Obtenha os grupos e funções de diretório dos quais esse [servicePrincipalName](../resources/serviceprincipal.md) é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-106">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of.</span></span> <span data-ttu-id="ddf3b-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddf3b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddf3b-108">Permissions</span></span>

<span data-ttu-id="ddf3b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddf3b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddf3b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddf3b-111">Permission type</span></span>      | <span data-ttu-id="ddf3b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddf3b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddf3b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddf3b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ddf3b-114">Application. Read. All, Directory. Read. All, Application. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="ddf3b-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ddf3b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddf3b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddf3b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-116">Not supported.</span></span>    |
|<span data-ttu-id="ddf3b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddf3b-117">Application</span></span> | <span data-ttu-id="ddf3b-118">Application. Read. All, Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ddf3b-118">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ddf3b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddf3b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddf3b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ddf3b-120">Optional query parameters</span></span>

<span data-ttu-id="ddf3b-121">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search` , `$count` e `$filter` .</span><span class="sxs-lookup"><span data-stu-id="ddf3b-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="ddf3b-122">A conversão OData também é habilitada, por exemplo, você pode transmitir para obter apenas o directoryRoles do usuário é um membro.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="ddf3b-123">Você pode usar `$search` na propriedade **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="ddf3b-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="ddf3b-124">Quando os itens são adicionados ou atualizados para esse recurso, eles são especialmente indexados para uso com os `$count` `$search` parâmetros de consulta e.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="ddf3b-125">Pode haver um ligeiro atraso entre a adição ou atualização de um item e quando ele está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddf3b-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf3b-126">Request headers</span></span>

| <span data-ttu-id="ddf3b-127">Nome</span><span class="sxs-lookup"><span data-stu-id="ddf3b-127">Name</span></span>       | <span data-ttu-id="ddf3b-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddf3b-128">Type</span></span> | <span data-ttu-id="ddf3b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddf3b-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ddf3b-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddf3b-130">Authorization</span></span>  | <span data-ttu-id="ddf3b-131">string</span><span class="sxs-lookup"><span data-stu-id="ddf3b-131">string</span></span>  | <span data-ttu-id="ddf3b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ddf3b-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="ddf3b-134">ConsistencyLevel</span></span> | <span data-ttu-id="ddf3b-135">ocorra.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-135">eventual.</span></span> <span data-ttu-id="ddf3b-136">Esse cabeçalho e `$count` são necessários ao usar os `$search` parâmetros de consulta de conversão de,, `$filter` `$orderby` ou OData.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="ddf3b-137">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddf3b-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf3b-138">Request body</span></span>
<span data-ttu-id="ddf3b-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddf3b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf3b-140">Response</span></span>

<span data-ttu-id="ddf3b-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ddf3b-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ddf3b-142">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-direct-member-of"></a><span data-ttu-id="ddf3b-143">Exemplo 1: obter grupos e funções de diretório de que a entidade de serviço é um membro direto de</span><span class="sxs-lookup"><span data-stu-id="ddf3b-143">Example 1: Get groups and directory roles that the service principal is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="ddf3b-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf3b-144">Request</span></span>

<span data-ttu-id="ddf3b-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ddf3b-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddf3b-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="ddf3b-147">C#</span><span class="sxs-lookup"><span data-stu-id="ddf3b-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddf3b-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddf3b-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddf3b-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddf3b-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddf3b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf3b-150">Response</span></span>

<span data-ttu-id="ddf3b-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-151">The following is an example of the response.</span></span> 
> <span data-ttu-id="ddf3b-152">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-152">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ddf3b-153">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-153">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="ddf3b-154">Exemplo 2: obter apenas uma contagem de todas as associações</span><span class="sxs-lookup"><span data-stu-id="ddf3b-154">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="ddf3b-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf3b-155">Request</span></span>

<span data-ttu-id="ddf3b-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ddf3b-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddf3b-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ddf3b-158">C#</span><span class="sxs-lookup"><span data-stu-id="ddf3b-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddf3b-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddf3b-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddf3b-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddf3b-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddf3b-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf3b-161">Response</span></span>

<span data-ttu-id="ddf3b-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="ddf3b-163">394</span><span class="sxs-lookup"><span data-stu-id="ddf3b-163">394</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="ddf3b-164">Exemplo 3: usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="ddf3b-164">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="ddf3b-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf3b-165">Request</span></span>

<span data-ttu-id="ddf3b-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ddf3b-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddf3b-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="ddf3b-168">C#</span><span class="sxs-lookup"><span data-stu-id="ddf3b-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-group-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddf3b-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddf3b-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-group-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddf3b-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddf3b-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-group-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddf3b-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf3b-171">Response</span></span>

<span data-ttu-id="ddf3b-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-172">The following is an example of the response.</span></span>

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

<span data-ttu-id="ddf3b-173">394</span><span class="sxs-lookup"><span data-stu-id="ddf3b-173">394</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="ddf3b-174">Exemplo 4: Use $search e a conversão OData para obter Associação de grupo com nomes de exibição que contenham as letras "vídeo", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="ddf3b-174">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ddf3b-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf3b-175">Request</span></span>

<span data-ttu-id="ddf3b-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET iv. https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search=”displayName:Video" 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ddf3b-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf3b-177">Response</span></span>

<span data-ttu-id="ddf3b-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-178">The following is an example of the response.</span></span>
><span data-ttu-id="ddf3b-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="ddf3b-181">Exemplo 5: use $filter e a conversão OData para obter a associação de grupo com um nome de exibição que comece com a letra "A", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="ddf3b-181">Example 5: Use $filter and OData cast to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ddf3b-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf3b-182">Request</span></span>

<span data-ttu-id="ddf3b-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ddf3b-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf3b-184">Response</span></span>

<span data-ttu-id="ddf3b-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-185">The following is an example of the response.</span></span>
><span data-ttu-id="ddf3b-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddf3b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
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
