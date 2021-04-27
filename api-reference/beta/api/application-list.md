---
title: Listar aplicativos
description: Obtenha a lista de applications nesta organização.
author: sureshja
localization_priority: Priority
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 5d1e3f4927241159fa1e351ea6e08c6427e7ef58
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048103"
---
# <a name="list-applications"></a><span data-ttu-id="cc3b7-103">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="cc3b7-103">List applications</span></span>

<span data-ttu-id="cc3b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc3b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc3b7-105">Obtenha a lista de [applications](../resources/application.md) nesta organização.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

> [!NOTE]
> <span data-ttu-id="cc3b7-106">Ao chamar essa API usando tokens emitidos para uma conta Microsoft pessoal, ele retornará os aplicativos pertencentes à conta Microsoft pessoal.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-106">When calling this API using tokens issued for a personal Microsoft account, it will return the apps owned by the personal Microsoft account.</span></span> <span data-ttu-id="cc3b7-107">A noção de organizações não existe para contas Microsoft pessoais.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-107">The notion of organizations doesn't exist for personal Microsoft accounts.</span></span> <span data-ttu-id="cc3b7-108">Para listar os aplicativos pertencentes a contas Microsoft pessoais, essa API exige a permissão User.Read, além de Application.Read.All ou Application.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-108">In order to list applications owned by specific personal Microsoft accounts, this API requires User.Read permission in addition to Application.Read.All or Application.ReadWrite.All.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="cc3b7-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="cc3b7-109">Permissions</span></span>

<span data-ttu-id="cc3b7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc3b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc3b7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc3b7-112">Permission type</span></span> | <span data-ttu-id="cc3b7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc3b7-113">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="cc3b7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc3b7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cc3b7-115">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cc3b7-115">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="cc3b7-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc3b7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc3b7-117">Application.Read.All e User.Read, Application.ReadWrite.All e User.Read</span><span class="sxs-lookup"><span data-stu-id="cc3b7-117">Application.Read.All and User.Read, Application.ReadWrite.All and User.Read</span></span>  |
| <span data-ttu-id="cc3b7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc3b7-118">Application</span></span> | <span data-ttu-id="cc3b7-119">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc3b7-119">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc3b7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc3b7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cc3b7-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cc3b7-121">Optional query parameters</span></span>

<span data-ttu-id="cc3b7-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="cc3b7-123">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="cc3b7-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="cc3b7-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc3b7-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc3b7-126">Request headers</span></span>

| <span data-ttu-id="cc3b7-127">Nome</span><span class="sxs-lookup"><span data-stu-id="cc3b7-127">Name</span></span> | <span data-ttu-id="cc3b7-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc3b7-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="cc3b7-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc3b7-129">Authorization</span></span>  | <span data-ttu-id="cc3b7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cc3b7-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="cc3b7-132">ConsistencyLevel</span></span> | <span data-ttu-id="cc3b7-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-133">eventual.</span></span> <span data-ttu-id="cc3b7-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-134">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="cc3b7-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-135">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc3b7-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc3b7-136">Request body</span></span>

<span data-ttu-id="cc3b7-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc3b7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc3b7-138">Response</span></span>

<span data-ttu-id="cc3b7-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-139">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc3b7-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cc3b7-140">Examples</span></span>

### <a name="example-1-get-the-list-of-applications"></a><span data-ttu-id="cc3b7-141">Exemplo 1: obter a lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="cc3b7-141">Example 1: Get the list of applications</span></span>

#### <a name="request"></a><span data-ttu-id="cc3b7-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc3b7-142">Request</span></span>

<span data-ttu-id="cc3b7-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cc3b7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc3b7-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications
```
# <a name="c"></a>[<span data-ttu-id="cc3b7-145">C#</span><span class="sxs-lookup"><span data-stu-id="cc3b7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc3b7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc3b7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc3b7-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc3b7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc3b7-148">Java</span><span class="sxs-lookup"><span data-stu-id="cc3b7-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cc3b7-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc3b7-149">Response</span></span>

<span data-ttu-id="cc3b7-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-150">Here is an example of the response.</span></span>
> <span data-ttu-id="cc3b7-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-applications"></a><span data-ttu-id="cc3b7-152">Exemplo 2: obter apenas uma contagem de aplicativos</span><span class="sxs-lookup"><span data-stu-id="cc3b7-152">Example 2: Get only a count of applications</span></span>

#### <a name="request"></a><span data-ttu-id="cc3b7-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc3b7-153">Request</span></span>

<span data-ttu-id="cc3b7-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cc3b7-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc3b7-155">Response</span></span>

<span data-ttu-id="cc3b7-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-156">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="cc3b7-157">893</span><span class="sxs-lookup"><span data-stu-id="cc3b7-157">893</span></span>


### <a name="example-3-use-filter-and-top-to-get-one-application-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="cc3b7-158">Exemplo 3: Utilize $filter e $top para obter um aplicativo com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="cc3b7-158">Example 3: Use $filter and $top to get one application with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cc3b7-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc3b7-159">Request</span></span>

<span data-ttu-id="cc3b7-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cc3b7-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc3b7-161">Response</span></span>

<span data-ttu-id="cc3b7-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-162">The following is an example of the response.</span></span>
><span data-ttu-id="cc3b7-163">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-163">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-search-to-get-applications-with-display-names-that-contain-the-letters-web-including-a-count-of-returned-objects"></a><span data-ttu-id="cc3b7-164">Exemplo 4: Utilize $search para obter aplicativos com nomes de exibição que contenham as letras 'Web', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="cc3b7-164">Example 4: Use $search to get applications with display names that contain the letters 'Web' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cc3b7-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc3b7-165">Request</span></span>

<span data-ttu-id="cc3b7-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_web_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$search="displayName:Web"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cc3b7-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc3b7-167">Response</span></span>

<span data-ttu-id="cc3b7-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-168">The following is an example of the response.</span></span>
><span data-ttu-id="cc3b7-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cc3b7-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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



