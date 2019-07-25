---
title: Listar usuários
description: Recuperar uma lista de objetos user. Esses objetos de usuário incluirão propriedades específicas de educação.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2ae96774c395d1b58ae339a7e241c17d1e459a32
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860436"
---
# <a name="list-users"></a><span data-ttu-id="810ca-104">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="810ca-104">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="810ca-105">Recuperar uma lista de objetos user.</span><span class="sxs-lookup"><span data-stu-id="810ca-105">Retrieve a list of user objects.</span></span> <span data-ttu-id="810ca-106">Esses objetos de usuário incluirão propriedades específicas de educação.</span><span class="sxs-lookup"><span data-stu-id="810ca-106">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="810ca-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="810ca-107">Permissions</span></span>
<span data-ttu-id="810ca-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="810ca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="810ca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="810ca-110">Permission type</span></span>      | <span data-ttu-id="810ca-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="810ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="810ca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="810ca-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="810ca-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="810ca-113">Not supported.</span></span>  |
|<span data-ttu-id="810ca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="810ca-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="810ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="810ca-115">Not supported.</span></span>  |
|<span data-ttu-id="810ca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="810ca-116">Application</span></span> | <span data-ttu-id="810ca-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="810ca-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="810ca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="810ca-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="810ca-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="810ca-119">Optional query parameters</span></span>
<span data-ttu-id="810ca-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="810ca-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="810ca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="810ca-121">Request headers</span></span>
| <span data-ttu-id="810ca-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="810ca-122">Header</span></span>       | <span data-ttu-id="810ca-123">Valor</span><span class="sxs-lookup"><span data-stu-id="810ca-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="810ca-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="810ca-124">Authorization</span></span>  | <span data-ttu-id="810ca-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="810ca-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="810ca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="810ca-127">Request body</span></span>
<span data-ttu-id="810ca-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="810ca-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="810ca-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="810ca-129">Response</span></span>
<span data-ttu-id="810ca-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="810ca-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="810ca-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="810ca-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="810ca-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="810ca-132">Request</span></span>
<span data-ttu-id="810ca-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="810ca-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="810ca-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="810ca-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationroot_get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="810ca-135">C#</span><span class="sxs-lookup"><span data-stu-id="810ca-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationroot-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="810ca-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="810ca-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationroot-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="810ca-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="810ca-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationroot-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="810ca-138">Java</span><span class="sxs-lookup"><span data-stu-id="810ca-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationroot-get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="810ca-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="810ca-139">Response</span></span>
<span data-ttu-id="810ca-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="810ca-140">The following is an example of the response.</span></span> 

><span data-ttu-id="810ca-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="810ca-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
