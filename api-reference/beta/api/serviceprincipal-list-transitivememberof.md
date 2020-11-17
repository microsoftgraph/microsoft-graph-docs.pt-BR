---
title: Listar memberOf transitivos de servicePrincipal
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: c463f4393a405a13ee2caeb8570facf33b3d64a8
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082013"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="edd38-103">Listar memberOf transitivos de servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="edd38-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="edd38-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edd38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edd38-p101">Obtenha os grupos e as funções de diretório dos quais essa [servicePrincipal](../resources/serviceprincipal.md) é membro direto. Esta operação é transitiva e incluirá todos os grupos que essa entidade de serviço é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="edd38-p101">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of. This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="edd38-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="edd38-107">Permissions</span></span>
<span data-ttu-id="edd38-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edd38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edd38-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="edd38-110">Permission type</span></span>      | <span data-ttu-id="edd38-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="edd38-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edd38-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="edd38-112">Delegated (work or school account)</span></span> | <span data-ttu-id="edd38-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="edd38-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="edd38-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="edd38-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edd38-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="edd38-115">Not supported.</span></span>    |
|<span data-ttu-id="edd38-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="edd38-116">Application</span></span> | <span data-ttu-id="edd38-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edd38-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="edd38-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="edd38-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="edd38-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="edd38-119">Optional query parameters</span></span>
<span data-ttu-id="edd38-p103">Este método dá suporte aos [parâmetros de consulta OData](/graph/query_parameters)para ajudar a personalizar a resposta, incluindo `$search`, `$count` e `$filter`. A conversão OData também está habilitada, por exemplo, você pode convertê-la para obter apenas o directoryRoles do qual o usuário é membro. Você pode usar `$search` na propriedade **displayName**. Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os parâmetros de consulta `$count` e `$search`. Pode haver um pequeno atraso entre o momento em que um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="edd38-p103">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`. OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="edd38-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="edd38-125">Request headers</span></span>

| <span data-ttu-id="edd38-126">Nome</span><span class="sxs-lookup"><span data-stu-id="edd38-126">Name</span></span>       | <span data-ttu-id="edd38-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="edd38-127">Type</span></span> | <span data-ttu-id="edd38-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="edd38-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="edd38-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="edd38-129">Authorization</span></span>  | <span data-ttu-id="edd38-130">string</span><span class="sxs-lookup"><span data-stu-id="edd38-130">string</span></span>  | <span data-ttu-id="edd38-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edd38-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="edd38-133">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="edd38-133">ConsistencyLevel</span></span> | <span data-ttu-id="edd38-p105">eventual. Esse cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData. Ele usa um índice que pode não estar atualizado com as alterações recentes feitas no objeto.</span><span class="sxs-lookup"><span data-stu-id="edd38-p105">eventual. This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters. It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="edd38-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="edd38-137">Request body</span></span>
<span data-ttu-id="edd38-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="edd38-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edd38-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="edd38-139">Response</span></span>

<span data-ttu-id="edd38-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="edd38-140">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="edd38-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="edd38-141">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-transitive-member-of"></a><span data-ttu-id="edd38-142">Exemplo 1: Obter os grupos e funções de diretório dos quais essa entidade de serviço é membro transitivo</span><span class="sxs-lookup"><span data-stu-id="edd38-142">Example 1: Get groups and directory roles that the service principal is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="edd38-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="edd38-143">Request</span></span>

<span data-ttu-id="edd38-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="edd38-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="edd38-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="edd38-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="edd38-146">C#</span><span class="sxs-lookup"><span data-stu-id="edd38-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-tranitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edd38-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edd38-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-tranitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edd38-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edd38-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-tranitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="edd38-149">Java</span><span class="sxs-lookup"><span data-stu-id="edd38-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-tranitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="edd38-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="edd38-150">Response</span></span>

<span data-ttu-id="edd38-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="edd38-151">The following is an example of the response.</span></span> 
> <span data-ttu-id="edd38-p106">**Observação:** o objeto de resposta mostrado aqui pode ser truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="edd38-p106">**Note:** The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="edd38-154">Exemplo 2: Obter apenas uma contagem de todas as associações transitivas</span><span class="sxs-lookup"><span data-stu-id="edd38-154">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="edd38-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="edd38-155">Request</span></span>

<span data-ttu-id="edd38-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="edd38-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="edd38-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="edd38-157">Response</span></span>

<span data-ttu-id="edd38-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="edd38-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="edd38-159">294</span><span class="sxs-lookup"><span data-stu-id="edd38-159">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="edd38-160">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação transitiva em grupos</span><span class="sxs-lookup"><span data-stu-id="edd38-160">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="edd38-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="edd38-161">Request</span></span>

<span data-ttu-id="edd38-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="edd38-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="edd38-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="edd38-163">Response</span></span>

<span data-ttu-id="edd38-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="edd38-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="edd38-165">294</span><span class="sxs-lookup"><span data-stu-id="edd38-165">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="edd38-166">Exemplo 4: Utilizar $search e conversão OData para obter associação de grupo com nomes de exibição que contenham as letras 'Vídeo', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="edd38-166">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="edd38-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="edd38-167">Request</span></span>

<span data-ttu-id="edd38-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="edd38-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="edd38-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="edd38-169">Response</span></span>

<span data-ttu-id="edd38-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="edd38-170">The following is an example of the response.</span></span>
><span data-ttu-id="edd38-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="edd38-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="edd38-173">Exemplo 5: Usar $filter e conversão OData para obter associação de grupo com um nome de exibição que começa com 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="edd38-173">Example 5: Use $filter and OData cast to get group membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="edd38-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="edd38-174">Request</span></span>

<span data-ttu-id="edd38-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="edd38-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="edd38-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="edd38-176">Response</span></span>

<span data-ttu-id="edd38-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="edd38-177">The following is an example of the response.</span></span>
><span data-ttu-id="edd38-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="edd38-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


