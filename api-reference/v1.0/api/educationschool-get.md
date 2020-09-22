---
title: Obter educationSchool
description: Recupere as propriedades e relações do objeto de escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: dc3f1f2855e060abeab7cb7bd30a4bccd292144c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063726"
---
# <a name="get-educationschool"></a><span data-ttu-id="86130-103">Obter educationSchool</span><span class="sxs-lookup"><span data-stu-id="86130-103">Get educationSchool</span></span>

<span data-ttu-id="86130-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86130-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86130-105">Recupere as propriedades e relações do objeto de escola.</span><span class="sxs-lookup"><span data-stu-id="86130-105">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="86130-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="86130-106">Permissions</span></span>
<span data-ttu-id="86130-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86130-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86130-109">Permission type</span></span>      | <span data-ttu-id="86130-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86130-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86130-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86130-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="86130-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="86130-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="86130-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86130-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="86130-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86130-114">Not supported.</span></span>  |
|<span data-ttu-id="86130-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86130-115">Application</span></span> | <span data-ttu-id="86130-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86130-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="86130-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86130-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="86130-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="86130-118">Optional query parameters</span></span>
<span data-ttu-id="86130-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="86130-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86130-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86130-120">Request headers</span></span>
| <span data-ttu-id="86130-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86130-121">Header</span></span>       | <span data-ttu-id="86130-122">Valor</span><span class="sxs-lookup"><span data-stu-id="86130-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="86130-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="86130-123">Authorization</span></span>  | <span data-ttu-id="86130-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86130-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86130-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86130-126">Request body</span></span>
<span data-ttu-id="86130-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86130-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="86130-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="86130-128">Response</span></span>
<span data-ttu-id="86130-129">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86130-129">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="86130-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86130-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86130-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86130-131">Request</span></span>
<span data-ttu-id="86130-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="86130-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="86130-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="86130-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
# <a name="c"></a>[<span data-ttu-id="86130-134">C#</span><span class="sxs-lookup"><span data-stu-id="86130-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86130-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86130-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86130-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86130-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86130-137">Java</span><span class="sxs-lookup"><span data-stu-id="86130-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="86130-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="86130-138">Response</span></span>
<span data-ttu-id="86130-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="86130-139">The following is an example of the response.</span></span> 

><span data-ttu-id="86130-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86130-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

