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
# <a name="list-applications"></a><span data-ttu-id="63fc8-103">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="63fc8-103">List applications</span></span>

<span data-ttu-id="63fc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63fc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63fc8-105">Obtenha a lista de [applications](../resources/application.md) nesta organização.</span><span class="sxs-lookup"><span data-stu-id="63fc8-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

> [!NOTE]
> <span data-ttu-id="63fc8-106">Ao chamar essa API usando tokens emitidos para uma conta Microsoft pessoal, ele retornará os aplicativos pertencentes à conta Microsoft pessoal.</span><span class="sxs-lookup"><span data-stu-id="63fc8-106">When calling this API using tokens issued for a personal Microsoft account, it will return the apps owned by the personal Microsoft account.</span></span> <span data-ttu-id="63fc8-107">A noção de organizações não existe para contas Microsoft pessoais.</span><span class="sxs-lookup"><span data-stu-id="63fc8-107">The notion of organizations doesn't exist for personal Microsoft accounts.</span></span> <span data-ttu-id="63fc8-108">Para listar os aplicativos pertencentes a contas Microsoft pessoais, essa API exige a permissão User.Read, além de Application.Read.All ou Application.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="63fc8-108">In order to list applications owned by specific personal Microsoft accounts, this API requires User.Read permission in addition to Application.Read.All or Application.ReadWrite.All.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="63fc8-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="63fc8-109">Permissions</span></span>

<span data-ttu-id="63fc8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63fc8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63fc8-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63fc8-112">Permission type</span></span> | <span data-ttu-id="63fc8-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63fc8-113">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="63fc8-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63fc8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="63fc8-115">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="63fc8-115">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="63fc8-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63fc8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63fc8-117">Application.Read.All e User.Read, Application.ReadWrite.All e User.Read</span><span class="sxs-lookup"><span data-stu-id="63fc8-117">Application.Read.All and User.Read, Application.ReadWrite.All and User.Read</span></span>  |
| <span data-ttu-id="63fc8-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63fc8-118">Application</span></span> | <span data-ttu-id="63fc8-119">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="63fc8-119">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63fc8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63fc8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="63fc8-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="63fc8-121">Optional query parameters</span></span>

<span data-ttu-id="63fc8-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="63fc8-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="63fc8-123">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="63fc8-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="63fc8-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="63fc8-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="63fc8-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="63fc8-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63fc8-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63fc8-126">Request headers</span></span>

| <span data-ttu-id="63fc8-127">Nome</span><span class="sxs-lookup"><span data-stu-id="63fc8-127">Name</span></span> | <span data-ttu-id="63fc8-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="63fc8-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="63fc8-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="63fc8-129">Authorization</span></span>  | <span data-ttu-id="63fc8-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63fc8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="63fc8-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="63fc8-132">ConsistencyLevel</span></span> | <span data-ttu-id="63fc8-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="63fc8-133">eventual.</span></span> <span data-ttu-id="63fc8-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="63fc8-134">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="63fc8-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="63fc8-135">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63fc8-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63fc8-136">Request body</span></span>

<span data-ttu-id="63fc8-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63fc8-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63fc8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="63fc8-138">Response</span></span>

<span data-ttu-id="63fc8-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63fc8-139">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63fc8-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="63fc8-140">Examples</span></span>

### <a name="example-1-get-the-list-of-applications"></a><span data-ttu-id="63fc8-141">Exemplo 1: obter a lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="63fc8-141">Example 1: Get the list of applications</span></span>

#### <a name="request"></a><span data-ttu-id="63fc8-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63fc8-142">Request</span></span>

<span data-ttu-id="63fc8-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63fc8-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63fc8-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="63fc8-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications
```
# <a name="c"></a>[<span data-ttu-id="63fc8-145">C#</span><span class="sxs-lookup"><span data-stu-id="63fc8-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63fc8-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63fc8-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63fc8-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63fc8-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63fc8-148">Java</span><span class="sxs-lookup"><span data-stu-id="63fc8-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="63fc8-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="63fc8-149">Response</span></span>

<span data-ttu-id="63fc8-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63fc8-150">Here is an example of the response.</span></span>
> <span data-ttu-id="63fc8-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63fc8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-applications"></a><span data-ttu-id="63fc8-153">Exemplo 2: obter apenas uma contagem de aplicativos</span><span class="sxs-lookup"><span data-stu-id="63fc8-153">Example 2: Get only a count of applications</span></span>

#### <a name="request"></a><span data-ttu-id="63fc8-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63fc8-154">Request</span></span>

<span data-ttu-id="63fc8-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="63fc8-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="63fc8-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="63fc8-156">Response</span></span>

<span data-ttu-id="63fc8-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="63fc8-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="63fc8-158">893</span><span class="sxs-lookup"><span data-stu-id="63fc8-158">893</span></span>


### <a name="example-3-use-filter-and-top-to-get-one-application-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="63fc8-159">Exemplo 3: Utilize $filter e $top para obter um aplicativo com um nome de exibição que comece com a letra 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="63fc8-159">Example 3: Use $filter and $top to get one application with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="63fc8-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63fc8-160">Request</span></span>

<span data-ttu-id="63fc8-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="63fc8-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="63fc8-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="63fc8-162">Response</span></span>

<span data-ttu-id="63fc8-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="63fc8-163">The following is an example of the response.</span></span>
><span data-ttu-id="63fc8-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63fc8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-search-to-get-applications-with-display-names-that-contain-the-letters-web-including-a-count-of-returned-objects"></a><span data-ttu-id="63fc8-166">Exemplo 4: Utilize $search para obter aplicativos com nomes de exibição que contenham as letras 'Web', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="63fc8-166">Example 4: Use $search to get applications with display names that contain the letters 'Web' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="63fc8-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63fc8-167">Request</span></span>

<span data-ttu-id="63fc8-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="63fc8-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_web_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications?$search="displayName:Web"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="63fc8-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="63fc8-169">Response</span></span>

<span data-ttu-id="63fc8-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="63fc8-170">The following is an example of the response.</span></span>
><span data-ttu-id="63fc8-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63fc8-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


