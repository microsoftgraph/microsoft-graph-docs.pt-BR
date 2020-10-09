---
title: Listar escolas
description: Recupere uma lista de escolas nas quais a aula é ministrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 19c25b81035bd1afc194094e8074d50900ba1309
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402244"
---
# <a name="list-schools"></a><span data-ttu-id="c9807-103">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="c9807-103">List schools</span></span>

<span data-ttu-id="c9807-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9807-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c9807-105">Recupere uma lista de escolas nas quais a aula é ministrada.</span><span class="sxs-lookup"><span data-stu-id="c9807-105">Retrieve a list of schools in which the class is taught.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9807-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9807-106">Permissions</span></span>

<span data-ttu-id="c9807-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9807-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c9807-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9807-109">Permission type</span></span>                        | <span data-ttu-id="c9807-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9807-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c9807-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9807-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9807-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="c9807-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="c9807-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9807-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9807-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c9807-114">Not supported</span></span>                               |
| <span data-ttu-id="c9807-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9807-115">Application</span></span>                            | <span data-ttu-id="c9807-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9807-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9807-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9807-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9807-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c9807-118">Optional query parameters</span></span>

<span data-ttu-id="c9807-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c9807-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9807-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9807-120">Request headers</span></span>

| <span data-ttu-id="c9807-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9807-121">Header</span></span>        | <span data-ttu-id="c9807-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c9807-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="c9807-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9807-123">Authorization</span></span> | <span data-ttu-id="c9807-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9807-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9807-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9807-126">Request body</span></span>

<span data-ttu-id="c9807-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9807-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9807-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9807-128">Response</span></span>

<span data-ttu-id="c9807-129">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9807-129">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9807-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9807-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c9807-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9807-131">Request</span></span>

<span data-ttu-id="c9807-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9807-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c9807-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9807-133">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/schools
```

# <a name="c"></a>[<span data-ttu-id="c9807-134">C#</span><span class="sxs-lookup"><span data-stu-id="c9807-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9807-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9807-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9807-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9807-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9807-137">Java</span><span class="sxs-lookup"><span data-stu-id="c9807-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schools-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c9807-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9807-138">Response</span></span>

<span data-ttu-id="c9807-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c9807-139">The following is an example of the response.</span></span>

><span data-ttu-id="c9807-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9807-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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