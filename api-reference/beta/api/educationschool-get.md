---
title: Obter educationSchool
description: Recupere as propriedades e relações do objeto de escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4be7ac1de38a1c27f8ecfdaf7baf66e8dedf0a31
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955145"
---
# <a name="get-educationschool"></a><span data-ttu-id="56daa-103">Obter educationSchool</span><span class="sxs-lookup"><span data-stu-id="56daa-103">Get educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56daa-104">Recupere as propriedades e relações do objeto de escola.</span><span class="sxs-lookup"><span data-stu-id="56daa-104">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="56daa-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="56daa-105">Permissions</span></span>
<span data-ttu-id="56daa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56daa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56daa-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56daa-108">Permission type</span></span>      | <span data-ttu-id="56daa-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56daa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56daa-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56daa-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="56daa-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="56daa-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="56daa-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56daa-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="56daa-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56daa-113">Not supported.</span></span>  |
|<span data-ttu-id="56daa-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56daa-114">Application</span></span> | <span data-ttu-id="56daa-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56daa-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="56daa-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56daa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="56daa-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="56daa-117">Optional query parameters</span></span>
<span data-ttu-id="56daa-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="56daa-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56daa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56daa-119">Request headers</span></span>
| <span data-ttu-id="56daa-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56daa-120">Header</span></span>       | <span data-ttu-id="56daa-121">Valor</span><span class="sxs-lookup"><span data-stu-id="56daa-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="56daa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="56daa-122">Authorization</span></span>  | <span data-ttu-id="56daa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56daa-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="56daa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56daa-125">Request body</span></span>
<span data-ttu-id="56daa-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56daa-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="56daa-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="56daa-127">Response</span></span>
<span data-ttu-id="56daa-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56daa-128">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56daa-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56daa-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56daa-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56daa-130">Request</span></span>
<span data-ttu-id="56daa-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="56daa-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="56daa-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="56daa-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10001
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="56daa-133">C#</span><span class="sxs-lookup"><span data-stu-id="56daa-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56daa-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="56daa-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="56daa-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="56daa-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="56daa-136">Java</span><span class="sxs-lookup"><span data-stu-id="56daa-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="56daa-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="56daa-137">Response</span></span>
<span data-ttu-id="56daa-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="56daa-138">The following is an example of the response.</span></span> 

><span data-ttu-id="56daa-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56daa-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
