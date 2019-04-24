---
title: Criar educationAssignment
description: 'Cria uma nova atribuição. Somente professores em uma classe podem criar uma atribuição. As atribuições começam no estado de rascunho, o que significa que os alunos não verão a atribuição até que Publish seja chamado.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: bac79b8f85eb6141b5159ac5dc7acbf067bf571c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457792"
---
# <a name="create-educationassignment"></a><span data-ttu-id="29c23-105">Criar educationAssignment</span><span class="sxs-lookup"><span data-stu-id="29c23-105">Create educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29c23-106">Cria uma nova atribuição.</span><span class="sxs-lookup"><span data-stu-id="29c23-106">Creates a new assignment.</span></span> <span data-ttu-id="29c23-107">Somente professores em uma classe podem criar uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="29c23-107">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="29c23-108">As atribuições começam no estado de rascunho, o que significa que os alunos não verão a atribuição até que Publish seja chamado.</span><span class="sxs-lookup"><span data-stu-id="29c23-108">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="29c23-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="29c23-109">Permissions</span></span>
<span data-ttu-id="29c23-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29c23-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29c23-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29c23-112">Permission type</span></span>      | <span data-ttu-id="29c23-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29c23-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29c23-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29c23-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="29c23-115">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29c23-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="29c23-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29c23-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="29c23-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29c23-117">Not supported.</span></span>  |
|<span data-ttu-id="29c23-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29c23-118">Application</span></span> | <span data-ttu-id="29c23-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29c23-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="29c23-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29c23-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments

```
## <a name="request-headers"></a><span data-ttu-id="29c23-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29c23-121">Request headers</span></span>
| <span data-ttu-id="29c23-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29c23-122">Header</span></span>       | <span data-ttu-id="29c23-123">Valor</span><span class="sxs-lookup"><span data-stu-id="29c23-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="29c23-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="29c23-124">Authorization</span></span>  | <span data-ttu-id="29c23-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29c23-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="29c23-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29c23-127">Content-Type</span></span>  | <span data-ttu-id="29c23-128">application/json</span><span class="sxs-lookup"><span data-stu-id="29c23-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29c23-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29c23-129">Request body</span></span>
<span data-ttu-id="29c23-130">No corpo da solicitação, forneça uma representação JSON de um objeto [educationAssignment](../resources/educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="29c23-130">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="29c23-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="29c23-131">Response</span></span>
<span data-ttu-id="29c23-132">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29c23-132">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29c23-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29c23-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29c23-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29c23-134">Request</span></span>
<span data-ttu-id="29c23-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="29c23-135">The following is an example of the request.</span></span>
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
<span data-ttu-id="29c23-136">No corpo da solicitação, forneça uma representação JSON de um objeto [educationAssignment](../resources/educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="29c23-136">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="29c23-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="29c23-137">Response</span></span>
<span data-ttu-id="29c23-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="29c23-138">The following is an example of the response.</span></span> 

><span data-ttu-id="29c23-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29c23-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-post-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
