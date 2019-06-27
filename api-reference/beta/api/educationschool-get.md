---
title: Obter educationSchool
description: Recupere as propriedades e relações do objeto de escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2a15b92ab9d99219638cb09bee40a78043e9693f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259658"
---
# <a name="get-educationschool"></a><span data-ttu-id="1bfb3-103">Obter educationSchool</span><span class="sxs-lookup"><span data-stu-id="1bfb3-103">Get educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bfb3-104">Recupere as propriedades e relações do objeto de escola.</span><span class="sxs-lookup"><span data-stu-id="1bfb3-104">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bfb3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1bfb3-105">Permissions</span></span>
<span data-ttu-id="1bfb3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bfb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bfb3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bfb3-108">Permission type</span></span>      | <span data-ttu-id="1bfb3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1bfb3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bfb3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bfb3-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1bfb3-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="1bfb3-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="1bfb3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bfb3-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1bfb3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bfb3-113">Not supported.</span></span>  |
|<span data-ttu-id="1bfb3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bfb3-114">Application</span></span> | <span data-ttu-id="1bfb3-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bfb3-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1bfb3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bfb3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1bfb3-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1bfb3-117">Optional query parameters</span></span>
<span data-ttu-id="1bfb3-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1bfb3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1bfb3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bfb3-119">Request headers</span></span>
| <span data-ttu-id="1bfb3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1bfb3-120">Header</span></span>       | <span data-ttu-id="1bfb3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1bfb3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1bfb3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bfb3-122">Authorization</span></span>  | <span data-ttu-id="1bfb3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bfb3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1bfb3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bfb3-125">Request body</span></span>
<span data-ttu-id="1bfb3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1bfb3-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1bfb3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bfb3-127">Response</span></span>
<span data-ttu-id="1bfb3-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bfb3-128">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1bfb3-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bfb3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bfb3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bfb3-130">Request</span></span>
<span data-ttu-id="1bfb3-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bfb3-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10001
```
##### <a name="response"></a><span data-ttu-id="1bfb3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bfb3-132">Response</span></span>
<span data-ttu-id="1bfb3-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1bfb3-133">The following is an example of the response.</span></span> 

><span data-ttu-id="1bfb3-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bfb3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "schoolPrincipalEmail": "AmyRoebuck@contoso.com",
  "schoolPrincipalName": "Amy Roebuck",
  "externalSchoolPrincipalId": "14007",
  "lowestGrade": "9",
  "highestGrade": "12"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1bfb3-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1bfb3-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1bfb3-137">C#</span><span class="sxs-lookup"><span data-stu-id="1bfb3-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_educationschool-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1bfb3-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="1bfb3-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_educationschool-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1bfb3-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1bfb3-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_educationschool-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationschool-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationschool-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationschool-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
