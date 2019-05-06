---
title: Obter educationAssignmentResource
description: 'Obter as propriedades de um recurso específico em uma atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 18d49ab13e124aebb596aacf5d48ef6f83e3a29b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587384"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="4dc29-103">Obter educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="4dc29-103">Get educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dc29-104">Obter as propriedades de um recurso específico em uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="4dc29-104">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="4dc29-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4dc29-105">Permissions</span></span>
<span data-ttu-id="4dc29-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dc29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dc29-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4dc29-108">Permission type</span></span>      | <span data-ttu-id="4dc29-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4dc29-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dc29-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4dc29-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4dc29-111">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4dc29-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="4dc29-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4dc29-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4dc29-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dc29-113">Not supported.</span></span>  |
|<span data-ttu-id="4dc29-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4dc29-114">Application</span></span> |  <span data-ttu-id="4dc29-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dc29-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4dc29-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4dc29-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4dc29-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4dc29-117">Optional query parameters</span></span>
<span data-ttu-id="4dc29-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4dc29-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4dc29-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4dc29-119">Request headers</span></span>
| <span data-ttu-id="4dc29-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4dc29-120">Header</span></span>       | <span data-ttu-id="4dc29-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4dc29-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4dc29-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4dc29-122">Authorization</span></span>  | <span data-ttu-id="4dc29-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4dc29-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4dc29-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4dc29-125">Request body</span></span>
<span data-ttu-id="4dc29-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4dc29-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4dc29-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dc29-127">Response</span></span>
<span data-ttu-id="4dc29-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4dc29-128">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4dc29-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4dc29-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4dc29-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4dc29-130">Request</span></span>
<span data-ttu-id="4dc29-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4dc29-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="4dc29-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dc29-132">Response</span></span>
<span data-ttu-id="4dc29-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4dc29-133">The following is an example of the response.</span></span> 

><span data-ttu-id="4dc29-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4dc29-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4dc29-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4dc29-135">All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4dc29-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4dc29-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4dc29-137">Basic</span><span class="sxs-lookup"><span data-stu-id="4dc29-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_educationassignmentresource-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4dc29-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4dc29-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_educationassignmentresource-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationassignmentresource-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationassignmentresource-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
