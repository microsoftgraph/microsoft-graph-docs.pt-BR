---
title: Obter educationAssignment
description: " professores podem ver todas as atribuições em uma classe."
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: eba959dcaf2478f3c49fc0fbb434d7269e37e5ba
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508367"
---
# <a name="get-educationassignment"></a><span data-ttu-id="5bbd1-103">Obter educationAssignment</span><span class="sxs-lookup"><span data-stu-id="5bbd1-103">Get educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bbd1-104">Obtenha as propriedades e relacionamentos de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-104">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="5bbd1-105">Alunos só podem ver atribuições atribuídas a eles; professores podem ver todas as atribuições em uma classe.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-105">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bbd1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5bbd1-106">Permissions</span></span>
<span data-ttu-id="5bbd1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bbd1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5bbd1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bbd1-109">Permission type</span></span>      | <span data-ttu-id="5bbd1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5bbd1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bbd1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bbd1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5bbd1-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5bbd1-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="5bbd1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bbd1-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5bbd1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-114">Not supported.</span></span>  |
|<span data-ttu-id="5bbd1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bbd1-115">Application</span></span> | <span data-ttu-id="5bbd1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="5bbd1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bbd1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5bbd1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5bbd1-118">Optional query parameters</span></span>
<span data-ttu-id="5bbd1-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bbd1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bbd1-120">Request headers</span></span>
| <span data-ttu-id="5bbd1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5bbd1-121">Header</span></span>       | <span data-ttu-id="5bbd1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5bbd1-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5bbd1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bbd1-123">Authorization</span></span>  | <span data-ttu-id="5bbd1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5bbd1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bbd1-126">Request body</span></span>
<span data-ttu-id="5bbd1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bbd1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bbd1-128">Response</span></span>
<span data-ttu-id="5bbd1-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-129">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5bbd1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bbd1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bbd1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bbd1-131">Request</span></span>
<span data-ttu-id="5bbd1-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="5bbd1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bbd1-133">Response</span></span>
<span data-ttu-id="5bbd1-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-134">The following is an example of the response.</span></span> 

><span data-ttu-id="5bbd1-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "id": "19002",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "classId": "11006",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "createdDateTime": "2014-01-01T00:00:00Z",
  "displayName": "Mid term exam",
  "dueDateTime": "2014-01-11T00:00:00Z",
  "grading": {
      "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType",
      "maxPoints": 100
  },
  "instructions": {
    "content": "Answer every question correctly",
    "contentType": "Text"
  },
  "lastModifiedBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "lastModifiedDateTime": "2014-01-01T00:00:00Z",
  "status": "assigned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
