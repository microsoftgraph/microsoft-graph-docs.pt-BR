---
title: Listar memberOf de servicePrincipal
description: Obtenha os grupos e as funções de diretório dos quais essa entidade de serviço é membro direto. Esta operação não é transitiva.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 9e34b75872f4a54c99844b67970e4860e2c69393
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082094"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="5d896-104">Listar memberOf de servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="5d896-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="5d896-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d896-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d896-p102">Obtenha os grupos e as funções de diretório dos quais essa [servicePrincipal](../resources/serviceprincipal.md) é membro direto. Esta operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="5d896-p102">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d896-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d896-108">Permissions</span></span>

<span data-ttu-id="5d896-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d896-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d896-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d896-111">Permission type</span></span>      | <span data-ttu-id="5d896-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d896-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d896-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d896-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5d896-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5d896-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5d896-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d896-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d896-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d896-116">Not supported.</span></span>    |
|<span data-ttu-id="5d896-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d896-117">Application</span></span> | <span data-ttu-id="5d896-118">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d896-118">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="5d896-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d896-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5d896-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5d896-120">Optional query parameters</span></span>

<span data-ttu-id="5d896-p104">Este método dá suporte aos [parâmetros de consulta OData](/graph/query_parameters)para ajudar a personalizar a resposta, incluindo `$search`, `$count` e `$filter`. A conversão OData também está habilitada, por exemplo, você pode convertê-la para obter apenas o directoryRoles do qual o usuário é membro. Você pode usar `$search` na propriedade **displayName**. Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os parâmetros de consulta `$count` e `$search`. Pode haver um pequeno atraso entre o momento em que um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="5d896-p104">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`. OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d896-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d896-126">Request headers</span></span>

| <span data-ttu-id="5d896-127">Nome</span><span class="sxs-lookup"><span data-stu-id="5d896-127">Name</span></span>       | <span data-ttu-id="5d896-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d896-128">Type</span></span> | <span data-ttu-id="5d896-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d896-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5d896-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d896-130">Authorization</span></span>  | <span data-ttu-id="5d896-131">string</span><span class="sxs-lookup"><span data-stu-id="5d896-131">string</span></span>  | <span data-ttu-id="5d896-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d896-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d896-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="5d896-134">ConsistencyLevel</span></span> | <span data-ttu-id="5d896-p106">eventual. Esse cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData. Ele usa um índice que pode não estar atualizado com as alterações recentes feitas no objeto.</span><span class="sxs-lookup"><span data-stu-id="5d896-p106">eventual. This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters. It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d896-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d896-138">Request body</span></span>
<span data-ttu-id="5d896-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d896-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d896-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d896-140">Response</span></span>

<span data-ttu-id="5d896-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d896-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5d896-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5d896-142">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-direct-member-of"></a><span data-ttu-id="5d896-143">Exemplo 1: Obter os grupos e funções de diretório dos quais essa entidade de serviço é membro direto</span><span class="sxs-lookup"><span data-stu-id="5d896-143">Example 1: Get groups and directory roles that the service principal is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="5d896-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d896-144">Request</span></span>

<span data-ttu-id="5d896-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d896-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5d896-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d896-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="5d896-147">C#</span><span class="sxs-lookup"><span data-stu-id="5d896-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d896-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d896-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d896-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d896-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d896-150">Java</span><span class="sxs-lookup"><span data-stu-id="5d896-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5d896-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d896-151">Response</span></span>

<span data-ttu-id="5d896-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5d896-152">The following is an example of the response.</span></span> 
> <span data-ttu-id="5d896-p107">**Observação:** o objeto de resposta mostrado aqui pode ser truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d896-p107">**Note:** The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="5d896-155">Exemplo 2: Obter apenas uma contagem de todas as associações</span><span class="sxs-lookup"><span data-stu-id="5d896-155">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="5d896-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d896-156">Request</span></span>

<span data-ttu-id="5d896-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d896-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5d896-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d896-158">Response</span></span>

<span data-ttu-id="5d896-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5d896-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="5d896-160">394</span><span class="sxs-lookup"><span data-stu-id="5d896-160">394</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="5d896-161">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="5d896-161">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="5d896-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d896-162">Request</span></span>

<span data-ttu-id="5d896-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d896-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5d896-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d896-164">Response</span></span>

<span data-ttu-id="5d896-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5d896-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="5d896-166">394</span><span class="sxs-lookup"><span data-stu-id="5d896-166">394</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="5d896-167">Exemplo 4: Utilizar $search e conversão OData para obter associação de grupo com nomes de exibição que contenham as letras 'Vídeo', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="5d896-167">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="5d896-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d896-168">Request</span></span>

<span data-ttu-id="5d896-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d896-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET iv. https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search=”displayName:Video" 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5d896-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d896-170">Response</span></span>

<span data-ttu-id="5d896-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5d896-171">The following is an example of the response.</span></span>
><span data-ttu-id="5d896-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d896-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="5d896-174">Exemplo 5: Usar $filter e conversão OData para obter associação de grupo com um nome de exibição que começa com a letra 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="5d896-174">Example 5: Use $filter and OData cast to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="5d896-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d896-175">Request</span></span>

<span data-ttu-id="5d896-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d896-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5d896-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d896-177">Response</span></span>

<span data-ttu-id="5d896-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5d896-178">The following is an example of the response.</span></span>
><span data-ttu-id="5d896-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d896-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


