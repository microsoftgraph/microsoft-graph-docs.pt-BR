---
title: Obter educationAssignmentResource
description: 'Obter as propriedades de um recurso específico em uma atribuição.  '
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c8c28c86ad77a5274d79cd00da5c04806a31ec34
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992195"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="6af35-103">Obter educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="6af35-103">Get educationAssignmentResource</span></span>

<span data-ttu-id="6af35-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6af35-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6af35-105">Obter as propriedades de um recurso específico em uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="6af35-105">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="6af35-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6af35-106">Permissions</span></span>
<span data-ttu-id="6af35-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6af35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6af35-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6af35-109">Permission type</span></span>      | <span data-ttu-id="6af35-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6af35-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6af35-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6af35-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6af35-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6af35-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="6af35-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6af35-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6af35-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6af35-114">Not supported.</span></span>  |
|<span data-ttu-id="6af35-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6af35-115">Application</span></span> |  <span data-ttu-id="6af35-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6af35-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="6af35-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6af35-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6af35-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6af35-118">Optional query parameters</span></span>
<span data-ttu-id="6af35-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6af35-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6af35-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6af35-120">Request headers</span></span>
| <span data-ttu-id="6af35-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6af35-121">Header</span></span>       | <span data-ttu-id="6af35-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6af35-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6af35-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6af35-123">Authorization</span></span>  | <span data-ttu-id="6af35-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6af35-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6af35-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6af35-126">Request body</span></span>
<span data-ttu-id="6af35-127">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="6af35-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6af35-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6af35-128">Response</span></span>
<span data-ttu-id="6af35-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6af35-129">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6af35-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6af35-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="6af35-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6af35-131">Request</span></span>
<span data-ttu-id="6af35-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6af35-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6af35-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6af35-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```msgraph-interactive
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c
```
# <a name="c"></a>[<span data-ttu-id="6af35-134">C#</span><span class="sxs-lookup"><span data-stu-id="6af35-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6af35-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6af35-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6af35-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6af35-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6af35-137">Java</span><span class="sxs-lookup"><span data-stu-id="6af35-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6af35-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6af35-138">Response</span></span>
<span data-ttu-id="6af35-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6af35-139">The following is an example of the response.</span></span> 

><span data-ttu-id="6af35-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6af35-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 842

{
  "distributeForStudentWork": true,
  "id": "22002",
  "resource": {
    "createdBy": {
      "user": {
        "displayName": "Shawn Hughes",
        "id": "14012"
      },
    },
    "createdDateTime": "2014-01-01T00:00:00Z",
    "displayName": "Excel workbook 1",
    "lastModifiedBy": {
      "user": {
        "displayName": "Shawn Hughes",
        "id": "14012"
      },
    },
    "lastModifiedDateTime": "2014-01-01T00:00:00Z"
  }
}
    
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
