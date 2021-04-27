---
title: Criar educationSchool
description: Crie uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0f4d91dc8756f74551a374151946d192ecf18b27
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043637"
---
# <a name="create-educationschool"></a><span data-ttu-id="64e88-103">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="64e88-103">Create educationSchool</span></span>

<span data-ttu-id="64e88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64e88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64e88-105">Crie uma escola.</span><span class="sxs-lookup"><span data-stu-id="64e88-105">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="64e88-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="64e88-106">Permissions</span></span>

<span data-ttu-id="64e88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64e88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64e88-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64e88-109">Permission type</span></span>                        | <span data-ttu-id="64e88-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64e88-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="64e88-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64e88-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="64e88-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64e88-112">Not supported.</span></span>                              |
| <span data-ttu-id="64e88-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64e88-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64e88-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64e88-114">Not supported.</span></span>                              |
| <span data-ttu-id="64e88-115">Application</span><span class="sxs-lookup"><span data-stu-id="64e88-115">Application</span></span>                            | <span data-ttu-id="64e88-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64e88-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="64e88-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64e88-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```

## <a name="request-headers"></a><span data-ttu-id="64e88-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64e88-118">Request headers</span></span>

| <span data-ttu-id="64e88-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64e88-119">Header</span></span>        | <span data-ttu-id="64e88-120">Valor</span><span class="sxs-lookup"><span data-stu-id="64e88-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="64e88-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="64e88-121">Authorization</span></span> | <span data-ttu-id="64e88-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64e88-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64e88-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64e88-124">Content-Type</span></span>  | <span data-ttu-id="64e88-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64e88-125">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="64e88-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64e88-126">Request body</span></span>

<span data-ttu-id="64e88-127">No corpo da solicitação, forneça uma representação JSON de um objeto [educationSchool](../resources/educationschool.md).</span><span class="sxs-lookup"><span data-stu-id="64e88-127">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="64e88-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="64e88-128">Response</span></span>

<span data-ttu-id="64e88-129">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64e88-129">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64e88-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64e88-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="64e88-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64e88-131">Request</span></span>

<span data-ttu-id="64e88-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64e88-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64e88-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="64e88-133">HTTP</span></span>](#tab/http)

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
  "phone": "+1 (253) 555-0102",
}
```

# <a name="c"></a>[<span data-ttu-id="64e88-134">C#</span><span class="sxs-lookup"><span data-stu-id="64e88-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationschool-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64e88-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64e88-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationschool-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64e88-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64e88-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationschool-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="64e88-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="64e88-137">Response</span></span>

<span data-ttu-id="64e88-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64e88-138">The following is an example of the response.</span></span>

><span data-ttu-id="64e88-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="64e88-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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


