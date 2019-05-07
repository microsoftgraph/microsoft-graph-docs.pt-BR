---
title: Listar professores
description: Recupere uma lista de professores de uma aula. Os tokens delegados devem ser membros da aula para obterem a lista de professores.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ae2ec5a581438b2b3535db38ed624a2b785a8f63
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616034"
---
# <a name="list-teachers"></a><span data-ttu-id="e10eb-104">Listar professores</span><span class="sxs-lookup"><span data-stu-id="e10eb-104">List teachers</span></span>

<span data-ttu-id="e10eb-105">Recupere uma lista de professores de uma aula.</span><span class="sxs-lookup"><span data-stu-id="e10eb-105">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="e10eb-106">Os tokens delegados devem ser membros da aula para obterem a lista de professores.</span><span class="sxs-lookup"><span data-stu-id="e10eb-106">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="e10eb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e10eb-107">Permissions</span></span>
<span data-ttu-id="e10eb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e10eb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e10eb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e10eb-110">Permission type</span></span>      | <span data-ttu-id="e10eb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e10eb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e10eb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e10eb-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="e10eb-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="e10eb-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="e10eb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e10eb-114">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="e10eb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e10eb-115">Not supported.</span></span>  |
|<span data-ttu-id="e10eb-116">Application</span><span class="sxs-lookup"><span data-stu-id="e10eb-116">Application</span></span> | <span data-ttu-id="e10eb-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e10eb-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e10eb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e10eb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e10eb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e10eb-119">Optional query parameters</span></span>
<span data-ttu-id="e10eb-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e10eb-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e10eb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e10eb-121">Request headers</span></span>
| <span data-ttu-id="e10eb-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e10eb-122">Header</span></span>       | <span data-ttu-id="e10eb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e10eb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e10eb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e10eb-124">Authorization</span></span>  | <span data-ttu-id="e10eb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e10eb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e10eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e10eb-127">Request body</span></span>
<span data-ttu-id="e10eb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e10eb-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e10eb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e10eb-129">Response</span></span>
<span data-ttu-id="e10eb-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e10eb-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e10eb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e10eb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e10eb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e10eb-132">Request</span></span>
<span data-ttu-id="e10eb-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e10eb-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers
```
##### <a name="response"></a><span data-ttu-id="e10eb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e10eb-134">Response</span></span>
<span data-ttu-id="e10eb-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e10eb-135">The following is an example of the response.</span></span> 

><span data-ttu-id="e10eb-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e10eb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "14006",
      "displayName": "Kristie Mitchell",
      "givenName": "Kristie",
      "middleName": "Anne",
      "surname": "Mitchell",
      "mail": "kristiem@Contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "Edu",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "Teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e10eb-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e10eb-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e10eb-139">Basic</span><span class="sxs-lookup"><span data-stu-id="e10eb-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_teachers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e10eb-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e10eb-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_teachers-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List teachers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationclass-list-teachers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationclass-list-teachers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
