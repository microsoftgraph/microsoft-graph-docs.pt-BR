---
title: Criar educationAssignment
description: 'Cria uma nova atribuição. Somente professores em uma classe podem criar uma atribuição. Iniciam o atribuições no estado de rascunho, o que significa que os alunos não verá a atribuição até que publicar seja chamado.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f86c6c3cc94ada7865038a0e8ae4aff90285719e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950155"
---
# <a name="create-educationassignment"></a><span data-ttu-id="7fb35-105">Criar educationAssignment</span><span class="sxs-lookup"><span data-stu-id="7fb35-105">Create educationAssignment</span></span>

> <span data-ttu-id="7fb35-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7fb35-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fb35-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7fb35-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7fb35-108">Cria uma nova atribuição.</span><span class="sxs-lookup"><span data-stu-id="7fb35-108">Creates a new assignment.</span></span> <span data-ttu-id="7fb35-109">Somente professores em uma classe podem criar uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="7fb35-109">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="7fb35-110">Iniciam o atribuições no estado de rascunho, o que significa que os alunos não verá a atribuição até que publicar seja chamado.</span><span class="sxs-lookup"><span data-stu-id="7fb35-110">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="7fb35-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="7fb35-111">Permissions</span></span>
<span data-ttu-id="7fb35-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fb35-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fb35-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fb35-114">Permission type</span></span>      | <span data-ttu-id="7fb35-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7fb35-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fb35-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fb35-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="7fb35-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7fb35-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="7fb35-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fb35-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7fb35-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fb35-119">Not supported.</span></span>  |
|<span data-ttu-id="7fb35-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fb35-120">Application</span></span> | <span data-ttu-id="7fb35-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fb35-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7fb35-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fb35-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments

```
## <a name="request-headers"></a><span data-ttu-id="7fb35-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fb35-123">Request headers</span></span>
| <span data-ttu-id="7fb35-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7fb35-124">Header</span></span>       | <span data-ttu-id="7fb35-125">Valor</span><span class="sxs-lookup"><span data-stu-id="7fb35-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7fb35-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fb35-126">Authorization</span></span>  | <span data-ttu-id="7fb35-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fb35-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7fb35-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7fb35-129">Content-Type</span></span>  | <span data-ttu-id="7fb35-130">application/json</span><span class="sxs-lookup"><span data-stu-id="7fb35-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7fb35-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fb35-131">Request body</span></span>
<span data-ttu-id="7fb35-132">No corpo da solicitação, fornece uma representação JSON de um objeto [educationAssignment](../resources/educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7fb35-132">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="7fb35-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fb35-133">Response</span></span>
<span data-ttu-id="7fb35-134">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fb35-134">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fb35-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fb35-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7fb35-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fb35-136">Request</span></span>
<span data-ttu-id="7fb35-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fb35-137">The following is an example of the request.</span></span>
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
      "contentType": "Text",
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
<span data-ttu-id="7fb35-138">No corpo da solicitação, fornece uma representação JSON de um objeto [educationAssignment](../resources/educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7fb35-138">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="7fb35-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fb35-139">Response</span></span>
<span data-ttu-id="7fb35-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7fb35-140">The following is an example of the response.</span></span> 

><span data-ttu-id="7fb35-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fb35-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "contentType": "Text",
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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
