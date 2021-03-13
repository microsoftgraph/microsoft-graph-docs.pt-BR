---
title: Listar orgContacts
description: Recupere a lista de contatos organizacionais dessa organização.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4919459f6501974970edbdafe51bb97bececd42f
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761581"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="ca313-103">Listar orgContacts</span><span class="sxs-lookup"><span data-stu-id="ca313-103">List orgContacts</span></span>

<span data-ttu-id="ca313-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca313-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ca313-105">Obter a lista de [contatos organizacionais](../resources/orgcontact.md) dessa organização.</span><span class="sxs-lookup"><span data-stu-id="ca313-105">Get the list of [organizational contacts](../resources/orgcontact.md) for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca313-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ca313-106">Permissions</span></span>
<span data-ttu-id="ca313-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca313-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca313-109">Permission type</span></span>      | <span data-ttu-id="ca313-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca313-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca313-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca313-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ca313-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ca313-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ca313-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca313-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca313-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca313-114">Not supported.</span></span>    |
|<span data-ttu-id="ca313-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca313-115">Application</span></span> | <span data-ttu-id="ca313-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca313-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca313-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca313-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ca313-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ca313-118">Optional query parameters</span></span>
<span data-ttu-id="ca313-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$expand` `$filter` `$search` `$select` `$top` .</span><span class="sxs-lookup"><span data-stu-id="ca313-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$expand`, `$filter`, `$search`,`$select`, and `$top`.</span></span> <span data-ttu-id="ca313-120">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="ca313-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="ca313-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="ca313-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="ca313-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="ca313-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca313-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca313-123">Request headers</span></span>
| <span data-ttu-id="ca313-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca313-124">Header</span></span>       | <span data-ttu-id="ca313-125">Valor</span><span class="sxs-lookup"><span data-stu-id="ca313-125">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ca313-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca313-126">Authorization</span></span>  |<span data-ttu-id="ca313-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca313-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca313-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="ca313-129">ConsistencyLevel</span></span> | <span data-ttu-id="ca313-130">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="ca313-130">eventual.</span></span> <span data-ttu-id="ca313-131">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="ca313-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="ca313-132">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="ca313-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca313-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca313-133">Request body</span></span>
<span data-ttu-id="ca313-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca313-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca313-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca313-135">Response</span></span>

<span data-ttu-id="ca313-136">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca313-136">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca313-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ca313-137">Examples</span></span>

### <a name="example-1-get-organizational-contacts-for-an-organization"></a><span data-ttu-id="ca313-138">Exemplo 1: Obter contatos organizacionais para uma organização</span><span class="sxs-lookup"><span data-stu-id="ca313-138">Example 1: Get organizational contacts for an organization</span></span>

#### <a name="request"></a><span data-ttu-id="ca313-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca313-139">Request</span></span>

<span data-ttu-id="ca313-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca313-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ca313-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca313-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts
```
# <a name="c"></a>[<span data-ttu-id="ca313-142">C#</span><span class="sxs-lookup"><span data-stu-id="ca313-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca313-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca313-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca313-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca313-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca313-145">Java</span><span class="sxs-lookup"><span data-stu-id="ca313-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ca313-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca313-146">Response</span></span>

<span data-ttu-id="ca313-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ca313-147">The following is an example of the response.</span></span>

><span data-ttu-id="ca313-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca313-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value": [
    {
      "companyName": "Contoso",
      "department": "Marketing",
      "displayName": "Eric S",
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

### <a name="example-2-get-only-a-count-of-organizational-contacts"></a><span data-ttu-id="ca313-150">Exemplo 2: Obter apenas uma contagem de contatos organizacionais</span><span class="sxs-lookup"><span data-stu-id="ca313-150">Example 2: Get only a count of organizational contacts</span></span>

#### <a name="request"></a><span data-ttu-id="ca313-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca313-151">Request</span></span>

<span data-ttu-id="ca313-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca313-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ca313-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca313-153">Response</span></span>

<span data-ttu-id="ca313-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ca313-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-filter-and-top-to-get-one-organizational-contact-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="ca313-155">Exemplo 3: use $filter e $top para obter um contato organizacional com um nome de exibição que comece com "a" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="ca313-155">Example 3: Use $filter and $top to get one organizational contact with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ca313-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca313-156">Request</span></span>

<span data-ttu-id="ca313-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca313-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ca313-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca313-158">Response</span></span>

<span data-ttu-id="ca313-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ca313-159">The following is an example of the response.</span></span>

><span data-ttu-id="ca313-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca313-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
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

### <a name="example-4-use-search-to-get-organizational-contacts-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="ca313-162">Exemplo 4: use $search para obter contatos organizacionais com nomes de exibição que contenham as letras 'wa' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="ca313-162">Example 4: Use $search to get organizational contacts with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ca313-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca313-163">Request</span></span>

<span data-ttu-id="ca313-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca313-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_phone_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts?$search="displayName:wa"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ca313-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca313-165">Response</span></span>

<span data-ttu-id="ca313-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ca313-166">The following is an example of the response.</span></span>

><span data-ttu-id="ca313-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca313-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
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

