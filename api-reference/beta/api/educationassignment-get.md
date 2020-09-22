---
title: Obter educationAssignment
description: " os professores podem ver todas as atribuições em uma classe."
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2c819e89e918ffbd2f460c88ce9668ce5062dde9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007802"
---
# <a name="get-educationassignment"></a><span data-ttu-id="c6761-103">Obter educationAssignment</span><span class="sxs-lookup"><span data-stu-id="c6761-103">Get educationAssignment</span></span>

<span data-ttu-id="c6761-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6761-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6761-105">Obtenha as propriedades e os relacionamentos de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="c6761-105">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="c6761-106">Os alunos só podem ver as atribuições atribuídas a eles; os professores podem ver todas as atribuições em uma classe.</span><span class="sxs-lookup"><span data-stu-id="c6761-106">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6761-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6761-107">Permissions</span></span>
<span data-ttu-id="c6761-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6761-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c6761-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6761-110">Permission type</span></span>      | <span data-ttu-id="c6761-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6761-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6761-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6761-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c6761-113">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6761-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="c6761-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6761-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c6761-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6761-115">Not supported.</span></span>  |
|<span data-ttu-id="c6761-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6761-116">Application</span></span> | <span data-ttu-id="c6761-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6761-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="c6761-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6761-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c6761-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c6761-119">Optional query parameters</span></span>
<span data-ttu-id="c6761-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c6761-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6761-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6761-121">Request headers</span></span>
| <span data-ttu-id="c6761-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6761-122">Header</span></span>       | <span data-ttu-id="c6761-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c6761-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c6761-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6761-124">Authorization</span></span>  | <span data-ttu-id="c6761-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6761-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c6761-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6761-127">Request body</span></span>
<span data-ttu-id="c6761-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6761-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6761-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6761-129">Response</span></span>
<span data-ttu-id="c6761-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6761-130">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6761-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6761-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6761-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6761-132">Request</span></span>
<span data-ttu-id="c6761-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6761-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="c6761-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6761-134">Response</span></span>
<span data-ttu-id="c6761-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c6761-135">The following is an example of the response.</span></span> 

><span data-ttu-id="c6761-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6761-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "closeDateTime": "2014-01-11T00:00:00Z",
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
  "suppressions": []
}
-->


