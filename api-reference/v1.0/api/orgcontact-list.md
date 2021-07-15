---
title: Listar orgContacts
description: Recupere a lista de contatos organizacionais dessa organização.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 66da3d385943bcd8b983997ec708efb10ecdd42e
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430113"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="a14e8-103">Listar orgContacts</span><span class="sxs-lookup"><span data-stu-id="a14e8-103">List orgContacts</span></span>

<span data-ttu-id="a14e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a14e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a14e8-105">Obter a lista de [contatos organizacionais](../resources/orgcontact.md) dessa organização.</span><span class="sxs-lookup"><span data-stu-id="a14e8-105">Get the list of [organizational contacts](../resources/orgcontact.md) for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="a14e8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a14e8-106">Permissions</span></span>
<span data-ttu-id="a14e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a14e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a14e8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a14e8-109">Permission type</span></span>      | <span data-ttu-id="a14e8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a14e8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a14e8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a14e8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a14e8-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a14e8-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a14e8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a14e8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a14e8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a14e8-114">Not supported.</span></span>    |
|<span data-ttu-id="a14e8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a14e8-115">Application</span></span> | <span data-ttu-id="a14e8-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a14e8-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a14e8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a14e8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a14e8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a14e8-118">Optional query parameters</span></span>
<span data-ttu-id="a14e8-119">Este método suporta aos parâmetros de consulta `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, e `$top` [OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a14e8-119">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="a14e8-120">Algumas consultas são suportadas somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`.</span><span class="sxs-lookup"><span data-stu-id="a14e8-120">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="a14e8-121">Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="a14e8-121">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a14e8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a14e8-122">Request headers</span></span>
| <span data-ttu-id="a14e8-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a14e8-123">Header</span></span>       | <span data-ttu-id="a14e8-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a14e8-124">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="a14e8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a14e8-125">Authorization</span></span>  |<span data-ttu-id="a14e8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a14e8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a14e8-128">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="a14e8-128">ConsistencyLevel</span></span> | <span data-ttu-id="a14e8-129">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="a14e8-129">eventual.</span></span> <span data-ttu-id="a14e8-130">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou em uso específico de `$filter`.</span><span class="sxs-lookup"><span data-stu-id="a14e8-130">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="a14e8-131">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="a14e8-131">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="a14e8-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a14e8-132">Request body</span></span>
<span data-ttu-id="a14e8-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a14e8-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a14e8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a14e8-134">Response</span></span>

<span data-ttu-id="a14e8-135">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a14e8-135">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a14e8-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a14e8-136">Examples</span></span>

### <a name="example-1-get-organizational-contacts-for-an-organization"></a><span data-ttu-id="a14e8-137">Exemplo 1: Obter contatos organizacionais para uma organização</span><span class="sxs-lookup"><span data-stu-id="a14e8-137">Example 1: Get organizational contacts for an organization</span></span>

#### <a name="request"></a><span data-ttu-id="a14e8-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a14e8-138">Request</span></span>

<span data-ttu-id="a14e8-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a14e8-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a14e8-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a14e8-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts
```
# <a name="c"></a>[<span data-ttu-id="a14e8-141">C#</span><span class="sxs-lookup"><span data-stu-id="a14e8-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a14e8-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a14e8-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a14e8-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a14e8-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a14e8-144">Java</span><span class="sxs-lookup"><span data-stu-id="a14e8-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a14e8-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a14e8-145">Response</span></span>

<span data-ttu-id="a14e8-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a14e8-146">The following is an example of the response.</span></span>

><span data-ttu-id="a14e8-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a14e8-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-organizational-contacts"></a><span data-ttu-id="a14e8-148">Exemplo 2: Obter apenas uma contagem de contatos organizacionais</span><span class="sxs-lookup"><span data-stu-id="a14e8-148">Example 2: Get only a count of organizational contacts</span></span>

#### <a name="request"></a><span data-ttu-id="a14e8-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a14e8-149">Request</span></span>

<span data-ttu-id="a14e8-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a14e8-150">The following is an example of the request.</span></span> <span data-ttu-id="a14e8-151">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$count` está na solicitação.</span><span class="sxs-lookup"><span data-stu-id="a14e8-151">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="a14e8-152">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="a14e8-152">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a14e8-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a14e8-153">Response</span></span>

<span data-ttu-id="a14e8-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a14e8-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```


### <a name="example-3-use-filter-and-top-to-get-one-organizational-contact-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="a14e8-155">Exemplo 3: use $filter e $top para obter um contato organizacional com um nome de exibição que comece com "a" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="a14e8-155">Example 3: Use $filter and $top to get one organizational contact with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a14e8-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a14e8-156">Request</span></span>

<span data-ttu-id="a14e8-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a14e8-157">The following is an example of the request.</span></span> <span data-ttu-id="a14e8-158">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` e a cadeia de caracteres de consulta `$count=true` porque a solicitação tem os parâmetros de consulta `$orderBy` e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="a14e8-158">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="a14e8-159">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="a14e8-159">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a14e8-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="a14e8-160">Response</span></span>

<span data-ttu-id="a14e8-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a14e8-161">The following is an example of the response.</span></span>

><span data-ttu-id="a14e8-162">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a14e8-162">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-search-to-get-organizational-contacts-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="a14e8-163">Exemplo 4: use $search para obter contatos organizacionais com nomes de exibição que contenham as letras 'wa' incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="a14e8-163">Example 4: Use $search to get organizational contacts with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="a14e8-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a14e8-164">Request</span></span>

<span data-ttu-id="a14e8-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a14e8-165">The following is an example of the request.</span></span> <span data-ttu-id="a14e8-166">Essa solicitação requer o header **ConsistencyLevel** definido como porque e a cadeia de caracteres de consulta `eventual` está na `$search` `$count=true` solicitação.</span><span class="sxs-lookup"><span data-stu-id="a14e8-166">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` and the `$count=true` query string is in the request.</span></span> <span data-ttu-id="a14e8-167">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="a14e8-167">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_phone_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts?$search="displayName:wa"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="a14e8-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="a14e8-168">Response</span></span>

<span data-ttu-id="a14e8-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a14e8-169">The following is an example of the response.</span></span>

><span data-ttu-id="a14e8-170">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a14e8-170">**Note:** The response object shown here might be shortened for readability.</span></span>

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

