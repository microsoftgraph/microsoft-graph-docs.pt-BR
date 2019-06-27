---
title: Obter educationSchool
description: Recupere as propriedades e relações do objeto de escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d85f5d038ae201d5ab8b53332a3e2f0ae9677630
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278201"
---
# <a name="get-educationschool"></a><span data-ttu-id="a0a56-103">Obter educationSchool</span><span class="sxs-lookup"><span data-stu-id="a0a56-103">Get educationSchool</span></span>

<span data-ttu-id="a0a56-104">Recupere as propriedades e relações do objeto de escola.</span><span class="sxs-lookup"><span data-stu-id="a0a56-104">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0a56-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0a56-105">Permissions</span></span>
<span data-ttu-id="a0a56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0a56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0a56-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0a56-108">Permission type</span></span>      | <span data-ttu-id="a0a56-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0a56-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0a56-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0a56-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a0a56-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a0a56-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="a0a56-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0a56-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a0a56-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0a56-113">Not supported.</span></span>  |
|<span data-ttu-id="a0a56-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0a56-114">Application</span></span> | <span data-ttu-id="a0a56-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0a56-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a0a56-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0a56-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a0a56-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0a56-117">Optional query parameters</span></span>
<span data-ttu-id="a0a56-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a0a56-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0a56-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0a56-119">Request headers</span></span>
| <span data-ttu-id="a0a56-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0a56-120">Header</span></span>       | <span data-ttu-id="a0a56-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a0a56-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0a56-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0a56-122">Authorization</span></span>  | <span data-ttu-id="a0a56-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0a56-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0a56-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0a56-125">Request body</span></span>
<span data-ttu-id="a0a56-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0a56-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a0a56-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0a56-127">Response</span></span>
<span data-ttu-id="a0a56-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0a56-128">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a0a56-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0a56-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0a56-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0a56-130">Request</span></span>
<span data-ttu-id="a0a56-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0a56-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
##### <a name="response"></a><span data-ttu-id="a0a56-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0a56-132">Response</span></span>
<span data-ttu-id="a0a56-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a0a56-133">The following is an example of the response.</span></span> 

><span data-ttu-id="a0a56-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0a56-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "principalEmail": "AmyRoebuck@contoso.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "lowestGrade": "9",
  "highestGrade": "12"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a0a56-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a0a56-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a0a56-137">C#</span><span class="sxs-lookup"><span data-stu-id="a0a56-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_educationschool-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0a56-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="a0a56-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_educationschool-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a0a56-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a0a56-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_educationschool-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationschool-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/educationschool-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationschool-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
