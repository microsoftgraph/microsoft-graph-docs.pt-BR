---
title: Obter meetingAttendanceReport
description: Obter o relatório de participação de uma reunião online.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: af9fa6e85082c7dbc16808e5852205cab6227af6
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860997"
---
# <a name="get-meetingattendancereport"></a>Obter meetingAttendanceReport

Namespace: microsoft.graph

Obter [o meetingAttendanceReport](../resources/meetingAttendanceReport.md) para um [onlineMeeting](../resources/onlinemeeting.md). Sempre que uma reunião online termina, um relatório de participação será gerado para essa sessão.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetingArtifact.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | OnlineMeetingArtifact.Read.All |

Para usar a permissão do aplicativo para essa API, os administradores de locatários devem criar uma política de acesso a aplicativos e concedi-la a um usuário. Isso autoriza o aplicativo configurado na política a buscar reuniões online e/ou artefatos de reunião online em nome desse usuário (com a ID do usuário especificada no caminho da solicitação). Para obter mais detalhes, consulte [Permitir que os aplicativos acessem reuniões online em nome de um usuário](/graph/cloud-communication-online-meeting-application-access-policy).

## <a name="http-request"></a>Solicitação HTTP

Para obter um relatório de participação por ID com permissão delegada ( `/me` ) e app ( ) `/users/{userId}` :

<!-- { "blockType": "ignored" } -->

```http
GET /me/onlineMeetings/{meetingId}/attendanceReports/{reportId}
GET /users/{userId}/onlineMeetings/{meetingId}/attendanceReports/{reportId}
```

> [!TIP]
>
>- `userId` é a ID de objeto de um usuário no [Portal de gerenciamento de usuário do Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade). Para obter mais detalhes, consulte [Permitir que os aplicativos acessem reuniões online em nome de um usuário](/graph/cloud-communication-online-meeting-application-access-policy).
>- `meetingId`é a **id** de um [objeto onlineMeeting.](../resources/onlinemeeting.md)
>- `reportId`é a **id** de um [objeto meetingAttendanceReport.](../resources/meetingAttendanceReport.md)

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

> [!TIP]
> A **propriedade attendanceRecords** é uma propriedade de navegação que não é retornada por padrão. Para recuperar **attendanceRecords** na linha, use a `$expand=attendanceRecords` opção de consulta, conforme mostrado no [exemplo](#example).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto meetingAttendanceReport](../resources/meetingAttendanceReport.md) no corpo da resposta.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como obter o relatório de participação de uma reunião online com permissão delegada.

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get-attendanceReport-by-id"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/attendanceReports/c9b6db1c-d5eb-427d-a5c0-20088d9b22d7?$expand=attendanceRecords
```

### <a name="response"></a>Resposta

> **Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.

<!-- {
  "blockType": "response",
  "name": "get-attendanceReport-by-id",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingAttendanceReport"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/attendanceReports('c9b6db1c-d5eb-427d-a5c0-20088d9b22d7')",
  "id": "c9b6db1c-d5eb-427d-a5c0-20088d9b22d7",
  "totalParticipantCount": 1,
  "meetingStartDateTime": "2021-10-05T04:38:23.945Z",
  "meetingEndDateTime": "2021-10-05T04:43:49.77Z",
  "attendanceRecords": [
    {
      "emailAddress": "frederick.cormier@contoso.com",
      "totalAttendanceInSeconds": 1152,
      "role": "Presenter",
      "identity": {
        "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4623",
        "displayName": "Frederick Cormier",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-03-16T18:59:52.2782182Z",
          "leaveDateTime": "2021-03-16T19:06:47.7218491Z",
          "durationInSeconds": 415
        },
        {
          "joinDateTime": "2021-03-16T19:09:23.9834702Z",
          "leaveDateTime": "2021-03-16T19:16:31.1381195Z",
          "durationInSeconds": 427
        },
        {
          "joinDateTime": "2021-03-16T19:20:27.7094382Z",
          "leaveDateTime": "2021-03-16T19:25:37.7121956Z",
          "durationInSeconds": 310
        }
      ]
    }
  ]
}
```
