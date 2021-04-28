---
title: Obter educationAssignmentResource
description: 'Obter as propriedades de um recurso específico em uma atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f5446926a3161004de1f3a19b5896df95e34ca52
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061683"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="93aca-103">Obter educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="93aca-103">Get educationAssignmentResource</span></span>

<span data-ttu-id="93aca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93aca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93aca-105">Obter as propriedades de um recurso específico em uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="93aca-105">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="93aca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="93aca-106">Permissions</span></span>
<span data-ttu-id="93aca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93aca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93aca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93aca-109">Permission type</span></span>      | <span data-ttu-id="93aca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93aca-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93aca-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93aca-111">Delegated (work or school account)</span></span> | <span data-ttu-id="93aca-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93aca-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="93aca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93aca-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="93aca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93aca-114">Not supported.</span></span>  |
|<span data-ttu-id="93aca-115">Application\*</span><span class="sxs-lookup"><span data-stu-id="93aca-115">Application\*</span></span> |  <span data-ttu-id="93aca-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93aca-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  | 

<span data-ttu-id="93aca-117">\*As permissões de aplicativo estão disponíveis apenas para clientes de visualização privada.</span><span class="sxs-lookup"><span data-stu-id="93aca-117">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="93aca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93aca-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="93aca-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="93aca-119">Optional query parameters</span></span>
<span data-ttu-id="93aca-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="93aca-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93aca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93aca-121">Request headers</span></span>
| <span data-ttu-id="93aca-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93aca-122">Header</span></span>       | <span data-ttu-id="93aca-123">Valor</span><span class="sxs-lookup"><span data-stu-id="93aca-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93aca-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="93aca-124">Authorization</span></span>  | <span data-ttu-id="93aca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93aca-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93aca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93aca-127">Request body</span></span>
<span data-ttu-id="93aca-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93aca-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="93aca-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="93aca-129">Response</span></span>
<span data-ttu-id="93aca-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93aca-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93aca-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93aca-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93aca-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93aca-132">Request</span></span>
<span data-ttu-id="93aca-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93aca-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93aca-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="93aca-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="c"></a>[<span data-ttu-id="93aca-135">C#</span><span class="sxs-lookup"><span data-stu-id="93aca-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93aca-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93aca-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93aca-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93aca-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93aca-138">Java</span><span class="sxs-lookup"><span data-stu-id="93aca-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="93aca-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="93aca-139">Response</span></span>
<span data-ttu-id="93aca-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="93aca-140">The following is an example of the response.</span></span> 

><span data-ttu-id="93aca-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="93aca-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
