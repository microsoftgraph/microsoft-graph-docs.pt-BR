---
title: Listar orgContacts
description: Recupere a lista de contatos organizacionais desta organização.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a44c82b6eef63863577bfd64e44e3ab020fc67a0
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336757"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="9a3b6-103">Listar orgContacts</span><span class="sxs-lookup"><span data-stu-id="9a3b6-103">List orgContacts</span></span>

<span data-ttu-id="9a3b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a3b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a3b6-105">Obtenha a lista de contatos organizacionais para esta organização.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-105">Get the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a3b6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a3b6-106">Permissions</span></span>
<span data-ttu-id="9a3b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a3b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a3b6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a3b6-109">Permission type</span></span>      | <span data-ttu-id="9a3b6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a3b6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a3b6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a3b6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a3b6-112">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="9a3b6-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9a3b6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a3b6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a3b6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-114">Not supported.</span></span>    |
|<span data-ttu-id="9a3b6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a3b6-115">Application</span></span> | <span data-ttu-id="9a3b6-116">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9a3b6-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a3b6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a3b6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9a3b6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9a3b6-118">Optional query parameters</span></span>
<span data-ttu-id="9a3b6-119">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search` , `$count` e `$filter` .</span><span class="sxs-lookup"><span data-stu-id="9a3b6-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="9a3b6-120">Você pode usar `$search` na propriedade **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="9a3b6-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="9a3b6-121">Quando os itens são adicionados ou atualizados para esse recurso, eles são especialmente indexados para uso com os `$count` `$search` parâmetros de consulta e.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="9a3b6-122">Pode haver um ligeiro atraso entre a adição ou atualização de um item e quando ele está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a3b6-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a3b6-123">Request headers</span></span>
| <span data-ttu-id="9a3b6-124">Nome</span><span class="sxs-lookup"><span data-stu-id="9a3b6-124">Name</span></span>       | <span data-ttu-id="9a3b6-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a3b6-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="9a3b6-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a3b6-126">Authorization</span></span>  | <span data-ttu-id="9a3b6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a3b6-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="9a3b6-129">ConsistencyLevel</span></span> | <span data-ttu-id="9a3b6-130">ocorra.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-130">eventual.</span></span> <span data-ttu-id="9a3b6-131">Esse cabeçalho e `$count` são necessários ao usar `$search` ou ao usar `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="9a3b6-132">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a3b6-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a3b6-133">Request body</span></span>
<span data-ttu-id="9a3b6-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a3b6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a3b6-135">Response</span></span>

<span data-ttu-id="9a3b6-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-136">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a3b6-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9a3b6-137">Examples</span></span>

### <a name="example-1-get-organizational-contacts-for-an-organization"></a><span data-ttu-id="9a3b6-138">Exemplo 1: obter contatos organizacionais para uma organização</span><span class="sxs-lookup"><span data-stu-id="9a3b6-138">Example 1: Get organizational contacts for an organization</span></span>

#### <a name="request"></a><span data-ttu-id="9a3b6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a3b6-139">Request</span></span>

<span data-ttu-id="9a3b6-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a3b6-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a3b6-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts
```
# <a name="c"></a>[<span data-ttu-id="9a3b6-142">C#</span><span class="sxs-lookup"><span data-stu-id="9a3b6-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a3b6-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a3b6-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a3b6-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a3b6-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9a3b6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a3b6-145">Response</span></span>

<span data-ttu-id="9a3b6-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-146">Here is an example of the response.</span></span> 
><span data-ttu-id="9a3b6-147">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9a3b6-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-148">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-organizational-contacts"></a><span data-ttu-id="9a3b6-149">Exemplo 2: obter apenas uma contagem de contatos organizacionais</span><span class="sxs-lookup"><span data-stu-id="9a3b6-149">Example 2: Get only a count of organizational contacts</span></span>

#### <a name="request"></a><span data-ttu-id="9a3b6-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a3b6-150">Request</span></span>

<span data-ttu-id="9a3b6-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9a3b6-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a3b6-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="9a3b6-153">C#</span><span class="sxs-lookup"><span data-stu-id="9a3b6-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a3b6-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a3b6-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a3b6-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a3b6-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9a3b6-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a3b6-156">Response</span></span>

<span data-ttu-id="9a3b6-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="9a3b6-158">893</span><span class="sxs-lookup"><span data-stu-id="9a3b6-158">893</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-organizational-contact-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="9a3b6-159">Exemplo 3: use $filter e $top para obter um contato organizacional com um nome de exibição que comece com ' a ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="9a3b6-159">Example 3: Use $filter and $top to get one organizational contact with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9a3b6-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a3b6-160">Request</span></span>

<span data-ttu-id="9a3b6-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9a3b6-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a3b6-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="9a3b6-163">C#</span><span class="sxs-lookup"><span data-stu-id="9a3b6-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a3b6-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a3b6-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a3b6-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a3b6-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9a3b6-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a3b6-166">Response</span></span>

<span data-ttu-id="9a3b6-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-167">The following is an example of the response.</span></span>
><span data-ttu-id="9a3b6-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-search-to-get-organizational-contacts-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="9a3b6-170">Exemplo 4: Use $search para obter contatos organizacionais com nomes de exibição que contenham as letras "WA", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="9a3b6-170">Example 4: Use $search to get organizational contacts with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9a3b6-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a3b6-171">Request</span></span>

<span data-ttu-id="9a3b6-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-172">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9a3b6-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a3b6-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phone_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$search="displayName:wa"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="9a3b6-174">C#</span><span class="sxs-lookup"><span data-stu-id="9a3b6-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phone-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a3b6-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a3b6-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phone-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a3b6-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a3b6-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phone-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9a3b6-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a3b6-177">Response</span></span>

<span data-ttu-id="9a3b6-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-178">The following is an example of the response.</span></span>
><span data-ttu-id="9a3b6-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a3b6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
