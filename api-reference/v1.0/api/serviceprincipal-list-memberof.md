---
title: Listar memberOf de servicePrincipal
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro direto. Essa operação não é transitiva.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 6e03a361d3cd8c52c2c9f69d81ee19ba4d82d9bf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132213"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="3b11d-104">Listar memberOf de servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="3b11d-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="3b11d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b11d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b11d-106">Obtenha os grupos e funções de diretório dos quais essa [servicePrincipal](../resources/serviceprincipal.md) é membro direto.</span><span class="sxs-lookup"><span data-stu-id="3b11d-106">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of.</span></span> <span data-ttu-id="3b11d-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="3b11d-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b11d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b11d-108">Permissions</span></span>

<span data-ttu-id="3b11d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b11d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b11d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b11d-111">Permission type</span></span>      | <span data-ttu-id="3b11d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b11d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b11d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b11d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3b11d-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3b11d-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3b11d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b11d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b11d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b11d-116">Not supported.</span></span>    |
|<span data-ttu-id="3b11d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b11d-117">Application</span></span> | <span data-ttu-id="3b11d-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b11d-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="3b11d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b11d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b11d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3b11d-120">Optional query parameters</span></span>

<span data-ttu-id="3b11d-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="3b11d-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="3b11d-122">A conversão OData também está habilitado, por exemplo, você pode convertê-la para obter apenas o directoryRoles do qual o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="3b11d-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="3b11d-123">Você pode usar `$search` nas propriedades **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="3b11d-123">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="3b11d-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="3b11d-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="3b11d-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="3b11d-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b11d-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b11d-126">Request headers</span></span>
| <span data-ttu-id="3b11d-127">Nome</span><span class="sxs-lookup"><span data-stu-id="3b11d-127">Name</span></span>           | <span data-ttu-id="3b11d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b11d-128">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="3b11d-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b11d-129">Authorization</span></span>  | <span data-ttu-id="3b11d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b11d-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3b11d-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="3b11d-132">ConsistencyLevel</span></span> | <span data-ttu-id="3b11d-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="3b11d-133">eventual.</span></span> <span data-ttu-id="3b11d-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="3b11d-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="3b11d-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="3b11d-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b11d-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b11d-136">Request body</span></span>

<span data-ttu-id="3b11d-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b11d-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b11d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b11d-138">Response</span></span>

<span data-ttu-id="3b11d-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b11d-139">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3b11d-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3b11d-140">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-direct-member-of"></a><span data-ttu-id="3b11d-141">Exemplo 1: Obter os grupos e funções de diretório dos quais essa entidade de serviço é membro direto</span><span class="sxs-lookup"><span data-stu-id="3b11d-141">Example 1: Get groups and directory roles that the service principal is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="3b11d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b11d-142">Request</span></span>

<span data-ttu-id="3b11d-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b11d-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3b11d-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b11d-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="3b11d-145">C#</span><span class="sxs-lookup"><span data-stu-id="3b11d-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b11d-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b11d-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b11d-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b11d-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b11d-148">Java</span><span class="sxs-lookup"><span data-stu-id="3b11d-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3b11d-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b11d-149">Response</span></span>

<span data-ttu-id="3b11d-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b11d-150">The following is an example of the response.</span></span>

> <span data-ttu-id="3b11d-151">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="3b11d-151">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3b11d-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b11d-152">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="3b11d-153">Exemplo 2: Obter apenas uma contagem de todas as associações</span><span class="sxs-lookup"><span data-stu-id="3b11d-153">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="3b11d-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b11d-154">Request</span></span>

<span data-ttu-id="3b11d-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b11d-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3b11d-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b11d-156">Response</span></span>

<span data-ttu-id="3b11d-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b11d-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`394`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="3b11d-158">Exemplo 3: Usar a conversão OData para obter apenas uma contagem de associação de grupo</span><span class="sxs-lookup"><span data-stu-id="3b11d-158">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="3b11d-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b11d-159">Request</span></span>

<span data-ttu-id="3b11d-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b11d-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3b11d-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b11d-161">Response</span></span>

<span data-ttu-id="3b11d-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b11d-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`394`

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="3b11d-163">Exemplo 4: Utilizar $search e conversão OData para obter associação de grupo com nomes de exibição que contenham as letras 'Vídeo', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="3b11d-163">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3b11d-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b11d-164">Request</span></span>

<span data-ttu-id="3b11d-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b11d-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET iv. https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search=”displayName:Video" 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3b11d-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b11d-166">Response</span></span>

<span data-ttu-id="3b11d-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b11d-167">The following is an example of the response.</span></span>

><span data-ttu-id="3b11d-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b11d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="3b11d-170">Exemplo 5: Usar $filter e conversão OData para obter associação de grupo com um nome de exibição que começa com a letra 'A' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="3b11d-170">Example 5: Use $filter and OData cast to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3b11d-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b11d-171">Request</span></span>

<span data-ttu-id="3b11d-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b11d-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3b11d-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b11d-173">Response</span></span>

<span data-ttu-id="3b11d-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b11d-174">The following is an example of the response.</span></span>

><span data-ttu-id="3b11d-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b11d-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
