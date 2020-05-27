---
title: List servicePrincipals
description: Recupere uma lista de objetos servicePrincipal.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: edbd17d4730ead8e230eb7b3b38a547ac199e922
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44382668"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="1be99-103">List servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="1be99-103">List servicePrincipals</span></span>

<span data-ttu-id="1be99-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1be99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1be99-105">Recupere uma lista de objetos de [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="1be99-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1be99-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1be99-106">Permissions</span></span>

<span data-ttu-id="1be99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1be99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1be99-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1be99-109">Permission type</span></span> | <span data-ttu-id="1be99-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1be99-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="1be99-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1be99-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1be99-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1be99-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="1be99-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1be99-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1be99-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1be99-114">Not supported.</span></span> |
| <span data-ttu-id="1be99-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1be99-115">Application</span></span> | <span data-ttu-id="1be99-116">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1be99-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1be99-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1be99-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1be99-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1be99-118">Optional query parameters</span></span>

<span data-ttu-id="1be99-119">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search` , `$count` e `$filter` .</span><span class="sxs-lookup"><span data-stu-id="1be99-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="1be99-120">Você pode usar `$search` na propriedade **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="1be99-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="1be99-121">Quando os itens são adicionados ou atualizados para esse recurso, eles são especialmente indexados para uso com os `$count` `$search` parâmetros de consulta e.</span><span class="sxs-lookup"><span data-stu-id="1be99-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="1be99-122">Pode haver um ligeiro atraso entre a adição ou atualização de um item e quando ele está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="1be99-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1be99-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1be99-123">Request headers</span></span>

| <span data-ttu-id="1be99-124">Nome</span><span class="sxs-lookup"><span data-stu-id="1be99-124">Name</span></span> | <span data-ttu-id="1be99-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1be99-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="1be99-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1be99-126">Authorization</span></span> | <span data-ttu-id="1be99-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1be99-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1be99-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="1be99-129">ConsistencyLevel</span></span> | <span data-ttu-id="1be99-130">ocorra.</span><span class="sxs-lookup"><span data-stu-id="1be99-130">eventual.</span></span> <span data-ttu-id="1be99-131">Esse cabeçalho e `$count` são necessários ao usar `$search` ou ao usar `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="1be99-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="1be99-132">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="1be99-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1be99-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1be99-133">Request body</span></span>

<span data-ttu-id="1be99-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1be99-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1be99-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1be99-135">Response</span></span>

<span data-ttu-id="1be99-136">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos de [servicePrincipalName](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1be99-136">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1be99-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1be99-137">Examples</span></span>

### <a name="example-1-get-a-list-of-service-principals"></a><span data-ttu-id="1be99-138">Exemplo 1: obter uma lista de entidades de serviço</span><span class="sxs-lookup"><span data-stu-id="1be99-138">Example 1: Get a list of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="1be99-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1be99-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1be99-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="1be99-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/serviceprincipals
```
# <a name="c"></a>[<span data-ttu-id="1be99-141">C#</span><span class="sxs-lookup"><span data-stu-id="1be99-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1be99-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1be99-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1be99-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1be99-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1be99-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="1be99-144">Response</span></span>

<span data-ttu-id="1be99-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1be99-145">The following is an example of the response.</span></span>
><span data-ttu-id="1be99-146">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1be99-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1be99-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1be99-147">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":true,
      "displayName":"amasf",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-service-principals"></a><span data-ttu-id="1be99-148">Exemplo 2: obter apenas uma contagem de entidades de serviço</span><span class="sxs-lookup"><span data-stu-id="1be99-148">Example 2: Get only a count of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="1be99-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1be99-149">Request</span></span>

<span data-ttu-id="1be99-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1be99-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1be99-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="1be99-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="1be99-152">C#</span><span class="sxs-lookup"><span data-stu-id="1be99-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1be99-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1be99-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1be99-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1be99-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1be99-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="1be99-155">Response</span></span>

<span data-ttu-id="1be99-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1be99-156">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="1be99-157">893</span><span class="sxs-lookup"><span data-stu-id="1be99-157">893</span></span>


### <a name="example-3-use-filter-and-top-to-get-one-service-principal-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="1be99-158">Exemplo 3: use $filter e $top para obter uma entidade de serviço com um nome de exibição que comece com ' a ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="1be99-158">Example 3: Use $filter and $top to get one service principal with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1be99-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1be99-159">Request</span></span>

<span data-ttu-id="1be99-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1be99-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1be99-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="1be99-161">Response</span></span>

<span data-ttu-id="1be99-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1be99-162">The following is an example of the response.</span></span>
><span data-ttu-id="1be99-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1be99-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrinciples",
  "@odata.count":1,
  "value":[
    {
      "accountEnabled":true,
      "displayName":"a",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-service-principals-with-display-names-that-contain-the-letters-team-including-a-count-of-returned-objects"></a><span data-ttu-id="1be99-165">Exemplo 4: Use $search para obter entidades de serviço com nomes de exibição que contenham as letras "equipe", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="1be99-165">Example 4: Use $search to get service principals with display names that contain the letters 'Team' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1be99-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1be99-166">Request</span></span>

<span data-ttu-id="1be99-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1be99-167">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1be99-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="1be99-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_team_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$search="displayName:Team"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="1be99-169">C#</span><span class="sxs-lookup"><span data-stu-id="1be99-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1be99-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1be99-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1be99-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1be99-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1be99-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="1be99-172">Response</span></span>

<span data-ttu-id="1be99-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1be99-173">The following is an example of the response.</span></span>
><span data-ttu-id="1be99-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1be99-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrincipals",
  "@odata.count":1396,
  "value":[
    {
      "accountEnabled":true,
      "displayName":"myContosoTeam",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
