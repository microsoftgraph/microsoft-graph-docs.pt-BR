---
title: Criar educationSchool
description: Crie uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 26c21ecb75ba1962a45320810d2babb52cfe4b3d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275058"
---
# <a name="create-educationschool"></a><span data-ttu-id="e67b0-103">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="e67b0-103">Create educationSchool</span></span>

<span data-ttu-id="e67b0-104">Crie uma escola.</span><span class="sxs-lookup"><span data-stu-id="e67b0-104">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="e67b0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e67b0-105">Permissions</span></span>
<span data-ttu-id="e67b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e67b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e67b0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e67b0-108">Permission type</span></span>      | <span data-ttu-id="e67b0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e67b0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e67b0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e67b0-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e67b0-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e67b0-111">Not supported.</span></span>  |
|<span data-ttu-id="e67b0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e67b0-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e67b0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e67b0-113">Not supported.</span></span>  |
|<span data-ttu-id="e67b0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e67b0-114">Application</span></span> | <span data-ttu-id="e67b0-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e67b0-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e67b0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e67b0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```
## <a name="request-headers"></a><span data-ttu-id="e67b0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e67b0-117">Request headers</span></span>
| <span data-ttu-id="e67b0-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e67b0-118">Header</span></span>       | <span data-ttu-id="e67b0-119">Valor</span><span class="sxs-lookup"><span data-stu-id="e67b0-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e67b0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e67b0-120">Authorization</span></span>  | <span data-ttu-id="e67b0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e67b0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e67b0-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e67b0-123">Content-Type</span></span>  | <span data-ttu-id="e67b0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e67b0-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e67b0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e67b0-125">Request body</span></span>
<span data-ttu-id="e67b0-126">No corpo da solicitação, forneça uma representação JSON de um objeto [educationSchool](../resources/educationschool.md).</span><span class="sxs-lookup"><span data-stu-id="e67b0-126">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="e67b0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e67b0-127">Response</span></span>
<span data-ttu-id="e67b0-128">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e67b0-128">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e67b0-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e67b0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e67b0-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e67b0-130">Request</span></span>
<span data-ttu-id="e67b0-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e67b0-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools
Content-type: application/json
Content-length: 292

{
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
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102",
}
```

##### <a name="response"></a><span data-ttu-id="e67b0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e67b0-132">Response</span></span>
<span data-ttu-id="e67b0-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e67b0-133">The following is an example of the response.</span></span> 

><span data-ttu-id="e67b0-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e67b0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 292

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
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102",
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e67b0-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e67b0-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e67b0-137">C#</span><span class="sxs-lookup"><span data-stu-id="e67b0-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_educationschool_from_educationroot-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e67b0-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="e67b0-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_educationschool_from_educationroot-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e67b0-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e67b0-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_educationschool_from_educationroot-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationroot-post-schools.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/educationroot-post-schools.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationroot-post-schools.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
