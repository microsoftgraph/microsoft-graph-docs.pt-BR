---
title: Listar aplicativos
description: Obtenha a lista de applications nesta organização.
author: sureshja
localization_priority: Priority
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 0e6ca75c7e1384ffa40f61ebb3976a870cb755a5
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2021
ms.locfileid: "53428847"
---
# <a name="list-applications"></a><span data-ttu-id="8db30-103">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="8db30-103">List applications</span></span>

<span data-ttu-id="8db30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8db30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8db30-105">Obtenha a lista de [applications](../resources/application.md) nesta organização.</span><span class="sxs-lookup"><span data-stu-id="8db30-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

> [!NOTE]
> <span data-ttu-id="8db30-106">Ao chamar essa API usando tokens emitidos para uma conta Microsoft pessoal, ele retornará os aplicativos pertencentes à conta Microsoft pessoal.</span><span class="sxs-lookup"><span data-stu-id="8db30-106">When calling this API using tokens issued for a personal Microsoft account, it will return the apps owned by the personal Microsoft account.</span></span> <span data-ttu-id="8db30-107">A noção de organizações não existe para contas Microsoft pessoais.</span><span class="sxs-lookup"><span data-stu-id="8db30-107">The notion of organizations doesn't exist for personal Microsoft accounts.</span></span> <span data-ttu-id="8db30-108">Para listar os aplicativos pertencentes a contas Microsoft pessoais, essa API exige a permissão User.Read, além de Application.Read.All ou Application.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="8db30-108">In order to list applications owned by specific personal Microsoft accounts, this API requires User.Read permission in addition to Application.Read.All or Application.ReadWrite.All.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="8db30-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="8db30-109">Permissions</span></span>

<span data-ttu-id="8db30-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8db30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8db30-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8db30-112">Permission type</span></span> | <span data-ttu-id="8db30-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8db30-113">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="8db30-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8db30-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8db30-115">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8db30-115">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="8db30-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8db30-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8db30-117">Application.Read.All e User.Read, Application.ReadWrite.All e User.Read</span><span class="sxs-lookup"><span data-stu-id="8db30-117">Application.Read.All and User.Read, Application.ReadWrite.All and User.Read</span></span>  |
| <span data-ttu-id="8db30-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8db30-118">Application</span></span> | <span data-ttu-id="8db30-119">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8db30-119">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8db30-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8db30-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8db30-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8db30-121">Optional query parameters</span></span>

<span data-ttu-id="8db30-122">Este método suporta aos parâmetros de consulta `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, e `$top` [OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8db30-122">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="8db30-123">Algumas consultas são suportadas somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`.</span><span class="sxs-lookup"><span data-stu-id="8db30-123">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="8db30-124">Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8db30-124">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>


## <a name="request-headers"></a><span data-ttu-id="8db30-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8db30-125">Request headers</span></span>

| <span data-ttu-id="8db30-126">Nome</span><span class="sxs-lookup"><span data-stu-id="8db30-126">Name</span></span> | <span data-ttu-id="8db30-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="8db30-127">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="8db30-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="8db30-128">Authorization</span></span>  | <span data-ttu-id="8db30-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8db30-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8db30-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="8db30-131">ConsistencyLevel</span></span> | <span data-ttu-id="8db30-132">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="8db30-132">eventual.</span></span> <span data-ttu-id="8db30-133">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou em uso específico de `$filter`.</span><span class="sxs-lookup"><span data-stu-id="8db30-133">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="8db30-134">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8db30-134">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="8db30-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8db30-135">Request body</span></span>

<span data-ttu-id="8db30-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8db30-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8db30-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8db30-137">Response</span></span>

<span data-ttu-id="8db30-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8db30-138">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8db30-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8db30-139">Examples</span></span>

### <a name="example-1-get-the-list-of-applications"></a><span data-ttu-id="8db30-140">Exemplo 1: obter a lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="8db30-140">Example 1: Get the list of applications</span></span>

#### <a name="request"></a><span data-ttu-id="8db30-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8db30-141">Request</span></span>

<span data-ttu-id="8db30-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8db30-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8db30-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8db30-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications
```
# <a name="c"></a>[<span data-ttu-id="8db30-144">C#</span><span class="sxs-lookup"><span data-stu-id="8db30-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8db30-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8db30-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8db30-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8db30-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8db30-147">Java</span><span class="sxs-lookup"><span data-stu-id="8db30-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8db30-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="8db30-148">Response</span></span>

<span data-ttu-id="8db30-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8db30-149">Here is an example of the response.</span></span>
> <span data-ttu-id="8db30-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8db30-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications",
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

### <a name="example-2-get-only-a-count-of-applications"></a><span data-ttu-id="8db30-151">Exemplo 2: obter apenas uma contagem de aplicativos</span><span class="sxs-lookup"><span data-stu-id="8db30-151">Example 2: Get only a count of applications</span></span>

#### <a name="request"></a><span data-ttu-id="8db30-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8db30-152">Request</span></span>

<span data-ttu-id="8db30-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8db30-153">The following is an example of the request.</span></span> <span data-ttu-id="8db30-154">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$count` está na solicitação.</span><span class="sxs-lookup"><span data-stu-id="8db30-154">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="8db30-155">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8db30-155">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8db30-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="8db30-156">Response</span></span>

<span data-ttu-id="8db30-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8db30-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```


### <a name="example-3-use-filter-and-top-to-get-one-application-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="8db30-158">Exemplo 3: Utilize $filter e $top para obter um aplicativo com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="8db30-158">Example 3: Use $filter and $top to get one application with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8db30-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8db30-159">Request</span></span>

<span data-ttu-id="8db30-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8db30-160">The following is an example of the request.</span></span> <span data-ttu-id="8db30-161">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` e a cadeia de caracteres de consulta `$count=true` porque a solicitação tem os parâmetros de consulta `$orderBy` e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="8db30-161">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="8db30-162">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8db30-162">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8db30-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="8db30-163">Response</span></span>

<span data-ttu-id="8db30-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8db30-164">The following is an example of the response.</span></span>
><span data-ttu-id="8db30-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8db30-165">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
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

### <a name="example-4-use-search-to-get-applications-with-display-names-that-contain-the-letters-web-including-a-count-of-returned-objects"></a><span data-ttu-id="8db30-166">Exemplo 4: Utilize $search para obter aplicativos com nomes de exibição que contenham as letras 'Web', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="8db30-166">Example 4: Use $search to get applications with display names that contain the letters 'Web' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8db30-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8db30-167">Request</span></span>

<span data-ttu-id="8db30-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8db30-168">The following is an example of the request.</span></span> <span data-ttu-id="8db30-169">Essa solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual`, pois a solicitação tem `$search` e a cadeia de caracteres de consulta `$count=true`.</span><span class="sxs-lookup"><span data-stu-id="8db30-169">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` and the `$count=true` query string is in the request.</span></span> <span data-ttu-id="8db30-170">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8db30-170">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_web_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$search="displayName:Web"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8db30-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="8db30-171">Response</span></span>

<span data-ttu-id="8db30-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8db30-172">The following is an example of the response.</span></span>
><span data-ttu-id="8db30-173">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8db30-173">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
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



