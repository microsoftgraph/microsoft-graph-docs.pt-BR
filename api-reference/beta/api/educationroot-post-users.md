---
title: Criar educationUser
description: Crie um novo usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 589fb34d12ed40ce248444d1e534871cd8d7861f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007474"
---
# <a name="create-educationuser"></a><span data-ttu-id="72685-103">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="72685-103">Create educationUser</span></span>

<span data-ttu-id="72685-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="72685-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72685-105">Crie um novo usuário.</span><span class="sxs-lookup"><span data-stu-id="72685-105">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="72685-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="72685-106">Permissions</span></span>
<span data-ttu-id="72685-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72685-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72685-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72685-109">Permission type</span></span>      | <span data-ttu-id="72685-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72685-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72685-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72685-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="72685-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72685-112">Not supported.</span></span>  |
|<span data-ttu-id="72685-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72685-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="72685-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72685-114">Not supported.</span></span>  |
|<span data-ttu-id="72685-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72685-115">Application</span></span> | <span data-ttu-id="72685-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72685-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="72685-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72685-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="72685-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72685-118">Request headers</span></span>
| <span data-ttu-id="72685-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72685-119">Header</span></span>       | <span data-ttu-id="72685-120">Valor</span><span class="sxs-lookup"><span data-stu-id="72685-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="72685-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="72685-121">Authorization</span></span>  | <span data-ttu-id="72685-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72685-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="72685-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72685-124">Content-Type</span></span>  | <span data-ttu-id="72685-125">application/json</span><span class="sxs-lookup"><span data-stu-id="72685-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="72685-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72685-126">Request body</span></span>
<span data-ttu-id="72685-127">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="72685-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="72685-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="72685-128">Response</span></span>
<span data-ttu-id="72685-129">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72685-129">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72685-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72685-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72685-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72685-131">Request</span></span>
<span data-ttu-id="72685-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="72685-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72685-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="72685-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="72685-134">C#</span><span class="sxs-lookup"><span data-stu-id="72685-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72685-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72685-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72685-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72685-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="72685-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="72685-137">Response</span></span>
<span data-ttu-id="72685-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="72685-138">The following is an example of the response.</span></span> 

><span data-ttu-id="72685-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72685-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


