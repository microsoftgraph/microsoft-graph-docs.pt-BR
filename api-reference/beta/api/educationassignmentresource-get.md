---
title: Obter educationAssignmentResource
description: 'Obter as propriedades de um recurso específico em uma atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1e2cfc389cdb40f73d688cf93a4e9d1a88eede5a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427239"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="20559-103">Obter educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="20559-103">Get educationAssignmentResource</span></span>

<span data-ttu-id="20559-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="20559-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20559-105">Obter as propriedades de um recurso específico em uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="20559-105">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="20559-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20559-106">Permissions</span></span>
<span data-ttu-id="20559-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20559-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20559-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20559-109">Permission type</span></span>      | <span data-ttu-id="20559-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20559-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20559-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20559-111">Delegated (work or school account)</span></span> | <span data-ttu-id="20559-112">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20559-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="20559-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20559-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="20559-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20559-114">Not supported.</span></span>  |
|<span data-ttu-id="20559-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20559-115">Application</span></span> |  <span data-ttu-id="20559-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20559-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="20559-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20559-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="20559-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="20559-118">Optional query parameters</span></span>
<span data-ttu-id="20559-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="20559-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20559-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20559-120">Request headers</span></span>
| <span data-ttu-id="20559-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20559-121">Header</span></span>       | <span data-ttu-id="20559-122">Valor</span><span class="sxs-lookup"><span data-stu-id="20559-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="20559-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="20559-123">Authorization</span></span>  | <span data-ttu-id="20559-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20559-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="20559-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20559-126">Request body</span></span>
<span data-ttu-id="20559-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20559-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="20559-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="20559-128">Response</span></span>
<span data-ttu-id="20559-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20559-129">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="20559-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20559-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20559-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20559-131">Request</span></span>
<span data-ttu-id="20559-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="20559-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20559-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="20559-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="c"></a>[<span data-ttu-id="20559-134">C#</span><span class="sxs-lookup"><span data-stu-id="20559-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20559-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20559-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20559-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20559-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="20559-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="20559-137">Response</span></span>
<span data-ttu-id="20559-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20559-138">The following is an example of the response.</span></span> 

><span data-ttu-id="20559-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="20559-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="20559-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20559-140">All of the properties will be returned from an actual call.</span></span>

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
