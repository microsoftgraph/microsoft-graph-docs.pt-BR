---
title: Listar educationUsers
description: Recupere uma lista de usuários em uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: acec750e85f726bf7e889fdcb9ecce90725b7d59
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366326"
---
# <a name="list-educationusers"></a><span data-ttu-id="1bb96-103">Listar educationUsers</span><span class="sxs-lookup"><span data-stu-id="1bb96-103">List educationUsers</span></span>

<span data-ttu-id="1bb96-104">Recupere uma lista de usuários em uma escola.</span><span class="sxs-lookup"><span data-stu-id="1bb96-104">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bb96-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1bb96-105">Permissions</span></span>
<span data-ttu-id="1bb96-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bb96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bb96-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bb96-108">Permission type</span></span>      | <span data-ttu-id="1bb96-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1bb96-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bb96-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bb96-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1bb96-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bb96-111">Not supported.</span></span>  |
|<span data-ttu-id="1bb96-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bb96-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1bb96-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bb96-113">Not supported.</span></span>  |
|<span data-ttu-id="1bb96-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bb96-114">Application</span></span> | <span data-ttu-id="1bb96-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bb96-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1bb96-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bb96-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1bb96-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1bb96-117">Optional query parameters</span></span>
<span data-ttu-id="1bb96-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1bb96-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1bb96-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb96-119">Request headers</span></span>
| <span data-ttu-id="1bb96-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1bb96-120">Header</span></span>       | <span data-ttu-id="1bb96-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1bb96-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1bb96-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bb96-122">Authorization</span></span>  | <span data-ttu-id="1bb96-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bb96-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1bb96-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb96-125">Request body</span></span>
<span data-ttu-id="1bb96-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1bb96-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1bb96-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bb96-127">Response</span></span>
<span data-ttu-id="1bb96-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bb96-128">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1bb96-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bb96-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bb96-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb96-130">Request</span></span>
<span data-ttu-id="1bb96-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bb96-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1bb96-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bb96-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1bb96-133">C#</span><span class="sxs-lookup"><span data-stu-id="1bb96-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1bb96-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bb96-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1bb96-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1bb96-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1bb96-136">Java</span><span class="sxs-lookup"><span data-stu-id="1bb96-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationschool-get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1bb96-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bb96-137">Response</span></span>
<span data-ttu-id="1bb96-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1bb96-138">The following is an example of the response.</span></span> 

><span data-ttu-id="1bb96-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bb96-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
