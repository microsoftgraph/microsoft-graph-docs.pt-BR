---
title: Obter educationUser
description: Recupere as propriedades e as relações de um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8a98d37c2c684847cca88a5319ab72837c4132ca
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963685"
---
# <a name="get-educationuser"></a><span data-ttu-id="a716e-103">Obter educationUser</span><span class="sxs-lookup"><span data-stu-id="a716e-103">Get educationUser</span></span>

<span data-ttu-id="a716e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a716e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a716e-105">Recupere as propriedades e as relações de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a716e-105">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a716e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a716e-106">Permissions</span></span>
<span data-ttu-id="a716e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a716e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a716e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a716e-109">Permission type</span></span>      | <span data-ttu-id="a716e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a716e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a716e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a716e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="a716e-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a716e-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="a716e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a716e-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a716e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a716e-114">Not supported.</span></span>  |
|<span data-ttu-id="a716e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a716e-115">Application</span></span> | <span data-ttu-id="a716e-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a716e-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="a716e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a716e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a716e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a716e-118">Optional query parameters</span></span>
<span data-ttu-id="a716e-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a716e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a716e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a716e-120">Request headers</span></span>
| <span data-ttu-id="a716e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a716e-121">Header</span></span>       | <span data-ttu-id="a716e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a716e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a716e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a716e-123">Authorization</span></span>  | <span data-ttu-id="a716e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a716e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a716e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a716e-126">Request body</span></span>
<span data-ttu-id="a716e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a716e-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a716e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a716e-128">Response</span></span>
<span data-ttu-id="a716e-129">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a716e-129">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a716e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a716e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a716e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a716e-131">Request</span></span>
<span data-ttu-id="a716e-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a716e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a716e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a716e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationuser_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="a716e-134">C#</span><span class="sxs-lookup"><span data-stu-id="a716e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a716e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a716e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a716e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a716e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a716e-137">Java</span><span class="sxs-lookup"><span data-stu-id="a716e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a716e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a716e-138">Response</span></span>
<span data-ttu-id="a716e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a716e-139">The following is an example of the response.</span></span> 

><span data-ttu-id="a716e-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a716e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
