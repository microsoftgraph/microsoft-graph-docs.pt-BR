---
title: 'educationAssignment: setUpResourcesFolder'
description: Crie uma SharePoint para carregar arquivos para um determinado educationAssignment.
localization_priority: Normal
author: sharmas
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b46e50f2756705e2698ca50fb804e864072a2faa
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912196"
---
# <a name="educationassignment-setupresourcesfolder"></a><span data-ttu-id="884a1-103">educationAssignment: setUpResourcesFolder</span><span class="sxs-lookup"><span data-stu-id="884a1-103">educationAssignment: setUpResourcesFolder</span></span>

<span data-ttu-id="884a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="884a1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="884a1-105">Crie uma SharePoint para carregar arquivos para um [determinado educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="884a1-105">Create a SharePoint folder to upload files for a given [educationAssignment](../resources/educationassignment.md).</span></span> 

<span data-ttu-id="884a1-106">O professor determina os recursos a carregar na pasta da atribuição.</span><span class="sxs-lookup"><span data-stu-id="884a1-106">The teacher determines the resources to upload in the assignment's folder.</span></span> 

## <a name="permissions"></a><span data-ttu-id="884a1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="884a1-107">Permissions</span></span>
<span data-ttu-id="884a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="884a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="884a1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="884a1-110">Permission type</span></span>      | <span data-ttu-id="884a1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="884a1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="884a1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="884a1-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="884a1-113">EduAssignments.ReadBasic, EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="884a1-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="884a1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="884a1-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="884a1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="884a1-115">Not supported.</span></span>  |
|<span data-ttu-id="884a1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="884a1-116">Application</span></span> | <span data-ttu-id="884a1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="884a1-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="884a1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="884a1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/setUpResourcesFolder
```
## <a name="request-headers"></a><span data-ttu-id="884a1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="884a1-119">Request headers</span></span>
| <span data-ttu-id="884a1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="884a1-120">Header</span></span>       | <span data-ttu-id="884a1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="884a1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="884a1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="884a1-122">Authorization</span></span>  | <span data-ttu-id="884a1-p102">`{token}` de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="884a1-p102">Bearer `{token}`. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="884a1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="884a1-125">Request body</span></span>
<span data-ttu-id="884a1-126">Você precisa fornecer um json vazio `{}` como corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="884a1-126">You need to provide an empty json `{}` as request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="884a1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="884a1-127">Response</span></span>
<span data-ttu-id="884a1-128">Se tiver êxito, este método retornará um código de resposta 200 Ok e um [objeto educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="884a1-128">If successful, this method returns a 200 Ok response code and [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) object in the request body.</span></span>

## <a name="example"></a><span data-ttu-id="884a1-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="884a1-129">Example</span></span>
<span data-ttu-id="884a1-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="884a1-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="884a1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="884a1-131">Request</span></span>
<span data-ttu-id="884a1-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="884a1-132">The following is an example of a request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "educationassignment_setupresourcesfolder"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/education/classes/d38ffdea-da93-46ac-90ba-d568c6073075/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/setUpResourcesFolder
Content-type: application/json

{
}
```

### <a name="response"></a><span data-ttu-id="884a1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="884a1-133">Response</span></span>
<span data-ttu-id="884a1-134">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="884a1-134">The following is an example of a response.</span></span> 

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

