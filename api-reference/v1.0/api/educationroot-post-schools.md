---
title: Criar educationSchool
description: Crie uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: cf4feff3a8071a337be443038534928f5d8a0986
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075354"
---
# <a name="create-educationschool"></a><span data-ttu-id="d2655-103">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="d2655-103">Create educationSchool</span></span>

<span data-ttu-id="d2655-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2655-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2655-105">Crie uma escola.</span><span class="sxs-lookup"><span data-stu-id="d2655-105">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2655-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2655-106">Permissions</span></span>

<span data-ttu-id="d2655-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2655-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2655-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2655-109">Permission type</span></span>                        | <span data-ttu-id="d2655-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2655-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d2655-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2655-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2655-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2655-112">Not supported.</span></span>                              |
| <span data-ttu-id="d2655-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2655-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2655-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2655-114">Not supported.</span></span>                              |
| <span data-ttu-id="d2655-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2655-115">Application</span></span>                            | <span data-ttu-id="d2655-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2655-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="d2655-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2655-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```

## <a name="request-headers"></a><span data-ttu-id="d2655-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2655-118">Request headers</span></span>

| <span data-ttu-id="d2655-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2655-119">Header</span></span>        | <span data-ttu-id="d2655-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d2655-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="d2655-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2655-121">Authorization</span></span> | <span data-ttu-id="d2655-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2655-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2655-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2655-124">Content-Type</span></span>  | <span data-ttu-id="d2655-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2655-125">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="d2655-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2655-126">Request body</span></span>

<span data-ttu-id="d2655-127">No corpo da solicitação, forneça uma representação JSON de um objeto [educationSchool](../resources/educationschool.md).</span><span class="sxs-lookup"><span data-stu-id="d2655-127">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d2655-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2655-128">Response</span></span>

<span data-ttu-id="d2655-129">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2655-129">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2655-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2655-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d2655-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2655-131">Request</span></span>

<span data-ttu-id="d2655-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2655-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2655-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2655-133">HTTP</span></span>](#tab/http)

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
  "phone": "+1 (253) 555-0102",
}
```

# <a name="c"></a>[<span data-ttu-id="d2655-134">C#</span><span class="sxs-lookup"><span data-stu-id="d2655-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationschool-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2655-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2655-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationschool-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2655-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2655-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationschool-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2655-137">Java</span><span class="sxs-lookup"><span data-stu-id="d2655-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationschool-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d2655-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2655-138">Response</span></span>

<span data-ttu-id="d2655-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d2655-139">The following is an example of the response.</span></span>

><span data-ttu-id="d2655-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2655-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "phone": "+1 (253) 555-0102",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

