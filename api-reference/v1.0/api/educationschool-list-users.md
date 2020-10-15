---
title: Listar educationUsers
description: Recupere uma lista de usuários em uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 59c95ee8e889113a4d6ef7419700dfe67095f61b
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460590"
---
# <a name="list-educationusers"></a><span data-ttu-id="6cf1e-103">Listar educationUsers</span><span class="sxs-lookup"><span data-stu-id="6cf1e-103">List educationUsers</span></span>

<span data-ttu-id="6cf1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cf1e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6cf1e-105">Recupere uma lista de usuários em uma escola.</span><span class="sxs-lookup"><span data-stu-id="6cf1e-105">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cf1e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6cf1e-106">Permissions</span></span>
<span data-ttu-id="6cf1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cf1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cf1e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cf1e-109">Permission type</span></span>      | <span data-ttu-id="6cf1e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6cf1e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cf1e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cf1e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="6cf1e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cf1e-112">Not supported.</span></span>  |
|<span data-ttu-id="6cf1e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cf1e-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6cf1e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cf1e-114">Not supported.</span></span>  |
|<span data-ttu-id="6cf1e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cf1e-115">Application</span></span> | <span data-ttu-id="6cf1e-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cf1e-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6cf1e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cf1e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6cf1e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6cf1e-118">Optional query parameters</span></span>
<span data-ttu-id="6cf1e-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6cf1e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cf1e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cf1e-120">Request headers</span></span>
| <span data-ttu-id="6cf1e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6cf1e-121">Header</span></span>       | <span data-ttu-id="6cf1e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6cf1e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6cf1e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cf1e-123">Authorization</span></span>  | <span data-ttu-id="6cf1e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cf1e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6cf1e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cf1e-126">Request body</span></span>
<span data-ttu-id="6cf1e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6cf1e-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6cf1e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cf1e-128">Response</span></span>
<span data-ttu-id="6cf1e-129">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cf1e-129">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6cf1e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cf1e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6cf1e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cf1e-131">Request</span></span>
<span data-ttu-id="6cf1e-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cf1e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6cf1e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cf1e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/users
```
# <a name="c"></a>[<span data-ttu-id="6cf1e-134">C#</span><span class="sxs-lookup"><span data-stu-id="6cf1e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cf1e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cf1e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cf1e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cf1e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cf1e-137">Java</span><span class="sxs-lookup"><span data-stu-id="6cf1e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationschool-get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6cf1e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cf1e-138">Response</span></span>
<span data-ttu-id="6cf1e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6cf1e-139">The following is an example of the response.</span></span> 

><span data-ttu-id="6cf1e-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6cf1e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
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
          "id": "14012",
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
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
