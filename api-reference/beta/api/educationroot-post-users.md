---
title: Criar educationUser
description: Crie um novo usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 18ced2a58fa4974ddca18bfc5b31d3e5e39fb46c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043581"
---
# <a name="create-educationuser"></a><span data-ttu-id="cbb7c-103">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="cbb7c-103">Create educationUser</span></span>

<span data-ttu-id="cbb7c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbb7c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbb7c-105">Crie um novo usuário.</span><span class="sxs-lookup"><span data-stu-id="cbb7c-105">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="cbb7c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbb7c-106">Permissions</span></span>
<span data-ttu-id="cbb7c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbb7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbb7c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbb7c-109">Permission type</span></span>      | <span data-ttu-id="cbb7c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbb7c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbb7c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbb7c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="cbb7c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbb7c-112">Not supported.</span></span>  |
|<span data-ttu-id="cbb7c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbb7c-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cbb7c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbb7c-114">Not supported.</span></span>  |
|<span data-ttu-id="cbb7c-115">Application</span><span class="sxs-lookup"><span data-stu-id="cbb7c-115">Application</span></span> | <span data-ttu-id="cbb7c-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbb7c-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cbb7c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbb7c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="cbb7c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbb7c-118">Request headers</span></span>
| <span data-ttu-id="cbb7c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cbb7c-119">Header</span></span>       | <span data-ttu-id="cbb7c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cbb7c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cbb7c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbb7c-121">Authorization</span></span>  | <span data-ttu-id="cbb7c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbb7c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cbb7c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cbb7c-124">Content-Type</span></span>  | <span data-ttu-id="cbb7c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cbb7c-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cbb7c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbb7c-126">Request body</span></span>
<span data-ttu-id="cbb7c-127">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="cbb7c-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="cbb7c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbb7c-128">Response</span></span>
<span data-ttu-id="cbb7c-129">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbb7c-129">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbb7c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbb7c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbb7c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbb7c-131">Request</span></span>
<span data-ttu-id="cbb7c-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbb7c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cbb7c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbb7c-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cbb7c-134">C#</span><span class="sxs-lookup"><span data-stu-id="cbb7c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cbb7c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cbb7c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cbb7c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cbb7c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cbb7c-137">Java</span><span class="sxs-lookup"><span data-stu-id="cbb7c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cbb7c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbb7c-138">Response</span></span>
<span data-ttu-id="cbb7c-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cbb7c-139">The following is an example of the response.</span></span> 

><span data-ttu-id="cbb7c-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cbb7c-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


