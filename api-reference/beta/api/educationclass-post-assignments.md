---
title: Criar educationAssignment
description: 'Cria uma nova atribuição. Somente professores em uma classe podem criar uma atribuição. As atribuições começam no estado de rascunho, o que significa que os alunos não verão a atribuição até que Publish seja chamado.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f00a31619e13bcae54565bab6fbfae9d0fdb937a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007620"
---
# <a name="create-educationassignment"></a><span data-ttu-id="2a66f-105">Criar educationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a66f-105">Create educationAssignment</span></span>

<span data-ttu-id="2a66f-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a66f-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a66f-107">Cria uma nova atribuição.</span><span class="sxs-lookup"><span data-stu-id="2a66f-107">Creates a new assignment.</span></span> <span data-ttu-id="2a66f-108">Somente professores em uma classe podem criar uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="2a66f-108">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="2a66f-109">As atribuições começam no estado de rascunho, o que significa que os alunos não verão a atribuição até que Publish seja chamado.</span><span class="sxs-lookup"><span data-stu-id="2a66f-109">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="2a66f-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a66f-110">Permissions</span></span>
<span data-ttu-id="2a66f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a66f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a66f-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a66f-113">Permission type</span></span>      | <span data-ttu-id="2a66f-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a66f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a66f-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a66f-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="2a66f-116">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a66f-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="2a66f-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a66f-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2a66f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a66f-118">Not supported.</span></span>  |
|<span data-ttu-id="2a66f-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a66f-119">Application</span></span> | <span data-ttu-id="2a66f-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a66f-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2a66f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a66f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments

```
## <a name="request-headers"></a><span data-ttu-id="2a66f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a66f-122">Request headers</span></span>
| <span data-ttu-id="2a66f-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a66f-123">Header</span></span>       | <span data-ttu-id="2a66f-124">Valor</span><span class="sxs-lookup"><span data-stu-id="2a66f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2a66f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a66f-125">Authorization</span></span>  | <span data-ttu-id="2a66f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a66f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2a66f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a66f-128">Content-Type</span></span>  | <span data-ttu-id="2a66f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="2a66f-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a66f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a66f-130">Request body</span></span>
<span data-ttu-id="2a66f-131">No corpo da solicitação, forneça uma representação JSON de um objeto [educationAssignment](../resources/educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2a66f-131">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="2a66f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a66f-132">Response</span></span>
<span data-ttu-id="2a66f-133">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a66f-133">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a66f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a66f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a66f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a66f-135">Request</span></span>
<span data-ttu-id="2a66f-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a66f-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationassignment_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11019/assignments
Content-type: application/json
Content-length: 279

{ 
  "dueDateTime": "2014-02-01T00:00:00Z",
  "displayName": "Midterm 1",
    "instructions":  {
      "contentType": "text",
      "content": "Read chapters 1 through 3"
    },
      "grading": {
        "@odata.type": "#microsoft.education.assignments.api.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "assignTo": {
        "@odata.type": "#microsoft.education.assignments.api.educationAssignmentClassRecipient"
      },
      "status":"draft",
      "allowStudentsToAddResourcesToSubmission": true
}
```
<span data-ttu-id="2a66f-137">No corpo da solicitação, forneça uma representação JSON de um objeto [educationAssignment](../resources/educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2a66f-137">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="2a66f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a66f-138">Response</span></span>
<span data-ttu-id="2a66f-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2a66f-139">The following is an example of the response.</span></span> 

><span data-ttu-id="2a66f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a66f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 279

{
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "2014-02-01T00:00:00Z",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "2014-02-01T00:00:00Z",
  "classId": "11018",
  "closeDateTime": "2014-02-11T00:00:00Z",
  "createdBy": {
      "application": null,
      "device": null,
      "user": {
          "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
          "displayName": null
      }
  },
  "createdDateTime": "2014-02-01T00:00:00Z",
  "displayName": "published",
  "dueDateTime": "2014-02-01T00:00:00Z",
  "grading": {
    "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
    "maxPoints": 100
  },
  "instructions": {
    "contentType": "text",
    "content": "Read chapters 1 through 3"
  },
  "lastModifiedBy": {
      "application": null,
      "device": null,
      "user": {
          "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
          "displayName": null
      }
  },
  "lastModifiedDateTime": "2014-02-01T00:00:00Z",
  "status": "published"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


