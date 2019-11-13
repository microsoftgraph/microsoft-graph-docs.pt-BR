---
title: Listar educationSchools
description: Recupere uma lista de todos os objetos de escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ac9e0e8d493ca9b4ea6d2c7a86bac274e9243896
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302975"
---
# <a name="list-educationschools"></a><span data-ttu-id="df37c-103">Listar educationSchools</span><span class="sxs-lookup"><span data-stu-id="df37c-103">List educationSchools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df37c-104">Recupere uma lista de todos os objetos de escola.</span><span class="sxs-lookup"><span data-stu-id="df37c-104">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="df37c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="df37c-105">Permissions</span></span>

<span data-ttu-id="df37c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df37c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df37c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df37c-108">Permission type</span></span>                        | <span data-ttu-id="df37c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df37c-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="df37c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df37c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="df37c-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="df37c-111">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="df37c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df37c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df37c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df37c-113">Not supported.</span></span>                              |
| <span data-ttu-id="df37c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df37c-114">Application</span></span>                            | <span data-ttu-id="df37c-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df37c-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df37c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df37c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http 
GET /education/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="df37c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="df37c-117">Optional query parameters</span></span>

<span data-ttu-id="df37c-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="df37c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df37c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df37c-119">Request headers</span></span>

| <span data-ttu-id="df37c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df37c-120">Header</span></span>        | <span data-ttu-id="df37c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="df37c-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="df37c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="df37c-122">Authorization</span></span> | <span data-ttu-id="df37c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df37c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df37c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df37c-125">Request body</span></span>

<span data-ttu-id="df37c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df37c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df37c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="df37c-127">Response</span></span>

<span data-ttu-id="df37c-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df37c-128">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df37c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df37c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="df37c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df37c-130">Request</span></span>

<span data-ttu-id="df37c-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df37c-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="df37c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="df37c-132">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="df37c-133">C#</span><span class="sxs-lookup"><span data-stu-id="df37c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df37c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df37c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="df37c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df37c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="df37c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="df37c-136">Response</span></span>

<span data-ttu-id="df37c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df37c-137">The following is an example of the response.</span></span>

><span data-ttu-id="df37c-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df37c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
