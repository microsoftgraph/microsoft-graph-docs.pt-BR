---
title: 'educationAssignment: setUpFeedbackResourcesFolder'
description: Crie uma pasta do SharePoint para carregar arquivos de comentários para uma determinada educationSubmission.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ed6381c3b5c7a9f6cdc0013d1c520a05374f6910
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900541"
---
# <a name="educationassignment-setupfeedbackresourcesfolder"></a>educationAssignment: setUpFeedbackResourcesFolder

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie uma pasta do SharePoint para carregar arquivos de comentários para uma [determinada educationSubmission](../resources/educationsubmission.md).

O professor determina os recursos a serem carregados na pasta de recursos de comentários de um envio.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) |  EduAssignments.ReadBasic, EduAssignments.Read  |
|Delegada (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /classes/{classId}/assignments/{assignmentId}/setUpFeedbackResourcesFolder
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type   | application/json           |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça um objeto JSON vazio `{}` para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [educationAssignment](../resources/educationassignment.md) no corpo da solicitação.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "request",
  "sampleKeys": ["37d99af7-cfc5-4e3b-8566-f7d40e4a2070","a3cce0ba-2008-4c4d-bf62-079408562d96"],  
  "name": "educationassignment_setupfeedbackresourcesfolder"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/37d99af7-cfc5-4e3b-8566-f7d40e4a2070/assignments/a3cce0ba-2008-4c4d-bf62-079408562d96/setUpFeedbackResourcesFolder
Content-type: application/json

{
}
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#educationAssignment",
    "@odata.type": "#microsoft.graph.educationAssignment",
    "classId": "155c5142-1716-4c24-b2ac-cd1bcd8ad7ac",
    "displayName": "2022-02-25T18_57_26_443Z",
    "closeDateTime": null,
    "dueDateTime": "2022-02-25T18:57:26.443Z",
    "assignDateTime": null,
    "assignedDateTime": null,
    "allowLateSubmissions": true,
    "resourcesFolderUrl": null,
    "feedbackResourcesFolderUrl": "https://graph.microsoft.com/beta/drives/b!9i0vapy4v02vPa13nXvmLuPofkLptz5InpCzu0fn0IRzOBm8o5mJQbXuPddtkYG7/items/01PREZ76FARBTP25X74JFISOFAN7QAHOYW",
    "createdDateTime": "2022-02-24T18:57:27.8611453Z",
    "lastModifiedDateTime": "2022-02-24T18:57:40.5319603Z",
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "draft",
    "notificationChannelUrl": null,
    "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%22155c5142-1716-4c24-b2ac-cd1bcd8ad7ac%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%22d10f56f7-ba7e-4dfc-b5a2-ae9f10b0d1ad%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
    "addToCalendarAction": "none",
    "addedStudentAction": "none",
    "id": "d10f56f7-ba7e-4dfc-b5a2-ae9f10b0d1ad",
    "instructions": {
        "content": "2022-02-25T18_57_26_443Z",
        "contentType": "text"
    },
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
    },
    "assignTo": {
        "@odata.type": "#microsoft.graph.educationAssignmentClassRecipient"
    },
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "fadaae59-b18c-44d1-993f-fe8a281bd69c",
            "displayName": null
        }
    },
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "AAAAAAAA-0123-4567-89AB-1B4BB48C3119",
            "displayName": null
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2022-05-05 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: setUpFeedbackResourcesFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
