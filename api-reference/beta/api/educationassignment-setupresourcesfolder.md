---
title: 'educationAssignment: setUpResourcesFolder'
description: Crie uma SharePoint para carregar arquivos para um determinado educationAssignment.
localization_priority: Normal
author: sharmas
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5ca3d7d267551bdeebb7a34a1624a4f1a4caea3f
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107610"
---
# <a name="educationassignment-setupresourcesfolder"></a><span data-ttu-id="d3e7e-103">educationAssignment: setUpResourcesFolder</span><span class="sxs-lookup"><span data-stu-id="d3e7e-103">educationAssignment: setUpResourcesFolder</span></span>

<span data-ttu-id="d3e7e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3e7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3e7e-105">Crie uma SharePoint para carregar arquivos para um [determinado educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d3e7e-105">Create a SharePoint folder to upload files for a given [educationAssignment](../resources/educationassignment.md).</span></span> 

<span data-ttu-id="d3e7e-106">O professor determina os recursos a carregar na pasta da atribuição.</span><span class="sxs-lookup"><span data-stu-id="d3e7e-106">The teacher determines the resources to upload in the assignment's folder.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d3e7e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3e7e-107">Permissions</span></span>
<span data-ttu-id="d3e7e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3e7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3e7e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3e7e-110">Permission type</span></span>      | <span data-ttu-id="d3e7e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3e7e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3e7e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3e7e-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="d3e7e-113">EduAssignments.ReadBasic, EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="d3e7e-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="d3e7e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3e7e-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d3e7e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3e7e-115">Not supported.</span></span>  |
|<span data-ttu-id="d3e7e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3e7e-116">Application</span></span> | <span data-ttu-id="d3e7e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3e7e-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d3e7e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3e7e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/setUpResourcesFolder
```
## <a name="request-headers"></a><span data-ttu-id="d3e7e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e7e-119">Request headers</span></span>
| <span data-ttu-id="d3e7e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3e7e-120">Header</span></span>       | <span data-ttu-id="d3e7e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d3e7e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d3e7e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3e7e-122">Authorization</span></span>  | <span data-ttu-id="d3e7e-p102">`{token}` de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3e7e-p102">Bearer `{token}`. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d3e7e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e7e-125">Request body</span></span>
<span data-ttu-id="d3e7e-126">Você precisa fornecer um json vazio `{}` como corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="d3e7e-126">You need to provide an empty json `{}` as request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d3e7e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3e7e-127">Response</span></span>
<span data-ttu-id="d3e7e-128">Se tiver êxito, este método retornará um código de resposta 200 Ok e um [objeto educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3e7e-128">If successful, this method returns a 200 Ok response code and [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) object in the request body.</span></span>

## <a name="example"></a><span data-ttu-id="d3e7e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3e7e-129">Example</span></span>
<span data-ttu-id="d3e7e-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d3e7e-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d3e7e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e7e-131">Request</span></span>
<span data-ttu-id="d3e7e-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3e7e-132">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d3e7e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3e7e-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d3e7e-134">C#</span><span class="sxs-lookup"><span data-stu-id="d3e7e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-setupresourcesfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3e7e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3e7e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-setupresourcesfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3e7e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3e7e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-setupresourcesfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3e7e-137">Java</span><span class="sxs-lookup"><span data-stu-id="d3e7e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-setupresourcesfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---
### <a name="response"></a><span data-ttu-id="d3e7e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3e7e-138">Response</span></span>
<span data-ttu-id="d3e7e-139">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="d3e7e-139">The following is an example of a response.</span></span> 

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

