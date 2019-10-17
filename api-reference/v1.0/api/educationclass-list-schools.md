---
title: Listar escolas
description: Recupere uma lista de escolas nas quais a aula é ministrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3e6bb02c9736badb39c84ed642ea7d0d05e596e5
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37553926"
---
# <a name="list-schools"></a><span data-ttu-id="85719-103">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="85719-103">List schools</span></span>

<span data-ttu-id="85719-104">Recupere uma lista de escolas nas quais a aula é ministrada.</span><span class="sxs-lookup"><span data-stu-id="85719-104">Retrieve a list of schools in which the class is taught.</span></span>

## <a name="permissions"></a><span data-ttu-id="85719-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="85719-105">Permissions</span></span>

<span data-ttu-id="85719-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85719-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85719-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85719-108">Permission type</span></span>                        | <span data-ttu-id="85719-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85719-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="85719-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85719-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="85719-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="85719-111">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="85719-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85719-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85719-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="85719-113">Not supported</span></span>                               |
| <span data-ttu-id="85719-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85719-114">Application</span></span>                            | <span data-ttu-id="85719-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85719-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="85719-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85719-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85719-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="85719-117">Optional query parameters</span></span>

<span data-ttu-id="85719-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="85719-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85719-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85719-119">Request headers</span></span>

| <span data-ttu-id="85719-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85719-120">Header</span></span>        | <span data-ttu-id="85719-121">Valor</span><span class="sxs-lookup"><span data-stu-id="85719-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="85719-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="85719-122">Authorization</span></span> | <span data-ttu-id="85719-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85719-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85719-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85719-125">Request body</span></span>

<span data-ttu-id="85719-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85719-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85719-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="85719-127">Response</span></span>

<span data-ttu-id="85719-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85719-128">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85719-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85719-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="85719-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85719-130">Request</span></span>

<span data-ttu-id="85719-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="85719-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="85719-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="85719-132">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/schools
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="85719-133">C#</span><span class="sxs-lookup"><span data-stu-id="85719-133">C#</span></span>](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="85719-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85719-134">JavaScript</span></span>](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="85719-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85719-135">Objective-C</span></span>](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="85719-136">Java</span><span class="sxs-lookup"><span data-stu-id="85719-136">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](../includes/snippets/java/get-schools-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="85719-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="85719-137">Response</span></span>

<span data-ttu-id="85719-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85719-138">The following is an example of the response.</span></span>

><span data-ttu-id="85719-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85719-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 892

{
  "value": [
    {
      "id": "10002",
      "displayName": "Fabrikam High School",
      "description": "Magnate school for the arts. Los Angeles School District",
      "status": "String",
      "externalSource": "String",
      "principalEmail": "AmyR@fabrikam.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10002",
      "address": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalId": "10002",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
