---
title: 'educationAssignment: setUpResourcesFolder'
description: Crie uma SharePoint para carregar arquivos para um determinado educationAssignment.
localization_priority: Normal
author: sharmas
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 99b876655f5b2e5006a738d9401434015b804373
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703451"
---
# <a name="educationassignment-setupresourcesfolder"></a><span data-ttu-id="16c5e-103">educationAssignment: setUpResourcesFolder</span><span class="sxs-lookup"><span data-stu-id="16c5e-103">educationAssignment: setUpResourcesFolder</span></span>

<span data-ttu-id="16c5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16c5e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16c5e-105">Crie uma SharePoint para carregar arquivos para um [determinado educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="16c5e-105">Create a SharePoint folder to upload files for a given [educationAssignment](../resources/educationassignment.md).</span></span> 

<span data-ttu-id="16c5e-106">O professor determina os recursos a carregar na pasta da atribuição.</span><span class="sxs-lookup"><span data-stu-id="16c5e-106">The teacher determines the resources to upload in the assignment's folder.</span></span> 

## <a name="permissions"></a><span data-ttu-id="16c5e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="16c5e-107">Permissions</span></span>
<span data-ttu-id="16c5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16c5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16c5e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16c5e-110">Permission type</span></span>      | <span data-ttu-id="16c5e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16c5e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16c5e-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16c5e-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="16c5e-113">EduAssignments.ReadBasic, EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="16c5e-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="16c5e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16c5e-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="16c5e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16c5e-115">Not supported.</span></span>  |
|<span data-ttu-id="16c5e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16c5e-116">Application</span></span> | <span data-ttu-id="16c5e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16c5e-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="16c5e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16c5e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/setUpResourcesFolder

```
## <a name="request-headers"></a><span data-ttu-id="16c5e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16c5e-119">Request headers</span></span>
| <span data-ttu-id="16c5e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16c5e-120">Header</span></span>       | <span data-ttu-id="16c5e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="16c5e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="16c5e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="16c5e-122">Authorization</span></span>  | <span data-ttu-id="16c5e-p102">`{token}` de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16c5e-p102">Bearer `{token}`. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="16c5e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16c5e-125">Request body</span></span>
<span data-ttu-id="16c5e-126">Você precisa fornecer um json vazio `{}` como corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="16c5e-126">You need to provide an empty json `{}` as request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="16c5e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="16c5e-127">Response</span></span>
<span data-ttu-id="16c5e-128">Se tiver êxito, este método retornará um código de resposta 200 Ok e um [objeto educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16c5e-128">If successful, this method returns a 200 Ok response code and [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) object in the request body.</span></span>

## <a name="example"></a><span data-ttu-id="16c5e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16c5e-129">Example</span></span>
<span data-ttu-id="16c5e-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="16c5e-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="16c5e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16c5e-131">Request</span></span>
<span data-ttu-id="16c5e-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="16c5e-132">The following is an example of a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationassignment_setupresourcesfolder"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/setUpResourcesFolder
Content-type: application/json

{
}
```
---
### <a name="response"></a><span data-ttu-id="16c5e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="16c5e-133">Response</span></span>
<span data-ttu-id="16c5e-134">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="16c5e-134">The following is an example of a response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('955e0bd5-52c2-41ad-b7e8-5b33a18c5e78')/assignments/$entity",
    "classId": "955e0bd5-52c2-41ad-b7e8-5b33a18c5e78",
    "displayName": "Unit 3 Essay",
    "closeDateTime": "2021-04-06T00:00:00Z",
    "dueDateTime": "2021-04-05T00:00:00Z",
    "assignDateTime": "2021-04-01T00:00:00Z",
    "assignedDateTime": null,
    "allowLateSubmissions": true,
    "createdDateTime": "2021-03-04T00:02:31.9834674Z",
    "lastModifiedDateTime": "2021-03-04T00:02:32.0954032Z",
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "draft",
    "notificationChannelUrl": null,
    "addedStudentAction": "assignIfOpen",
    "addToCalendarAction": "studentsAndTeamOwners",
    "id": "18d17255-3278-49fb-8da7-d095b7f610c4",
    "instructions": {
        "content": "Upload a 500 word essay about the theme of nature in a Shakespearean sonnet.",
        "contentType": "text"
    },
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
    },
    "assignTo": {
        "@odata.type": "#microsoft.graph.educationAssignmentIndividualRecipient",
        "recipients": [
            "42ff222c-571f-497c-a9d3-f77ea9ece327"
        ]
    },
    "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!H0Unq6KJREmMLHgbJXfKw4YTuh2luKRDvUVGQBLOmvaRxxvbedZKT4LKslSIjT9a/items/01SMYGQ3IUCDNLBJ4XCFE3AQMQHTLSLVYX",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
            "displayName": null
        }
    },
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
            "displayName": null
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

