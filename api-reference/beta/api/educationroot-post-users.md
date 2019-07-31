---
title: Criar educationUser
description: Crie um novo usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 376dddf5b875ae4164698f0f7d77aed3b6af43f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955226"
---
# <a name="create-educationuser"></a><span data-ttu-id="ba916-103">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="ba916-103">Create educationUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba916-104">Crie um novo usuário.</span><span class="sxs-lookup"><span data-stu-id="ba916-104">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="ba916-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba916-105">Permissions</span></span>
<span data-ttu-id="ba916-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba916-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba916-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba916-108">Permission type</span></span>      | <span data-ttu-id="ba916-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba916-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba916-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba916-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ba916-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba916-111">Not supported.</span></span>  |
|<span data-ttu-id="ba916-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba916-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ba916-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba916-113">Not supported.</span></span>  |
|<span data-ttu-id="ba916-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba916-114">Application</span></span> | <span data-ttu-id="ba916-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba916-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ba916-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba916-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="ba916-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba916-117">Request headers</span></span>
| <span data-ttu-id="ba916-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba916-118">Header</span></span>       | <span data-ttu-id="ba916-119">Valor</span><span class="sxs-lookup"><span data-stu-id="ba916-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ba916-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba916-120">Authorization</span></span>  | <span data-ttu-id="ba916-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba916-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ba916-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba916-123">Content-Type</span></span>  | <span data-ttu-id="ba916-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ba916-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba916-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba916-125">Request body</span></span>
<span data-ttu-id="ba916-126">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="ba916-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ba916-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba916-127">Response</span></span>
<span data-ttu-id="ba916-128">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba916-128">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba916-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba916-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba916-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba916-130">Request</span></span>
<span data-ttu-id="ba916-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba916-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ba916-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba916-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/users
Content-type: application/json
Content-length: 508

{
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
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ba916-133">C#</span><span class="sxs-lookup"><span data-stu-id="ba916-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba916-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="ba916-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ba916-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ba916-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ba916-136">Java</span><span class="sxs-lookup"><span data-stu-id="ba916-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ba916-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba916-137">Response</span></span>
<span data-ttu-id="ba916-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ba916-138">The following is an example of the response.</span></span> 

><span data-ttu-id="ba916-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba916-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 508

{
  "id": "13012",
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": " ",
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
