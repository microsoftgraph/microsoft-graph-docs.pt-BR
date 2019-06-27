---
title: Listar usuários
description: Recuperar uma lista de objetos user. Esses objetos de usuário incluirão propriedades específicas de educação.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 340debc95f926f231889bdd38045b3f5dc0efd2c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275093"
---
# <a name="list-users"></a><span data-ttu-id="f811c-104">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="f811c-104">List users</span></span>

<span data-ttu-id="f811c-105">Recuperar uma lista de objetos user.</span><span class="sxs-lookup"><span data-stu-id="f811c-105">Retrieve a list of user objects.</span></span> <span data-ttu-id="f811c-106">Esses objetos de usuário incluirão propriedades específicas de educação.</span><span class="sxs-lookup"><span data-stu-id="f811c-106">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="f811c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f811c-107">Permissions</span></span>
<span data-ttu-id="f811c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f811c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f811c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f811c-110">Permission type</span></span>      | <span data-ttu-id="f811c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f811c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f811c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f811c-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="f811c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f811c-113">Not supported.</span></span>  |
|<span data-ttu-id="f811c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f811c-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f811c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f811c-115">Not supported.</span></span>  |
|<span data-ttu-id="f811c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f811c-116">Application</span></span> | <span data-ttu-id="f811c-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f811c-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f811c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f811c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f811c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f811c-119">Optional query parameters</span></span>
<span data-ttu-id="f811c-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f811c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f811c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f811c-121">Request headers</span></span>
| <span data-ttu-id="f811c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f811c-122">Header</span></span>       | <span data-ttu-id="f811c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f811c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f811c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f811c-124">Authorization</span></span>  | <span data-ttu-id="f811c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f811c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f811c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f811c-127">Request body</span></span>
<span data-ttu-id="f811c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f811c-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f811c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f811c-129">Response</span></span>
<span data-ttu-id="f811c-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f811c-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f811c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f811c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f811c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f811c-132">Request</span></span>
<span data-ttu-id="f811c-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f811c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/users
```
##### <a name="response"></a><span data-ttu-id="f811c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f811c-134">Response</span></span>
<span data-ttu-id="f811c-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f811c-135">The following is an example of the response.</span></span> 

><span data-ttu-id="f811c-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f811c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "middleName": null,
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
      }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f811c-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f811c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f811c-139">C#</span><span class="sxs-lookup"><span data-stu-id="f811c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f811c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="f811c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_users-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f811c-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f811c-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_users-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationroot-list-users.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/educationroot-list-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationroot-list-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
