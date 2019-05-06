---
title: Obter educationUser
description: Recupere as propriedades e as relações de um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8beaf8d3f8a6a63f5950773f6815348676fdca15
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587293"
---
# <a name="get-educationuser"></a><span data-ttu-id="c9d30-103">Obter educationUser</span><span class="sxs-lookup"><span data-stu-id="c9d30-103">Get educationUser</span></span>

<span data-ttu-id="c9d30-104">Recupere as propriedades e as relações de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c9d30-104">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9d30-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9d30-105">Permissions</span></span>
<span data-ttu-id="c9d30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9d30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9d30-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9d30-108">Permission type</span></span>      | <span data-ttu-id="c9d30-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9d30-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9d30-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9d30-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c9d30-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="c9d30-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="c9d30-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9d30-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c9d30-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9d30-113">Not supported.</span></span>  |
|<span data-ttu-id="c9d30-114">Application</span><span class="sxs-lookup"><span data-stu-id="c9d30-114">Application</span></span> | <span data-ttu-id="c9d30-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9d30-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="c9d30-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9d30-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c9d30-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c9d30-117">Optional query parameters</span></span>
<span data-ttu-id="c9d30-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c9d30-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9d30-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9d30-119">Request headers</span></span>
| <span data-ttu-id="c9d30-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9d30-120">Header</span></span>       | <span data-ttu-id="c9d30-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c9d30-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c9d30-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9d30-122">Authorization</span></span>  | <span data-ttu-id="c9d30-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9d30-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c9d30-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9d30-125">Request body</span></span>
<span data-ttu-id="c9d30-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9d30-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c9d30-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9d30-127">Response</span></span>
<span data-ttu-id="c9d30-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9d30-128">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c9d30-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9d30-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9d30-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9d30-130">Request</span></span>
<span data-ttu-id="c9d30-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9d30-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="c9d30-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9d30-132">Response</span></span>
<span data-ttu-id="c9d30-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c9d30-133">The following is an example of the response.</span></span> 

><span data-ttu-id="c9d30-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9d30-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c9d30-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c9d30-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c9d30-137">Basic</span><span class="sxs-lookup"><span data-stu-id="c9d30-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_educationuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9d30-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9d30-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_educationuser-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationuser-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationuser-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
