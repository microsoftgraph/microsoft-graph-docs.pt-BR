---
title: Listar membros
description: Recupere os professores e alunos de uma aula. Se o token delegado for usado, os membros poderão ser vistos apenas por outros membros da aula.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 15714450c00da11b3713fffe0414cd9f2d41ecc2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860602"
---
# <a name="list-members"></a><span data-ttu-id="2f133-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="2f133-104">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f133-105">Recupere os professores e alunos de uma aula.</span><span class="sxs-lookup"><span data-stu-id="2f133-105">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="2f133-106">Se o token delegado for usado, os membros poderão ser vistos apenas por outros membros da aula.</span><span class="sxs-lookup"><span data-stu-id="2f133-106">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f133-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f133-107">Permissions</span></span>
<span data-ttu-id="2f133-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f133-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f133-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f133-110">Permission type</span></span>      | <span data-ttu-id="2f133-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f133-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f133-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f133-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="2f133-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="2f133-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="2f133-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f133-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2f133-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f133-115">Not supported</span></span>  |
|<span data-ttu-id="2f133-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f133-116">Application</span></span> | <span data-ttu-id="2f133-117">EduRoster. Read. All, EduRoster. ReadWrite. All mais member. Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="2f133-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2f133-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f133-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2f133-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2f133-119">Optional query parameters</span></span>
<span data-ttu-id="2f133-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2f133-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f133-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f133-121">Request headers</span></span>
| <span data-ttu-id="2f133-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f133-122">Header</span></span>       | <span data-ttu-id="2f133-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2f133-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f133-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f133-124">Authorization</span></span>  | <span data-ttu-id="2f133-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f133-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f133-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f133-127">Request body</span></span>
<span data-ttu-id="2f133-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f133-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2f133-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f133-129">Response</span></span>
<span data-ttu-id="2f133-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f133-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2f133-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f133-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f133-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f133-132">Request</span></span>
<span data-ttu-id="2f133-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f133-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2f133-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f133-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11016/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2f133-135">C#</span><span class="sxs-lookup"><span data-stu-id="2f133-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f133-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="2f133-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2f133-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2f133-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2f133-138">Java</span><span class="sxs-lookup"><span data-stu-id="2f133-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2f133-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f133-139">Response</span></span>
<span data-ttu-id="2f133-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f133-140">The following is an example of the response.</span></span> 

><span data-ttu-id="2f133-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f133-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "13013",
      "displayName": "Ora Klein",
      "givenName": "Ora",
      "middleName": " ",
      "surname": "Klein",
      "mail": "OraK@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "teacher",
      "externalId": "13013",
      "teacherNumber": "8802",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    },
    {
      "id": "13005",
      "displayName": "Erna Parker",
      "givenName": "Erna",
      "middleName": " ",
      "surname": "Parker",
      "mail": "ernap@contoso.com",
      "mobilePhone": "+1 (253) 555-0104",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z",
      "gender": "female",
      "grade": "9",
      "graduationYear": "2019",
      "studentNumber": "13005",
      "residenceAddress": {
        "city": "Long Beach",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Maple St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
