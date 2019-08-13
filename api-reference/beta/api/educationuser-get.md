---
title: Obter educationUser
description: Recupere as propriedades e as relações de um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e1ea282d4a9eef36ff399bb498bb8eb06b5a7a1f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326608"
---
# <a name="get-educationuser"></a><span data-ttu-id="477da-103">Obter educationUser</span><span class="sxs-lookup"><span data-stu-id="477da-103">Get educationUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="477da-104">Recupere as propriedades e as relações de um usuário.</span><span class="sxs-lookup"><span data-stu-id="477da-104">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="477da-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="477da-105">Permissions</span></span>
<span data-ttu-id="477da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="477da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="477da-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="477da-108">Permission type</span></span>      | <span data-ttu-id="477da-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="477da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="477da-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="477da-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="477da-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="477da-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="477da-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="477da-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="477da-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="477da-113">Not supported.</span></span>  |
|<span data-ttu-id="477da-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="477da-114">Application</span></span> | <span data-ttu-id="477da-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="477da-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="477da-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="477da-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="477da-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="477da-117">Optional query parameters</span></span>
<span data-ttu-id="477da-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="477da-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="477da-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="477da-119">Request headers</span></span>
| <span data-ttu-id="477da-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="477da-120">Header</span></span>       | <span data-ttu-id="477da-121">Valor</span><span class="sxs-lookup"><span data-stu-id="477da-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="477da-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="477da-122">Authorization</span></span>  | <span data-ttu-id="477da-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="477da-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="477da-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="477da-125">Request body</span></span>
<span data-ttu-id="477da-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="477da-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="477da-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="477da-127">Response</span></span>
<span data-ttu-id="477da-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="477da-128">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="477da-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="477da-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="477da-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="477da-130">Request</span></span>
<span data-ttu-id="477da-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="477da-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="477da-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="477da-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```http
GET https://graph.microsoft.com/beta/education/users/13012
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="477da-133">C#</span><span class="sxs-lookup"><span data-stu-id="477da-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="477da-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="477da-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="477da-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="477da-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="477da-136">Java</span><span class="sxs-lookup"><span data-stu-id="477da-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="477da-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="477da-137">Response</span></span>
<span data-ttu-id="477da-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="477da-138">The following is an example of the response.</span></span> 

><span data-ttu-id="477da-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="477da-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
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
  },
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
