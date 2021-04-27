---
title: Listar servicePrincipals
description: Recupere uma lista de objetos servicePrincipal.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: cc69bc3eef04ee4bab00f1ebd059b4682ef77b03
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049006"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="10b9e-103">Listar servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="10b9e-103">List servicePrincipals</span></span>

<span data-ttu-id="10b9e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10b9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10b9e-105">Recupere uma lista de objetos [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="10b9e-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="10b9e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="10b9e-106">Permissions</span></span>

<span data-ttu-id="10b9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10b9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10b9e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10b9e-109">Permission type</span></span> | <span data-ttu-id="10b9e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10b9e-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="10b9e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10b9e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="10b9e-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="10b9e-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="10b9e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10b9e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10b9e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10b9e-114">Not supported.</span></span> |
| <span data-ttu-id="10b9e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10b9e-115">Application</span></span> | <span data-ttu-id="10b9e-116">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="10b9e-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10b9e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10b9e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10b9e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="10b9e-118">Optional query parameters</span></span>

<span data-ttu-id="10b9e-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="10b9e-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="10b9e-120">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="10b9e-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="10b9e-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="10b9e-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="10b9e-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="10b9e-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10b9e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10b9e-123">Request headers</span></span>

| <span data-ttu-id="10b9e-124">Nome</span><span class="sxs-lookup"><span data-stu-id="10b9e-124">Name</span></span> | <span data-ttu-id="10b9e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="10b9e-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="10b9e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="10b9e-126">Authorization</span></span> | <span data-ttu-id="10b9e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10b9e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="10b9e-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="10b9e-129">ConsistencyLevel</span></span> | <span data-ttu-id="10b9e-130">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="10b9e-130">eventual.</span></span> <span data-ttu-id="10b9e-131">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="10b9e-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="10b9e-132">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="10b9e-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10b9e-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10b9e-133">Request body</span></span>

<span data-ttu-id="10b9e-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10b9e-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10b9e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="10b9e-135">Response</span></span>

<span data-ttu-id="10b9e-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10b9e-136">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10b9e-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="10b9e-137">Examples</span></span>

### <a name="example-1-get-a-list-of-service-principals"></a><span data-ttu-id="10b9e-138">Exemplo 1: obter uma lista de entidades de serviço</span><span class="sxs-lookup"><span data-stu-id="10b9e-138">Example 1: Get a list of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="10b9e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10b9e-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="10b9e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="10b9e-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals
```
# <a name="c"></a>[<span data-ttu-id="10b9e-141">C#</span><span class="sxs-lookup"><span data-stu-id="10b9e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10b9e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10b9e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10b9e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10b9e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10b9e-144">Java</span><span class="sxs-lookup"><span data-stu-id="10b9e-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="10b9e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="10b9e-145">Response</span></span>

<span data-ttu-id="10b9e-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="10b9e-146">The following is an example of the response.</span></span>
><span data-ttu-id="10b9e-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="10b9e-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-service-principals"></a><span data-ttu-id="10b9e-148">Exemplo 2: obter apenas uma contagem de entidades de serviço</span><span class="sxs-lookup"><span data-stu-id="10b9e-148">Example 2: Get only a count of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="10b9e-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10b9e-149">Request</span></span>

<span data-ttu-id="10b9e-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="10b9e-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="10b9e-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="10b9e-151">Response</span></span>

<span data-ttu-id="10b9e-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="10b9e-152">The following is an example of the response.</span></span>

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

### <a name="example-3-use-filter-and-top-to-get-one-service-principal-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="10b9e-153">Exemplo 3: Utilize $filter e $top para obter uma entidade de serviço com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="10b9e-153">Example 3: Use $filter and $top to get one service principal with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="10b9e-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10b9e-154">Request</span></span>

<span data-ttu-id="10b9e-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="10b9e-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="10b9e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="10b9e-156">Response</span></span>

<span data-ttu-id="10b9e-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="10b9e-157">The following is an example of the response.</span></span>
><span data-ttu-id="10b9e-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="10b9e-158">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-search-to-get-service-principals-with-display-names-that-contain-the-letters-team-including-a-count-of-returned-objects"></a><span data-ttu-id="10b9e-159">Exemplo 4: Utilize $search para obter entidades de serviço com nomes de exibição que contenham as letras 'Team', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="10b9e-159">Example 4: Use $search to get service principals with display names that contain the letters 'Team' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="10b9e-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10b9e-160">Request</span></span>

<span data-ttu-id="10b9e-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="10b9e-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$search="displayName:Team"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="10b9e-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="10b9e-162">Response</span></span>

<span data-ttu-id="10b9e-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="10b9e-163">The following is an example of the response.</span></span>
><span data-ttu-id="10b9e-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="10b9e-164">**Note:** The response object shown here might be shortened for readability.</span></span>

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



