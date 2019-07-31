---
title: Criar educationSchool
description: Crie uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 19e374bdbb9a0fdc083d817a3c54917de2c55641
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955247"
---
# <a name="create-educationschool"></a><span data-ttu-id="64611-103">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="64611-103">Create educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64611-104">Crie uma escola.</span><span class="sxs-lookup"><span data-stu-id="64611-104">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="64611-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="64611-105">Permissions</span></span>
<span data-ttu-id="64611-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64611-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64611-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64611-108">Permission type</span></span>      | <span data-ttu-id="64611-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64611-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64611-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64611-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="64611-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64611-111">Not supported.</span></span>  |
|<span data-ttu-id="64611-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64611-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="64611-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64611-113">Not supported.</span></span>  |
|<span data-ttu-id="64611-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64611-114">Application</span></span> | <span data-ttu-id="64611-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64611-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="64611-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64611-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```
## <a name="request-headers"></a><span data-ttu-id="64611-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64611-117">Request headers</span></span>
| <span data-ttu-id="64611-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64611-118">Header</span></span>       | <span data-ttu-id="64611-119">Valor</span><span class="sxs-lookup"><span data-stu-id="64611-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64611-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="64611-120">Authorization</span></span>  | <span data-ttu-id="64611-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64611-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="64611-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64611-123">Content-Type</span></span>  | <span data-ttu-id="64611-124">application/json</span><span class="sxs-lookup"><span data-stu-id="64611-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64611-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64611-125">Request body</span></span>
<span data-ttu-id="64611-126">No corpo da solicitação, forneça uma representação JSON de um objeto [educationSchool](../resources/educationschool.md).</span><span class="sxs-lookup"><span data-stu-id="64611-126">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="64611-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="64611-127">Response</span></span>
<span data-ttu-id="64611-128">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64611-128">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64611-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64611-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64611-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64611-130">Request</span></span>
<span data-ttu-id="64611-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64611-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="64611-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="64611-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="64611-133">C#</span><span class="sxs-lookup"><span data-stu-id="64611-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationschool-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64611-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="64611-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationschool-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="64611-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="64611-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationschool-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="64611-136">Java</span><span class="sxs-lookup"><span data-stu-id="64611-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationschool-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="64611-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="64611-137">Response</span></span>
<span data-ttu-id="64611-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64611-138">The following is an example of the response.</span></span> 

><span data-ttu-id="64611-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64611-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
