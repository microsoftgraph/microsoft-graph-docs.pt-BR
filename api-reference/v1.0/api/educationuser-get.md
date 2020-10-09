---
title: Obter educationUser
description: Recupere as propriedades e as relações de um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: bdaa75966034a3ae05e6d1158c24cc79c2277747
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403710"
---
# <a name="get-educationuser"></a><span data-ttu-id="551a4-103">Obter educationUser</span><span class="sxs-lookup"><span data-stu-id="551a4-103">Get educationUser</span></span>

<span data-ttu-id="551a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="551a4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="551a4-105">Recupere as propriedades e as relações de um usuário.</span><span class="sxs-lookup"><span data-stu-id="551a4-105">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="551a4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="551a4-106">Permissions</span></span>
<span data-ttu-id="551a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="551a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="551a4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="551a4-109">Permission type</span></span>      | <span data-ttu-id="551a4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="551a4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="551a4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="551a4-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="551a4-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="551a4-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="551a4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="551a4-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="551a4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="551a4-114">Not supported.</span></span>  |
|<span data-ttu-id="551a4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="551a4-115">Application</span></span> | <span data-ttu-id="551a4-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="551a4-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="551a4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="551a4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="551a4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="551a4-118">Optional query parameters</span></span>
<span data-ttu-id="551a4-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="551a4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="551a4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="551a4-120">Request headers</span></span>
| <span data-ttu-id="551a4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="551a4-121">Header</span></span>       | <span data-ttu-id="551a4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="551a4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="551a4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="551a4-123">Authorization</span></span>  | <span data-ttu-id="551a4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="551a4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="551a4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="551a4-126">Request body</span></span>
<span data-ttu-id="551a4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="551a4-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="551a4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="551a4-128">Response</span></span>
<span data-ttu-id="551a4-129">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="551a4-129">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="551a4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="551a4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="551a4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="551a4-131">Request</span></span>
<span data-ttu-id="551a4-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="551a4-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="551a4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="551a4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="551a4-134">C#</span><span class="sxs-lookup"><span data-stu-id="551a4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="551a4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="551a4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="551a4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="551a4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="551a4-137">Java</span><span class="sxs-lookup"><span data-stu-id="551a4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="551a4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="551a4-138">Response</span></span>
<span data-ttu-id="551a4-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="551a4-139">The following is an example of the response.</span></span> 

><span data-ttu-id="551a4-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="551a4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

{
  "id": "13012",
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": " ",
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    }
  },
  "externalSource": "sis",
  "mailingAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "primaryRole": "student",
  "residenceAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->