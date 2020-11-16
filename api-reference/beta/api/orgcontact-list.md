---
title: Listar orgContacts
description: Recupere a lista de contatos organizacionais desta organização.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 242b4906a52ffb9af540bd8fc44244c665dc2037
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2020
ms.locfileid: "49081893"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="e7507-103">Listar orgContacts</span><span class="sxs-lookup"><span data-stu-id="e7507-103">List orgContacts</span></span>

<span data-ttu-id="e7507-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7507-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7507-105">Obtenha a lista de contatos organizacionais para esta organização.</span><span class="sxs-lookup"><span data-stu-id="e7507-105">Get the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7507-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e7507-106">Permissions</span></span>
<span data-ttu-id="e7507-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7507-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7507-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7507-109">Permission type</span></span>      | <span data-ttu-id="e7507-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7507-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7507-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7507-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e7507-112">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="e7507-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e7507-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7507-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7507-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7507-114">Not supported.</span></span>    |
|<span data-ttu-id="e7507-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7507-115">Application</span></span> | <span data-ttu-id="e7507-116">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e7507-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7507-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7507-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e7507-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e7507-118">Optional query parameters</span></span>
<span data-ttu-id="e7507-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="e7507-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="e7507-120">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="e7507-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="e7507-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="e7507-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="e7507-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="e7507-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7507-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7507-123">Request headers</span></span>
| <span data-ttu-id="e7507-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e7507-124">Name</span></span>       | <span data-ttu-id="e7507-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7507-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="e7507-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7507-126">Authorization</span></span>  | <span data-ttu-id="e7507-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7507-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7507-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="e7507-129">ConsistencyLevel</span></span> | <span data-ttu-id="e7507-130">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="e7507-130">eventual.</span></span> <span data-ttu-id="e7507-131">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="e7507-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="e7507-132">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="e7507-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7507-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7507-133">Request body</span></span>
<span data-ttu-id="e7507-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7507-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7507-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7507-135">Response</span></span>

<span data-ttu-id="e7507-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7507-136">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e7507-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e7507-137">Examples</span></span>

### <a name="example-1-get-organizational-contacts-for-an-organization"></a><span data-ttu-id="e7507-138">Exemplo 1: obter contatos organizacionais para uma organização</span><span class="sxs-lookup"><span data-stu-id="e7507-138">Example 1: Get organizational contacts for an organization</span></span>

#### <a name="request"></a><span data-ttu-id="e7507-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7507-139">Request</span></span>

<span data-ttu-id="e7507-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7507-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e7507-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7507-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts
```
# <a name="c"></a>[<span data-ttu-id="e7507-142">C#</span><span class="sxs-lookup"><span data-stu-id="e7507-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7507-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7507-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7507-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7507-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7507-145">Java</span><span class="sxs-lookup"><span data-stu-id="e7507-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e7507-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7507-146">Response</span></span>

<span data-ttu-id="e7507-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7507-147">Here is an example of the response.</span></span> 
><span data-ttu-id="e7507-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7507-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "companyName":"Contoso",
      "department":"Accounting",
      "displayName":"Eric Solomon",
      "givenName":"Eric",
      "jobTitle":"Accountant",
      "mail":"erics@contoso.com",
      "mailNickname":"erics",
      "surname":"Solomon",
      "addresses":[
        {
          "city":"MyCity",
          "countryOrRegion":"United States",
          "officeLocation":"MyCity",
          "postalCode":"98000",
          "state":"WA",
          "street":"Contoso Way"
        }
      ],
      "phones":[
        {
          "number":"111-1111",
          "type":"businessFax"
        }
      ]
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-organizational-contacts"></a><span data-ttu-id="e7507-150">Exemplo 2: obter apenas uma contagem de contatos organizacionais</span><span class="sxs-lookup"><span data-stu-id="e7507-150">Example 2: Get only a count of organizational contacts</span></span>

#### <a name="request"></a><span data-ttu-id="e7507-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7507-151">Request</span></span>

<span data-ttu-id="e7507-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7507-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="e7507-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7507-153">Response</span></span>

<span data-ttu-id="e7507-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7507-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="e7507-155">893</span><span class="sxs-lookup"><span data-stu-id="e7507-155">893</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-organizational-contact-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="e7507-156">Exemplo 3: use $filter e $top para obter um contato organizacional com um nome de exibição que comece com ' a ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="e7507-156">Example 3: Use $filter and $top to get one organizational contact with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="e7507-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7507-157">Request</span></span>

<span data-ttu-id="e7507-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7507-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="e7507-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7507-159">Response</span></span>

<span data-ttu-id="e7507-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7507-160">The following is an example of the response.</span></span>
><span data-ttu-id="e7507-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7507-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
  "@odata.count":1,
  "value":[
    {
      "displayName":"Abigail Jackson",
      "mail":"abigailJ@contoso.com",
      "mailNickname":"abigailJ"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-organizational-contacts-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="e7507-163">Exemplo 4: Use $search para obter contatos organizacionais com nomes de exibição que contenham as letras "WA", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="e7507-163">Example 4: Use $search to get organizational contacts with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="e7507-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7507-164">Request</span></span>

<span data-ttu-id="e7507-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7507-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_phone_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$search="displayName:wa"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="e7507-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7507-166">Response</span></span>

<span data-ttu-id="e7507-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7507-167">The following is an example of the response.</span></span>
><span data-ttu-id="e7507-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7507-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
  "@odata.count":22,
  "value":[
    {
      "displayName":"Nicole Wagner",
      "mail":"nicolewa@contoso.com",
      "mailNickname":"nicolewa"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


