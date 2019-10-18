---
title: Listar educationSchools
description: Recupere uma lista de todos os objetos de escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d719268a8b3e6ff044e928485449320b77bbeff4
ms.sourcegitcommit: 6deec57c0ab736260ee3599703bfd3f567ee6d82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2019
ms.locfileid: "37581199"
---
# <a name="list-educationschools"></a><span data-ttu-id="99bb5-103">Listar educationSchools</span><span class="sxs-lookup"><span data-stu-id="99bb5-103">List educationSchools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99bb5-104">Recupere uma lista de todos os objetos de escola.</span><span class="sxs-lookup"><span data-stu-id="99bb5-104">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="99bb5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="99bb5-105">Permissions</span></span>

<span data-ttu-id="99bb5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99bb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99bb5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99bb5-108">Permission type</span></span>                        | <span data-ttu-id="99bb5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99bb5-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="99bb5-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99bb5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="99bb5-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="99bb5-111">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="99bb5-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99bb5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99bb5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99bb5-113">Not supported.</span></span>                              |
| <span data-ttu-id="99bb5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99bb5-114">Application</span></span>                            | <span data-ttu-id="99bb5-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99bb5-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99bb5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99bb5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http GET /education/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="99bb5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="99bb5-117">Optional query parameters</span></span>

<span data-ttu-id="99bb5-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="99bb5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99bb5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99bb5-119">Request headers</span></span>

| <span data-ttu-id="99bb5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99bb5-120">Header</span></span>        | <span data-ttu-id="99bb5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="99bb5-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="99bb5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="99bb5-122">Authorization</span></span> | <span data-ttu-id="99bb5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99bb5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99bb5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99bb5-125">Request body</span></span>

<span data-ttu-id="99bb5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99bb5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99bb5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="99bb5-127">Response</span></span>

<span data-ttu-id="99bb5-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99bb5-128">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99bb5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99bb5-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="99bb5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99bb5-130">Request</span></span>

<span data-ttu-id="99bb5-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="99bb5-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="99bb5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="99bb5-132">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="99bb5-133">C#</span><span class="sxs-lookup"><span data-stu-id="99bb5-133">C#</span></span>](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="99bb5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99bb5-134">JavaScript</span></span>](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="99bb5-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99bb5-135">Objective-C</span></span>](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="99bb5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="99bb5-136">Response</span></span>

<span data-ttu-id="99bb5-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="99bb5-137">The following is an example of the response.</span></span>

><span data-ttu-id="99bb5-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99bb5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
