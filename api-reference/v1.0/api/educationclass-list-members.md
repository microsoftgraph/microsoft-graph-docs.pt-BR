---
title: Listar membros
description: Recupere os professores e alunos de uma aula. Se o token delegado for usado, os membros poderão ser vistos apenas por outros membros da aula.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 83d1f6e52e11afc60c84977676279ae02182e047
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972583"
---
# <a name="list-members"></a><span data-ttu-id="46ffe-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="46ffe-104">List members</span></span>

<span data-ttu-id="46ffe-105">Recupere os professores e alunos de uma aula.</span><span class="sxs-lookup"><span data-stu-id="46ffe-105">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="46ffe-106">Se o token delegado for usado, os membros poderão ser vistos apenas por outros membros da aula.</span><span class="sxs-lookup"><span data-stu-id="46ffe-106">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="46ffe-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="46ffe-107">Permissions</span></span>
<span data-ttu-id="46ffe-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46ffe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46ffe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46ffe-110">Permission type</span></span>      | <span data-ttu-id="46ffe-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46ffe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46ffe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46ffe-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="46ffe-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="46ffe-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="46ffe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46ffe-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="46ffe-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="46ffe-115">Not supported</span></span>  |
|<span data-ttu-id="46ffe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46ffe-116">Application</span></span> | <span data-ttu-id="46ffe-117">EduRoster.Read.All, EduRoster.ReadWrite.All mais Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="46ffe-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="46ffe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46ffe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="46ffe-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="46ffe-119">Optional query parameters</span></span>
<span data-ttu-id="46ffe-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="46ffe-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46ffe-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46ffe-121">Request headers</span></span>
| <span data-ttu-id="46ffe-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46ffe-122">Header</span></span>       | <span data-ttu-id="46ffe-123">Valor</span><span class="sxs-lookup"><span data-stu-id="46ffe-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="46ffe-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="46ffe-124">Authorization</span></span>  | <span data-ttu-id="46ffe-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46ffe-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="46ffe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46ffe-127">Request body</span></span>
<span data-ttu-id="46ffe-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46ffe-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="46ffe-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="46ffe-129">Response</span></span>
<span data-ttu-id="46ffe-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46ffe-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46ffe-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46ffe-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46ffe-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46ffe-132">Request</span></span>
<span data-ttu-id="46ffe-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="46ffe-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
##### <a name="response"></a><span data-ttu-id="46ffe-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="46ffe-134">Response</span></span>
<span data-ttu-id="46ffe-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="46ffe-135">The following is an example of the response.</span></span> 

><span data-ttu-id="46ffe-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46ffe-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "teacher": {
        "externalId": "13013",
        "teacherNumber": "8802",
      }
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
      "student": {
        "birthDate": "2001-01-01T00:00:00Z",
        "externalId": "13005",
        "gender": "female",
        "grade": "9",
        "graduationYear": "2019",
        "studentNumber": "13005",
      },
      "primaryRole": "student",
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
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
