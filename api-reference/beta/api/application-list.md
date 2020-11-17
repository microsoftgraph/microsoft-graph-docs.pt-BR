---
title: Listar aplicativos
description: Obtenha a lista de applications nesta organização.
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e94927d7c84e376488873f261f06710e53a84b33
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2020
ms.locfileid: "49081891"
---
# <a name="list-applications"></a><span data-ttu-id="3aa6b-103">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="3aa6b-103">List applications</span></span>

<span data-ttu-id="3aa6b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aa6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3aa6b-105">Obtenha a lista de [aplicativos](../resources/application.md) nesta organização.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

> [!NOTE]
> <span data-ttu-id="3aa6b-p101">Ao chamar essa API usando tokens emitidos para uma conta pessoal da Microsoft, ela retornará os aplicativos pertencentes à conta pessoal da Microsoft. A noção de organizações não existe para contas pessoais da Microsoft. Para listar os aplicativos pertencentes a contas pessoais da Microsoft, essa API exige a permissão User.Read, além de Application.Read.All ou Application.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-p101">When calling this API using tokens issued for a personal Microsoft account, it will return the apps owned by the personal Microsoft account. The notion of organizations doesn't exist for personal Microsoft accounts. In order to list applications owned by specific personal Microsoft accounts, this API requires User.Read permission in addition to Application.Read.All or Application.ReadWrite.All.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="3aa6b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="3aa6b-109">Permissions</span></span>

<span data-ttu-id="3aa6b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aa6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3aa6b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3aa6b-112">Permission type</span></span> | <span data-ttu-id="3aa6b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3aa6b-113">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="3aa6b-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3aa6b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3aa6b-115">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3aa6b-115">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="3aa6b-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3aa6b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aa6b-117">Application.Read.All e User.Read, Application.ReadWrite.All e User.Read</span><span class="sxs-lookup"><span data-stu-id="3aa6b-117">Application.Read.All and User.Read, Application.ReadWrite.All and User.Read</span></span>  |
| <span data-ttu-id="3aa6b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3aa6b-118">Application</span></span> | <span data-ttu-id="3aa6b-119">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3aa6b-119">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3aa6b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3aa6b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3aa6b-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3aa6b-121">Optional query parameters</span></span>

<span data-ttu-id="3aa6b-p103">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count` e `$filter`. Você pode usar `$search` na propriedade **displayName**. Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os parâmetros de consulta `$count` e `$search`. Pode haver um pequeno atraso entre o momento em que um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-p103">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3aa6b-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3aa6b-126">Request headers</span></span>

| <span data-ttu-id="3aa6b-127">Nome</span><span class="sxs-lookup"><span data-stu-id="3aa6b-127">Name</span></span> | <span data-ttu-id="3aa6b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aa6b-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="3aa6b-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="3aa6b-129">Authorization</span></span>  | <span data-ttu-id="3aa6b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3aa6b-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="3aa6b-132">ConsistencyLevel</span></span> | <span data-ttu-id="3aa6b-p105">eventual. Esse cabeçalho e `$count` são necessários ao usar `$search` ou ao usar `$filter` com o parâmetro de consulta `$orderby`. Ele usa um índice que pode não estar atualizado com as alterações recentes feitas no objeto.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-p105">eventual. This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter. It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3aa6b-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3aa6b-136">Request body</span></span>

<span data-ttu-id="3aa6b-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3aa6b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aa6b-138">Response</span></span>

<span data-ttu-id="3aa6b-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-139">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3aa6b-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3aa6b-140">Examples</span></span>

### <a name="example-1-get-the-list-of-applications"></a><span data-ttu-id="3aa6b-141">Exemplo 1: obter a lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="3aa6b-141">Example 1: Get the list of applications</span></span>

#### <a name="request"></a><span data-ttu-id="3aa6b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3aa6b-142">Request</span></span>

<span data-ttu-id="3aa6b-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3aa6b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aa6b-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications
```
# <a name="c"></a>[<span data-ttu-id="3aa6b-145">C#</span><span class="sxs-lookup"><span data-stu-id="3aa6b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3aa6b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3aa6b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3aa6b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3aa6b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3aa6b-148">Java</span><span class="sxs-lookup"><span data-stu-id="3aa6b-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3aa6b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aa6b-149">Response</span></span>

<span data-ttu-id="3aa6b-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-150">Here is an example of the response.</span></span>
> <span data-ttu-id="3aa6b-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-applications"></a><span data-ttu-id="3aa6b-153">Exemplo 2: obter apenas uma contagem de aplicativos</span><span class="sxs-lookup"><span data-stu-id="3aa6b-153">Example 2: Get only a count of applications</span></span>

#### <a name="request"></a><span data-ttu-id="3aa6b-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3aa6b-154">Request</span></span>

<span data-ttu-id="3aa6b-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3aa6b-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aa6b-156">Response</span></span>

<span data-ttu-id="3aa6b-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="3aa6b-158">893</span><span class="sxs-lookup"><span data-stu-id="3aa6b-158">893</span></span>


### <a name="example-3-use-filter-and-top-to-get-one-application-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="3aa6b-159">Exemplo 3: Utilize $filter e $top para obter um aplicativo com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="3aa6b-159">Example 3: Use $filter and $top to get one application with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3aa6b-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3aa6b-160">Request</span></span>

<span data-ttu-id="3aa6b-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3aa6b-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aa6b-162">Response</span></span>

<span data-ttu-id="3aa6b-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-163">The following is an example of the response.</span></span>
><span data-ttu-id="3aa6b-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-search-to-get-applications-with-display-names-that-contain-the-letters-web-including-a-count-of-returned-objects"></a><span data-ttu-id="3aa6b-166">Exemplo 4: Utilize $search para obter aplicativos com nomes de exibição que contenham as letras 'Web', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="3aa6b-166">Example 4: Use $search to get applications with display names that contain the letters 'Web' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3aa6b-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3aa6b-167">Request</span></span>

<span data-ttu-id="3aa6b-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_web_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$search="displayName:Web"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3aa6b-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aa6b-169">Response</span></span>

<span data-ttu-id="3aa6b-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-170">The following is an example of the response.</span></span>
><span data-ttu-id="3aa6b-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


