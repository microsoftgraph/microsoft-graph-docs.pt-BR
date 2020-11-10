---
title: Obter educationAssignmentResource
description: 'Obter as propriedades de um recurso específico em uma atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b8c899ffa30354fadaa4c2d25ad3e2e9a020346c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966437"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="10435-103">Obter educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="10435-103">Get educationAssignmentResource</span></span>

<span data-ttu-id="10435-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10435-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10435-105">Obter as propriedades de um recurso específico em uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="10435-105">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="10435-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="10435-106">Permissions</span></span>
<span data-ttu-id="10435-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10435-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10435-109">Permission type</span></span>      | <span data-ttu-id="10435-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10435-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10435-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10435-111">Delegated (work or school account)</span></span> | <span data-ttu-id="10435-112">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10435-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="10435-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10435-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="10435-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10435-114">Not supported.</span></span>  |
|<span data-ttu-id="10435-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10435-115">Application</span></span> |  <span data-ttu-id="10435-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10435-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="10435-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10435-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="10435-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="10435-118">Optional query parameters</span></span>
<span data-ttu-id="10435-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="10435-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10435-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10435-120">Request headers</span></span>
| <span data-ttu-id="10435-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10435-121">Header</span></span>       | <span data-ttu-id="10435-122">Valor</span><span class="sxs-lookup"><span data-stu-id="10435-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="10435-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="10435-123">Authorization</span></span>  | <span data-ttu-id="10435-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10435-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="10435-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10435-126">Request body</span></span>
<span data-ttu-id="10435-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10435-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="10435-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="10435-128">Response</span></span>
<span data-ttu-id="10435-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10435-129">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10435-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10435-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10435-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10435-131">Request</span></span>
<span data-ttu-id="10435-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="10435-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="10435-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="10435-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="c"></a>[<span data-ttu-id="10435-134">C#</span><span class="sxs-lookup"><span data-stu-id="10435-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10435-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10435-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10435-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10435-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10435-137">Java</span><span class="sxs-lookup"><span data-stu-id="10435-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="10435-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="10435-138">Response</span></span>
<span data-ttu-id="10435-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="10435-139">The following is an example of the response.</span></span> 

><span data-ttu-id="10435-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="10435-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="10435-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10435-141">All of the properties will be returned from an actual call.</span></span>

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
