---
title: Obter educationAssignmentResource
description: 'Obter as propriedades de um recurso específico em uma atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2fee9fdb2a1dd692608c1e7339fec015792d9b52
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436106"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="381e9-103">Obter educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="381e9-103">Get educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="381e9-104">Obter as propriedades de um recurso específico em uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="381e9-104">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="381e9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="381e9-105">Permissions</span></span>
<span data-ttu-id="381e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="381e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="381e9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="381e9-108">Permission type</span></span>      | <span data-ttu-id="381e9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="381e9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="381e9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="381e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="381e9-111">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="381e9-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="381e9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="381e9-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="381e9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="381e9-113">Not supported.</span></span>  |
|<span data-ttu-id="381e9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="381e9-114">Application</span></span> |  <span data-ttu-id="381e9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="381e9-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="381e9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="381e9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="381e9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="381e9-117">Optional query parameters</span></span>
<span data-ttu-id="381e9-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="381e9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="381e9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="381e9-119">Request headers</span></span>
| <span data-ttu-id="381e9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="381e9-120">Header</span></span>       | <span data-ttu-id="381e9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="381e9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="381e9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="381e9-122">Authorization</span></span>  | <span data-ttu-id="381e9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="381e9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="381e9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="381e9-125">Request body</span></span>
<span data-ttu-id="381e9-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="381e9-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="381e9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="381e9-127">Response</span></span>
<span data-ttu-id="381e9-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="381e9-128">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="381e9-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="381e9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="381e9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="381e9-130">Request</span></span>
<span data-ttu-id="381e9-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="381e9-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="381e9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="381e9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="381e9-133">C#</span><span class="sxs-lookup"><span data-stu-id="381e9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="381e9-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="381e9-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="381e9-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="381e9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="381e9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="381e9-136">Response</span></span>
<span data-ttu-id="381e9-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="381e9-137">The following is an example of the response.</span></span> 

><span data-ttu-id="381e9-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="381e9-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="381e9-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="381e9-139">All of the properties will be returned from an actual call.</span></span>

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
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "createdDateTime": "2014-01-01T00:00:00Z",
    "displayName": "Excel workbook 1",
    "lastModifiedBy": {
      "user": {
        "displayName": "Susana Rocha",
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
