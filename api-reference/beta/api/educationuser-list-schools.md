---
title: Listar escolas
description: Recupere uma lista de escolas de um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1709cbf5abaad87e22677ee9222927b2a83a125f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954680"
---
# <a name="list-schools"></a><span data-ttu-id="74cc2-103">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="74cc2-103">List schools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74cc2-104">Recupere uma lista de escolas de um usuário.</span><span class="sxs-lookup"><span data-stu-id="74cc2-104">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="74cc2-105">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="74cc2-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="74cc2-106">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="74cc2-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="74cc2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="74cc2-107">Permissions</span></span>
<span data-ttu-id="74cc2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74cc2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74cc2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74cc2-110">Permission type</span></span>      | <span data-ttu-id="74cc2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74cc2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74cc2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74cc2-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="74cc2-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="74cc2-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="74cc2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74cc2-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="74cc2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74cc2-115">Not supported.</span></span>  |
|<span data-ttu-id="74cc2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74cc2-116">Application</span></span> | <span data-ttu-id="74cc2-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74cc2-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="74cc2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74cc2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="74cc2-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="74cc2-119">Optional query parameters</span></span>
<span data-ttu-id="74cc2-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="74cc2-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74cc2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74cc2-121">Request headers</span></span>
| <span data-ttu-id="74cc2-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74cc2-122">Header</span></span>       | <span data-ttu-id="74cc2-123">Valor</span><span class="sxs-lookup"><span data-stu-id="74cc2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="74cc2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="74cc2-124">Authorization</span></span>  | <span data-ttu-id="74cc2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74cc2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74cc2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74cc2-127">Request body</span></span>
<span data-ttu-id="74cc2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74cc2-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="74cc2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="74cc2-129">Response</span></span>
<span data-ttu-id="74cc2-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74cc2-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="74cc2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74cc2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74cc2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74cc2-132">Request</span></span>
<span data-ttu-id="74cc2-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="74cc2-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="74cc2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="74cc2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/schools
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="74cc2-135">C#</span><span class="sxs-lookup"><span data-stu-id="74cc2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74cc2-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="74cc2-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74cc2-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="74cc2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="74cc2-138">Java</span><span class="sxs-lookup"><span data-stu-id="74cc2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schools-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="74cc2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="74cc2-139">Response</span></span>
<span data-ttu-id="74cc2-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="74cc2-140">The following is an example of the response.</span></span> 

><span data-ttu-id="74cc2-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74cc2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
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
      "externalId": "10001",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
