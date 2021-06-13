---
title: Criar educationAssignment
description: Crie uma nova atribuição.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c15bca046a08b62ff9a3d6cc75631e6a9110ef34
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911778"
---
# <a name="create-educationassignment"></a><span data-ttu-id="c0612-103">Criar educationAssignment</span><span class="sxs-lookup"><span data-stu-id="c0612-103">Create educationAssignment</span></span>

<span data-ttu-id="c0612-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0612-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0612-105">Crie uma nova atribuição.</span><span class="sxs-lookup"><span data-stu-id="c0612-105">Create a new assignment.</span></span> 

<span data-ttu-id="c0612-106">Somente professores em uma classe podem criar uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="c0612-106">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="c0612-107">As atribuições começam no estado Rascunho, o que significa que os alunos não verão a atribuição até a publicação.</span><span class="sxs-lookup"><span data-stu-id="c0612-107">Assignments start in the Draft state, which means that students will not see the assignment until publication.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0612-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0612-108">Permissions</span></span>
<span data-ttu-id="c0612-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0612-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0612-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0612-111">Permission type</span></span>      | <span data-ttu-id="c0612-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0612-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0612-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0612-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="c0612-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0612-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c0612-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0612-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c0612-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0612-116">Not supported.</span></span>  |
|<span data-ttu-id="c0612-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0612-117">Application</span></span> | <span data-ttu-id="c0612-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0612-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c0612-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0612-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments
```
## <a name="request-headers"></a><span data-ttu-id="c0612-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0612-120">Request headers</span></span>
| <span data-ttu-id="c0612-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0612-121">Header</span></span>       | <span data-ttu-id="c0612-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c0612-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c0612-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0612-123">Authorization</span></span>  | <span data-ttu-id="c0612-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0612-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c0612-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0612-126">Content-Type</span></span>  | <span data-ttu-id="c0612-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c0612-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0612-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0612-128">Request body</span></span>
<span data-ttu-id="c0612-129">No corpo da solicitação, fornece uma representação JSON de um [objeto educationAssignment.](../resources/educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c0612-129">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="c0612-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0612-130">Response</span></span>
<span data-ttu-id="c0612-131">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0612-131">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0612-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0612-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0612-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0612-133">Request</span></span>
<span data-ttu-id="c0612-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0612-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="c0612-135">No corpo da solicitação, fornece uma representação JSON de um [objeto educationAssignment.](../resources/educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c0612-135">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="c0612-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0612-136">Response</span></span>
<span data-ttu-id="c0612-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c0612-137">The following is an example of the response.</span></span> 

><span data-ttu-id="c0612-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c0612-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 279

{
  "addedStudentAction": "none",
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
  "notificationChannelUrl": null,
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


