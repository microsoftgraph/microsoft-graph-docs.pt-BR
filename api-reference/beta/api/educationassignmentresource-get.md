---
title: Obter educationAssignmentResource
description: 'Obter as propriedades de um recurso específico em uma atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 76d9ed55c4e914385ad6282e3bed6025ef5c6036
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457967"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="caad8-103">Obter educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="caad8-103">Get educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="caad8-104">Obter as propriedades de um recurso específico em uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="caad8-104">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="caad8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="caad8-105">Permissions</span></span>
<span data-ttu-id="caad8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caad8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caad8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="caad8-108">Permission type</span></span>      | <span data-ttu-id="caad8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="caad8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="caad8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="caad8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="caad8-111">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="caad8-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="caad8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="caad8-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="caad8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caad8-113">Not supported.</span></span>  |
|<span data-ttu-id="caad8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="caad8-114">Application</span></span> |  <span data-ttu-id="caad8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caad8-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="caad8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="caad8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="caad8-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="caad8-117">Optional query parameters</span></span>
<span data-ttu-id="caad8-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="caad8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="caad8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="caad8-119">Request headers</span></span>
| <span data-ttu-id="caad8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="caad8-120">Header</span></span>       | <span data-ttu-id="caad8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="caad8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="caad8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="caad8-122">Authorization</span></span>  | <span data-ttu-id="caad8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="caad8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="caad8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="caad8-125">Request body</span></span>
<span data-ttu-id="caad8-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="caad8-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="caad8-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="caad8-127">Response</span></span>
<span data-ttu-id="caad8-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="caad8-128">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="caad8-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="caad8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="caad8-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="caad8-130">Request</span></span>
<span data-ttu-id="caad8-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="caad8-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="caad8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="caad8-132">Response</span></span>
<span data-ttu-id="caad8-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="caad8-133">The following is an example of the response.</span></span> 

><span data-ttu-id="caad8-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="caad8-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="caad8-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="caad8-135">All of the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/educationassignmentresource-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
