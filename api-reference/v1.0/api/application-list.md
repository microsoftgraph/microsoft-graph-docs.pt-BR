---
title: Listar aplicativos
description: Obtenha a lista de applications nesta organização.
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fa6d2eaf1a9480976407d78c75152b8861d82297
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905582"
---
# <a name="list-applications"></a><span data-ttu-id="d464e-103">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="d464e-103">List applications</span></span>

<span data-ttu-id="d464e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d464e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d464e-105">Obtenha a lista de [applications](../resources/application.md) nesta organização.</span><span class="sxs-lookup"><span data-stu-id="d464e-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="d464e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d464e-106">Permissions</span></span>
<span data-ttu-id="d464e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d464e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d464e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d464e-109">Permission type</span></span>      | <span data-ttu-id="d464e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d464e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d464e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d464e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d464e-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d464e-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d464e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d464e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d464e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d464e-114">Not supported.</span></span>    |
|<span data-ttu-id="d464e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d464e-115">Application</span></span> | <span data-ttu-id="d464e-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d464e-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d464e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d464e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d464e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d464e-118">Optional query parameters</span></span>

<span data-ttu-id="d464e-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="d464e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="d464e-120">Você pode usar `$search` nas propriedades **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="d464e-120">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="d464e-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="d464e-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="d464e-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="d464e-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d464e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d464e-123">Request headers</span></span>

| <span data-ttu-id="d464e-124">Nome</span><span class="sxs-lookup"><span data-stu-id="d464e-124">Name</span></span>           | <span data-ttu-id="d464e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d464e-125">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="d464e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d464e-126">Authorization</span></span>  | <span data-ttu-id="d464e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d464e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d464e-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="d464e-129">ConsistencyLevel</span></span> | <span data-ttu-id="d464e-130">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="d464e-130">eventual.</span></span> <span data-ttu-id="d464e-131">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="d464e-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="d464e-132">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="d464e-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d464e-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d464e-133">Request body</span></span>
<span data-ttu-id="d464e-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d464e-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d464e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d464e-135">Response</span></span>

<span data-ttu-id="d464e-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d464e-136">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d464e-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d464e-137">Examples</span></span>

### <a name="example-1-get-the-list-of-applications"></a><span data-ttu-id="d464e-138">Exemplo 1: obter a lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="d464e-138">Example 1: Get the list of applications</span></span>

#### <a name="request"></a><span data-ttu-id="d464e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d464e-139">Request</span></span>

<span data-ttu-id="d464e-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d464e-140">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d464e-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="d464e-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications
```
# <a name="c"></a>[<span data-ttu-id="d464e-142">C#</span><span class="sxs-lookup"><span data-stu-id="d464e-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d464e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d464e-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d464e-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d464e-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d464e-145">Java</span><span class="sxs-lookup"><span data-stu-id="d464e-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d464e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d464e-146">Response</span></span>

<span data-ttu-id="d464e-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d464e-147">Here is an example of the response.</span></span>

> <span data-ttu-id="d464e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d464e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications",
  "value": [
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName": "My app",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-applications"></a><span data-ttu-id="d464e-150">Exemplo 2: obter apenas uma contagem de aplicativos</span><span class="sxs-lookup"><span data-stu-id="d464e-150">Example 2: Get only a count of applications</span></span>

#### <a name="request"></a><span data-ttu-id="d464e-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d464e-151">Request</span></span>

<span data-ttu-id="d464e-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d464e-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d464e-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="d464e-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="d464e-154">C#</span><span class="sxs-lookup"><span data-stu-id="d464e-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d464e-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d464e-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d464e-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d464e-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d464e-157">Java</span><span class="sxs-lookup"><span data-stu-id="d464e-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d464e-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="d464e-158">Response</span></span>

<span data-ttu-id="d464e-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d464e-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-filter-and-top-to-get-one-application-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="d464e-160">Exemplo 3: Utilize $filter e $top para obter um aplicativo com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="d464e-160">Example 3: Use $filter and $top to get one application with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="d464e-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d464e-161">Request</span></span>

<span data-ttu-id="d464e-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d464e-162">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d464e-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="d464e-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="d464e-164">C#</span><span class="sxs-lookup"><span data-stu-id="d464e-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d464e-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d464e-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d464e-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d464e-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d464e-167">Java</span><span class="sxs-lookup"><span data-stu-id="d464e-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d464e-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="d464e-168">Response</span></span>

<span data-ttu-id="d464e-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d464e-169">The following is an example of the response.</span></span>

><span data-ttu-id="d464e-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d464e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#applications",
  "@odata.count":1,
  "value":[
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName":"a",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-applications-with-display-names-that-contain-the-letters-web-including-a-count-of-returned-objects"></a><span data-ttu-id="d464e-172">Exemplo 4: Utilize $search para obter aplicativos com nomes de exibição que contenham as letras 'Web', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="d464e-172">Example 4: Use $search to get applications with display names that contain the letters 'Web' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="d464e-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d464e-173">Request</span></span>

<span data-ttu-id="d464e-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d464e-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d464e-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="d464e-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_web_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications?$search="displayName:Web"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="d464e-176">C#</span><span class="sxs-lookup"><span data-stu-id="d464e-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-web-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d464e-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d464e-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-web-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d464e-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d464e-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-web-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d464e-179">Java</span><span class="sxs-lookup"><span data-stu-id="d464e-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-web-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d464e-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="d464e-180">Response</span></span>

<span data-ttu-id="d464e-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d464e-181">The following is an example of the response.</span></span>

><span data-ttu-id="d464e-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d464e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#applications",
  "@odata.count":1396,
  "value":[
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName":"'DotNetWeb-App' ",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
