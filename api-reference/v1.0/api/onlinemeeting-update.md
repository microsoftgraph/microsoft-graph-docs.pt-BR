---
title: Atualizar onlineMeeting
description: Atualize as propriedades de uma reunião online.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 66a7cac0fcdf63a09daa190549ff442304c1d29d
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766485"
---
# <a name="update-onlinemeeting"></a>Atualizar onlineMeeting

Namespace: microsoft.graph

Atualize as propriedades do objeto [onlineMeeting](../resources/onlinemeeting.md) especificado.

Consulte [a seção Solicitar corpo](#request-body) para a lista de propriedades que suportam a atualização.

## <a name="permissions"></a>Permissões

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | OnlineMeetings.ReadWrite                    |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | OnlineMeetings.ReadWrite.All                |

Para usar a permissão do aplicativo para [](/graph/cloud-communication-online-meeting-application-access-policy) essa API, os administradores de locatários devem criar uma política de acesso a aplicativos e concedi-la a um usuário para autorizar o aplicativo configurado na política para obter artefatos de reunião online em nome desse usuário (com a ID do usuário especificada no caminho da solicitação).

## <a name="http-request"></a>Solicitação HTTP

Para atualizar o **onlineMeeting** especificado usando a ID da reunião com a permissão delegada ( `/me` ) e do aplicativo ( ) `/users/{userId}/` :
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{meetingId}
PATCH /users/{userId}/onlineMeetings/{meetingId}
```

> [!NOTE]
>
> - `userId` é a ID de objeto de um usuário no [Portal de gerenciamento de usuário do Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade). Para obter mais detalhes, consulte [política de acesso ao aplicativo](/graph/cloud-communication-online-meeting-application-access-policy).
> - `meetingId`é a **id** de um [objeto onlineMeeting.](../resources/onlinemeeting.md)

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                 |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

A tabela a seguir lista as propriedades que podem ser atualizadas. No corpo da solicitação, inclua apenas as propriedades que precisam ser atualizadas, com as seguintes exceções:

- Ajustar a data/hora inicial ou final de uma reunião online sempre requer as propriedades **startDateTime** e **endDateTime** no corpo da solicitação.
- O **campo** organizador da **propriedade participants** não pode ser atualizado. O organizador da reunião não pode ser modificado após a criação da reunião.
- Ajustar o **campo de** participantes  da propriedade participantes, como adicionar ou remover um participante à reunião, sempre requer a lista completa de participantes no corpo da solicitação.

A última coluna indica se a atualização dessa propriedade terá efeito para uma reunião em andamento.

| Propriedade                    | Tipo                                                       | Descrição                                                                         | Aplica-se a reuniões em andamento?    |
|-----------------------------|------------------------------------------------------------|-------------------------------------------------------------------------------------|------------------------------|
| startDateTime               | DateTime                                                   | O horário de início da reunião em UTC.                                                      | Não                           |
| endDateTime                 | DateTime                                                   | A hora de término da reunião em UTC.                                                        | Não                           |
| assunto                     | Cadeia de caracteres                                                     | O assunto da reunião online.                                                  | Não                           |
| participants                | [meetingParticipants](../resources/meetingparticipants.md) | Os participantes associados à reunião online. Somente participantes podem ser atualizados. | Não                           |
| isEntryExitAnnounced        | Boolean                                                    | Se os chamadores ingressarão ou sairão.                              | Sim                          |
| lobbyBypassSettings         | [lobbyBypassSettings](../resources/lobbyBypassSettings.md) | Especifica quais participantes podem ignorar o lobby da reunião.                          | Sim                          |
| allowedPresenters           | onlineMeetingPresenters                                    | Especifica quem pode ser um apresentador em uma reunião.                                      | Sim |
| allowAttendeeToEnableCamera | Boolean                                                    | Indica se os participantes podem ativar a câmera.                               | Sim                          |
| allowAttendeeToEnableMic    | Boolean                                                    | Indica se os participantes podem ativar o microfone.                           | Sim                          |
| allowMeetingChat            | meetingChatMode                                            | Especifica o modo de chat de reunião.                                                 | Sim                          |
| allowTeamworkReactions      | Boolean                                                    | Indica se Teams reações estão habilitadas para a reunião.                      | Sim                          |

> [!NOTE]
>
>- Para ver a lista de valores possíveis **para allowedPresenters** e **allowMeetingChat,** consulte [onlineMeeting](../resources/onlinemeeting.md).
>- Ao atualizar o valor **de allowedPresenters** para , inclua uma lista completa de participantes com participantes especificados definido como no corpo `roleIsPresenter` da  `role` `presenter` solicitação.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto onlineMeeting](../resources/onlinemeeting.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-update-the-startdatetime-enddatetime-and-subject"></a>Exemplo 1: atualizar o startDateTime, endDateTime e assunto

#### <a name="request"></a>Solicitação

> **Observação:** A ID da reunião foi reduzida para a capacidade de leitura.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_start_end_subject"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "startDateTime": "2020-09-09T14:33:30.8546353-07:00",
  "endDateTime": "2020-09-09T15:03:30.8566356-07:00",
  "subject": "Patch Meeting Subject"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-start-end-subject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-start-end-subject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-start-end-subject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-start-end-subject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi",
   "creationDateTime":"2020-07-03T00:23:39.444642Z",
   "startDateTime":"2020-09-09T21:33:30.8546353Z",
   "endDateTime":"2020-09-09T22:03:30.8566356Z",
   "joinWebUrl":"url",
   "subject":"Patch Meeting Subject",
   "isBroadcast":false,
   "autoAdmittedUsers":"EveryoneInCompany",
   "outerMeetingAutoAdmittedUsers":null,
   "participants":{
      "organizer":{
         "upn":"upn",
         "role": "presenter",
         "identity":{
            "azureApplicationInstance":null,
            "applicationInstance":null,
            "application":null,
            "device":null,
            "user":{
               "id":"8716745d-77a9-4be3-afff-009e4b81658e",
               "displayName":null,
               "tenantId":"0823831b-1f1b-424b-b90a-1caa345a742a",
               "identityProvider":"AAD"
            }
         }
      }
   },
   "audioConferencing":{
      "conferenceId":"id",
      "tollNumber":"+1-900-555-0100",
      "tollFreeNumber":"+1-800-555-0100",
      "dialinUrl":"url"
   }
}
```

#### <a name="example-2-update-the-lobbybypasssettings"></a>Exemplo 2: atualizar o lobbyBypassSettings
> **Observação:** A ID da reunião foi reduzida para a capacidade de leitura.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_lobbyBypassSettings"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "lobbyBypassSettings": {
      "isDialInBypassEnabled": true
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-lobbybypasssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-lobbybypasssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-lobbybypasssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-lobbybypasssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi",
    "creationDateTime":"2020-07-03T00:23:39.444642Z",
    "startDateTime":"2020-09-09T21:33:30.8546353Z",
    "endDateTime":"2020-09-09T22:03:30.8566356Z",
    "joinWebUrl":"(redacted)",
    "subject":"Patch Meeting Subject",
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "videoTeleconferenceId": "(redacted)",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622",
                    "displayName": null,
                    "tenantId": "909c6581-5130-43e9-88f3-fcb3582cde38",
                    "identityProvider": "AAD"
                }
            }
        },
        "attendees": [],
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-7-16 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch online meeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


