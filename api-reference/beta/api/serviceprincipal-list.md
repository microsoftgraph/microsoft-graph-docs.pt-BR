---
title: Listar servicePrincipals
description: Recupere uma lista de objetos servicePrincipal.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 595c7e9ee58fc2186fb1f29ccfe5f413cd36b7d5
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430281"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="1cc40-103">Listar servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="1cc40-103">List servicePrincipals</span></span>

<span data-ttu-id="1cc40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cc40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cc40-105">Recupere uma lista de objetos [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="1cc40-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cc40-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cc40-106">Permissions</span></span>

<span data-ttu-id="1cc40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cc40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1cc40-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cc40-109">Permission type</span></span> | <span data-ttu-id="1cc40-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cc40-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="1cc40-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cc40-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1cc40-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1cc40-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="1cc40-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cc40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cc40-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cc40-114">Not supported.</span></span> |
| <span data-ttu-id="1cc40-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cc40-115">Application</span></span> | <span data-ttu-id="1cc40-116">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1cc40-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cc40-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cc40-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1cc40-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1cc40-118">Optional query parameters</span></span>

<span data-ttu-id="1cc40-119">Este método suporta aos parâmetros de consulta `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, e `$top` [OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1cc40-119">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="1cc40-120">Algumas consultas são suportadas somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`.</span><span class="sxs-lookup"><span data-stu-id="1cc40-120">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="1cc40-121">Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="1cc40-121">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1cc40-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc40-122">Request headers</span></span>

| <span data-ttu-id="1cc40-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1cc40-123">Name</span></span> | <span data-ttu-id="1cc40-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cc40-124">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="1cc40-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cc40-125">Authorization</span></span> | <span data-ttu-id="1cc40-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cc40-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1cc40-128">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="1cc40-128">ConsistencyLevel</span></span> | <span data-ttu-id="1cc40-129">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="1cc40-129">eventual.</span></span> <span data-ttu-id="1cc40-130">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou em uso específico de `$filter`.</span><span class="sxs-lookup"><span data-stu-id="1cc40-130">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="1cc40-131">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="1cc40-131">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cc40-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc40-132">Request body</span></span>

<span data-ttu-id="1cc40-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1cc40-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cc40-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc40-134">Response</span></span>

<span data-ttu-id="1cc40-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cc40-135">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1cc40-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1cc40-136">Examples</span></span>

### <a name="example-1-get-a-list-of-service-principals"></a><span data-ttu-id="1cc40-137">Exemplo 1: obter uma lista de entidades de serviço</span><span class="sxs-lookup"><span data-stu-id="1cc40-137">Example 1: Get a list of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="1cc40-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc40-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1cc40-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cc40-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals
```
# <a name="c"></a>[<span data-ttu-id="1cc40-140">C#</span><span class="sxs-lookup"><span data-stu-id="1cc40-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cc40-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cc40-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cc40-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cc40-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1cc40-143">Java</span><span class="sxs-lookup"><span data-stu-id="1cc40-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1cc40-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc40-144">Response</span></span>

<span data-ttu-id="1cc40-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1cc40-145">The following is an example of the response.</span></span>
><span data-ttu-id="1cc40-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1cc40-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-service-principals"></a><span data-ttu-id="1cc40-147">Exemplo 2: obter apenas uma contagem de entidades de serviço</span><span class="sxs-lookup"><span data-stu-id="1cc40-147">Example 2: Get only a count of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="1cc40-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc40-148">Request</span></span>

<span data-ttu-id="1cc40-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cc40-149">The following is an example of the request.</span></span> <span data-ttu-id="1cc40-150">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$count` está na solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cc40-150">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="1cc40-151">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="1cc40-151">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1cc40-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc40-152">Response</span></span>

<span data-ttu-id="1cc40-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1cc40-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-3-use-filter-and-top-to-get-one-service-principal-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="1cc40-154">Exemplo 3: Utilize $filter e $top para obter uma entidade de serviço com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="1cc40-154">Example 3: Use $filter and $top to get one service principal with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1cc40-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc40-155">Request</span></span>

<span data-ttu-id="1cc40-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cc40-156">The following is an example of the request.</span></span> <span data-ttu-id="1cc40-157">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` e a cadeia de caracteres de consulta `$count=true` porque a solicitação tem os parâmetros de consulta `$orderBy` e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="1cc40-157">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="1cc40-158">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="1cc40-158">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1cc40-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc40-159">Response</span></span>

<span data-ttu-id="1cc40-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1cc40-160">The following is an example of the response.</span></span>
><span data-ttu-id="1cc40-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1cc40-161">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-search-to-get-service-principals-with-display-names-that-contain-the-letters-team-including-a-count-of-returned-objects"></a><span data-ttu-id="1cc40-162">Exemplo 4: Utilize $search para obter entidades de serviço com nomes de exibição que contenham as letras 'Team', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="1cc40-162">Example 4: Use $search to get service principals with display names that contain the letters 'Team' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1cc40-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc40-163">Request</span></span>

<span data-ttu-id="1cc40-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cc40-164">The following is an example of the request.</span></span> <span data-ttu-id="1cc40-165">Essa solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$search` e a cadeia de caracteres de consulta `$count=true` está na solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cc40-165">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` and the `$count=true` query string is in the request.</span></span> <span data-ttu-id="1cc40-166">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="1cc40-166">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_team_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$search="displayName:Team"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1cc40-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc40-167">Response</span></span>

<span data-ttu-id="1cc40-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1cc40-168">The following is an example of the response.</span></span>
><span data-ttu-id="1cc40-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1cc40-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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



