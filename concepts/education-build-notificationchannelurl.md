---
title: Especificar o canal padrão para notificações de atribuição de educação
description: Use a API de educação no Microsoft Graph para especificar o canal padrão do Microsoft Teams para enviar notificações sobre uma tarefa.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 392cfaeef8f4491204dcd6a1cba992ce7f07a092
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440905"
---
# <a name="specify-the-default-channel-for-education-assignment-notifications-using-the-microsoft-graph-api"></a>Especifique o canal padrão para notificações de atribuição de educação usando o Microsoft API do Graph

Este artigo descreve como usar a API de educação no Microsoft Graph para especificar o canal padrão do Microsoft Teams para enviar notificações sobre uma **tarefa**. Especificar o canal padrão envolve a criação da propriedade de cadeia de caracteres **notificationChannelUrl** para [um educationAssignment](/graph/api/resources/educationassignment). O valor padrão dessa propriedade é `null`.

## <a name="prerequisites"></a>Pré-requisitos

Antes de criar a propriedade, identifique a equipe correspondente para a atribuição e o nome do canal.

Para identificar a equipe para a tarefa, no menu à esquerda no Teams, clique em **Teams** e selecione a equipe apropriada.

![Captura de tela de uma equipe selecionada no elemento de navegação do Teams](./images/notificationchannel-team.png)

Identifique o canal apropriado dentro da equipe selecionada.

![Captura de tela de um canal selecionado em uma equipe](./images/notificationchannel-channel.png)

## <a name="build-the-notificationchannelurl-property-value"></a>Criar o valor da propriedade notificationChannelUrl

As etapas a seguir descrevem como criar o valor da propriedade.

### <a name="step-1---get-the-team-id-based-on-your-team-name"></a>Etapa 1 – Obter a ID da equipe com base no nome da sua equipe
Para localizar a ID da equipe, faça uma solicitação GET com o nome da equipe. Se você já tiver a ID da equipe, ignore esta etapa.

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra a solicitação.

```http
GET https://graph.microsoft.com/v1.0/teams?$filter=displayName eq 'English Fall ''21'
```

#### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta.

```http
HTTP/1.1 200 Ok
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams",
    "@odata.count": 1,
    "value": [
        {
            "id": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "createdDateTime": null,
            "displayName": "English Fall '21",
            "description": "English Fall '21",
            "internalId": null,
            "classification": null,
            "specialization": null,
            "visibility": null,
            "webUrl": null,
            "isArchived": null,
            "isMembershipLimitedToOwners": null,
            "memberSettings": null,
            "guestSettings": null,
            "messagingSettings": null,
            "funSettings": null,
            "discoverySettings": null
        }
    ]
}
```

### <a name="step-2---get-the-channel-id-based-on-channel-name-and-team-id"></a>Etapa 2 – Obter a ID do canal com base no nome do canal e na ID da equipe
Faça uma solicitação GET com a ID da equipe obtida na etapa anterior e o nome do canal. Ignore esta etapa se você já tiver a ID do canal.

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra a solicitação.

```http
GET https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels?$filter=displayName eq 'General'
```

#### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta.

```http
HTTP/1.1 200 Ok
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('72a7baec-c3e9-4213-a850-f62de0adad5f')/channels",
    "@odata.count": 1,
    "value": [
        {
            "id": "19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2",
            "createdDateTime": "2021-08-25T12:33:49.124Z",
            "displayName": "General",
            "description": "English Fall '21",
            "isFavoriteByDefault": null,
            "email": "",
            "webUrl": "https://teams.microsoft.com/l/channel/19%3Ajb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1%40thread.tacv2/General?groupId=72a7baec-c3e9-4213-a850-f62de0adad5f&tenantId=b6338c92-533e-4f6d-a327-994263712399",
            "membershipType": "standard"
        }
    ]
}
```

### <a name="step-3---construct-the-value-for-the-notificationchannelurl-property"></a>Etapa 3 – Construir o valor para a propriedade notificationChannelUrl
Crie o valor para a **propriedade notificationChannelUrl** usando o seguinte formato: 

> `https://graph.microsoft.com/v1.0/teams/{team-id}/channels/{channel-id}` 

Substitua os `{team-id}` espaços `{channel-id}` reservados e os valores descritos na tabela a seguir.

| Espaço reservado | Descrição | Exemplo |
|:--|:--|:--|
| `{team-id}` | A ID da equipe da resposta na etapa 1. Essa é a equipe à qual a atribuição atual pertence. | 72a7baec-c3e9-4213-a850-f62de0adad5f |
| `{channel-id}` | ID do item do corpo da resposta obtido na etapa 2. | 19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2 |

O exemplo a seguir mostra **um notificationChannelUrl** com base nesse formato.

```http
https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2
```

### <a name="step-4---assign-the-value-to-the-notificationchannelurl-property-for-the-assignment"></a>Etapa 4 – Atribuir o valor à propriedade notificationChannelUrl para a atribuição

Agora que você criou a URL com êxito, é hora de atribuir o valor à propriedade. Você pode executar essa operação atualizando os recursos **educationAssignment** ou **educationAssignmentDefaults** .

#### <a name="example-1-update-an-educationassignment"></a>Exemplo 1: atualizar um educationAssignment

##### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

```http
PATCH https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/4679bc1b-90c5-45af-ae1a-d5357672ed39
Content-type: application/json

{
    "displayName": "Property update",
    "notificationChannelUrl": "https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2"
}
```

##### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments/$entity",
    "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
    "displayName": "Property update",
    "closeDateTime": null,
    "dueDateTime": "2021-09-10T00:00:00Z",
    "assignDateTime": null,
    "assignedDateTime": null,
    "allowLateSubmissions": true,
    "resourcesFolderUrl": null,
    "createdDateTime": "2021-09-03T23:57:14.6088791Z",
    "lastModifiedDateTime": "2021-09-04T15:01:35.3361649Z",
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "draft",
    "notificationChannelUrl": "https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2",
    "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%224679bc1b-90c5-45af-ae1a-d5357672ed39%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
    "addToCalendarAction": "studentsAndPublisher",
    "addedStudentAction": "none",
    "id": "4679bc1b-90c5-45af-ae1a-d5357672ed39",
    "instructions": {
        "content": "Read chapter 5 and write your review",
        "contentType": "text"
    },
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 50
    },
    "assignTo": {
        "@odata.type": "#microsoft.graph.educationAssignmentClassRecipient"
    },
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
            "displayName": null
        }
    },
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
            "displayName": null
        }
    }
}
```

#### <a name="example-2-update-educationassignmentdefaults"></a>Exemplo 2: Atualizar educationAssignmentDefaults

##### <a name="request"></a>Solicitação

``` http
PATCH https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentDefaults
Content-Type: application/json

{
  "addToCalendarAction": "studentsOnly",
  "notificationChannelUrl": "https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2"
}
```

##### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentDefaults"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "addedStudentAction": "assignIfOpen",
  "addToCalendarAction": "studentsOnly",
  "dueTime": "23:59:00",
  "notificationChannelUrl": "https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2"
}
```

## <a name="see-also"></a>Confira também

* [Atualizar educationAssignmentDefaults](/graph/api/educationassignmentdefaults-update)
* [Atualizar educationAssignment](/graph/api/educationassignment-update)
