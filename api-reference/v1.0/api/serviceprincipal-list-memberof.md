---
title: Listar memberOf de servicePrincipal
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro direto. Essa operação não é transitiva.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: ce371ee9554ed5b217ea768ebb7709d52921f8d6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054431"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="b5a1a-104">Listar memberOf de servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="b5a1a-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="b5a1a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5a1a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5a1a-106">Obtenha os grupos e funções de diretório dos quais essa [servicePrincipal](../resources/serviceprincipal.md) é membro direto.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-106">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of.</span></span> <span data-ttu-id="b5a1a-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5a1a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5a1a-108">Permissions</span></span>

<span data-ttu-id="b5a1a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5a1a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5a1a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5a1a-111">Permission type</span></span>      | <span data-ttu-id="b5a1a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5a1a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5a1a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5a1a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b5a1a-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b5a1a-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b5a1a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5a1a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5a1a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-116">Not supported.</span></span>    |
|<span data-ttu-id="b5a1a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5a1a-117">Application</span></span> | <span data-ttu-id="b5a1a-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5a1a-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="b5a1a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5a1a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5a1a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b5a1a-120">Optional query parameters</span></span>

<span data-ttu-id="b5a1a-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="b5a1a-122">A conversão OData também está habilitado, por exemplo, você pode convertê-la para obter apenas o directoryRoles do qual o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="b5a1a-123">Você pode usar `$search` nas propriedades **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-123">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="b5a1a-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="b5a1a-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5a1a-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5a1a-126">Request headers</span></span>
| <span data-ttu-id="b5a1a-127">Nome</span><span class="sxs-lookup"><span data-stu-id="b5a1a-127">Name</span></span>           | <span data-ttu-id="b5a1a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5a1a-128">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="b5a1a-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5a1a-129">Authorization</span></span>  | <span data-ttu-id="b5a1a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b5a1a-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="b5a1a-132">ConsistencyLevel</span></span> | <span data-ttu-id="b5a1a-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-133">eventual.</span></span> <span data-ttu-id="b5a1a-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="b5a1a-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5a1a-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5a1a-136">Request body</span></span>

<span data-ttu-id="b5a1a-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5a1a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5a1a-138">Response</span></span>

<span data-ttu-id="b5a1a-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-139">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5a1a-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b5a1a-140">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-direct-member-of"></a><span data-ttu-id="b5a1a-141">Exemplo 1: Obter os grupos e funções de diretório dos quais essa entidade de serviço é membro direto</span><span class="sxs-lookup"><span data-stu-id="b5a1a-141">Example 1: Get groups and directory roles that the service principal is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="b5a1a-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5a1a-142">Request</span></span>

<span data-ttu-id="b5a1a-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5a1a-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5a1a-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="b5a1a-145">C#</span><span class="sxs-lookup"><span data-stu-id="b5a1a-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5a1a-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5a1a-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5a1a-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5a1a-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5a1a-148">Java</span><span class="sxs-lookup"><span data-stu-id="b5a1a-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b5a1a-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5a1a-149">Response</span></span>

<span data-ttu-id="b5a1a-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-150">The following is an example of the response.</span></span>

> <span data-ttu-id="b5a1a-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="b5a1a-152">Exemplo 2: Obter apenas uma contagem de todas as associações</span><span class="sxs-lookup"><span data-stu-id="b5a1a-152">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="b5a1a-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5a1a-153">Request</span></span>

<span data-ttu-id="b5a1a-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b5a1a-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5a1a-155">Response</span></span>

<span data-ttu-id="b5a1a-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-156">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

394
```

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="b5a1a-157">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="b5a1a-157">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="b5a1a-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5a1a-158">Request</span></span>

<span data-ttu-id="b5a1a-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b5a1a-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5a1a-160">Response</span></span>

<span data-ttu-id="b5a1a-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-161">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

394
```

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="b5a1a-162">Exemplo 4: Utilizar $search e conversão OData para obter associação de grupo com nomes de exibição que contenham as letras 'Vídeo', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="b5a1a-162">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b5a1a-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5a1a-163">Request</span></span>

<span data-ttu-id="b5a1a-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search=”displayName:Video" 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b5a1a-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5a1a-165">Response</span></span>

<span data-ttu-id="b5a1a-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-166">The following is an example of the response.</span></span>

><span data-ttu-id="b5a1a-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
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

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="b5a1a-168">Exemplo 5: Usar $filter e conversão OData para obter associação de grupo com um nome de exibição que começa com a letra 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="b5a1a-168">Example 5: Use $filter and OData cast to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b5a1a-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5a1a-169">Request</span></span>

<span data-ttu-id="b5a1a-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b5a1a-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5a1a-171">Response</span></span>

<span data-ttu-id="b5a1a-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-172">The following is an example of the response.</span></span>

><span data-ttu-id="b5a1a-173">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b5a1a-173">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
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
