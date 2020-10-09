---
title: Listar membros
description: Recupere os professores e alunos de uma aula. Se o token delegado for usado, os membros poderão ser vistos apenas por outros membros da aula.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 701dbe9da7a19ac93dd901e0b3ca5523c3d28be0
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403521"
---
# <a name="list-members"></a><span data-ttu-id="02a2a-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="02a2a-104">List members</span></span>

<span data-ttu-id="02a2a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02a2a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02a2a-106">Recupere os professores e alunos de uma aula.</span><span class="sxs-lookup"><span data-stu-id="02a2a-106">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="02a2a-107">Se o token delegado for usado, os membros poderão ser vistos apenas por outros membros da aula.</span><span class="sxs-lookup"><span data-stu-id="02a2a-107">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="02a2a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="02a2a-108">Permissions</span></span>
<span data-ttu-id="02a2a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02a2a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02a2a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02a2a-111">Permission type</span></span>      | <span data-ttu-id="02a2a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02a2a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02a2a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02a2a-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="02a2a-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="02a2a-114">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="02a2a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02a2a-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="02a2a-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="02a2a-116">Not supported</span></span>  |
|<span data-ttu-id="02a2a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02a2a-117">Application</span></span> | <span data-ttu-id="02a2a-118">EduRoster. Read. All, EduRoster. ReadWrite. All mais member. Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="02a2a-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="02a2a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02a2a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="02a2a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="02a2a-120">Optional query parameters</span></span>
<span data-ttu-id="02a2a-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="02a2a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02a2a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02a2a-122">Request headers</span></span>
| <span data-ttu-id="02a2a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02a2a-123">Header</span></span>       | <span data-ttu-id="02a2a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="02a2a-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="02a2a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="02a2a-125">Authorization</span></span>  | <span data-ttu-id="02a2a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02a2a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02a2a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02a2a-128">Request body</span></span>
<span data-ttu-id="02a2a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02a2a-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="02a2a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="02a2a-130">Response</span></span>
<span data-ttu-id="02a2a-131">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02a2a-131">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="02a2a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02a2a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02a2a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02a2a-133">Request</span></span>
<span data-ttu-id="02a2a-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02a2a-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="02a2a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="02a2a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationclass_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11016/members
```
# <a name="c"></a>[<span data-ttu-id="02a2a-136">C#</span><span class="sxs-lookup"><span data-stu-id="02a2a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationclass-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02a2a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02a2a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationclass-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02a2a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02a2a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationclass-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="02a2a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="02a2a-139">Response</span></span>
<span data-ttu-id="02a2a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02a2a-140">The following is an example of the response.</span></span> 

><span data-ttu-id="02a2a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02a2a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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