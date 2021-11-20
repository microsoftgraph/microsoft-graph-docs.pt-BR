---
title: Obter meetingAttendanceReport
description: Obter o relatório de participação de uma reunião online.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6ff8c812928a983868b47775e3c970c4c60da21c
ms.sourcegitcommit: 1cf7a82df17afc6291e2c93d8b2c277bf3382e6a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2021
ms.locfileid: "61130248"
---
# <a name="get-meetingattendancereport"></a>Obter meetingAttendanceReport

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter [o meetingAttendanceReport](../resources/meetingAttendanceReport.md) para um [onlineMeeting](../resources/onlinemeeting.md). Sempre que uma reunião online termina, um relatório de participação será gerado para essa sessão.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetingArtifact.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | OnlineMeetingArtifact.Read.All |

Para usar a permissão do aplicativo para essa API, os administradores de locatários devem criar uma política de acesso a aplicativos [e](/graph/cloud-communication-online-meeting-application-access-policy) concedi-la a um usuário. Isso autoriza o aplicativo configurado na política a buscar reuniões online e/ou artefatos de reunião online em nome desse usuário (com a ID do usuário especificada no caminho da solicitação).

## <a name="http-request"></a>Solicitação HTTP

Para obter um relatório de participação por ID com permissão delegada ( `/me` ) e app ( ) `/users/{userId}` :
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}/attendanceReports/{reportId}
GET /users/{userId}/onlineMeetings/{meetingId}/attendanceReports/{reportId}
```

Para obter o relatório de participação da sessão mais recente de uma reunião online com permissão delegada ( `/me` ) e app ( ) `/users/{userId}` :
<!-- { "blockType": "ignored" }-->
```http
GET /me/onlineMeetings/{meetingId}/meetingAttendanceReport
GET /users/{userId}/onlineMeetings/{meetingId}/meetingAttendanceReport
```

> [!TIP]
>
>- `userId` é a ID de objeto de um usuário no [Portal de gerenciamento de usuário do Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade). Para obter mais detalhes, consulte [política de acesso ao aplicativo](/graph/cloud-communication-online-meeting-application-access-policy).
>- `meetingId`é a **id** de um [objeto onlineMeeting.](../resources/onlinemeeting.md)
>- `reportId`é a **id** de um [objeto meetingAttendanceReport.](../resources/meetingAttendanceReport.md)

> [!CAUTION]
>
>- O caminho `/meetingAttendanceReport` foi preterido. Em frente, use o `/attendanceReports` caminho para recuperar relatórios de participação para uma reunião online.
>- O `/meetingAttendanceReport` caminho permanecerá em beta para compatibilidade com versões. No entanto, para obter a mesma resposta, você precisa adicionar a `expand` opção de consulta. Para obter detalhes, consulte [a seção Parâmetros de consulta](#optional-query-parameters) opcional.

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

> [!TIP]
> A **propriedade attendanceRecords** é uma propriedade de navegação que não é retornada por padrão. Para recuperar **attendanceRecords** na linha, use a opção de consulta, conforme `$expand=attendanceRecords` mostrado no exemplo [2](#example-2-get-the-latest-attendance-report-for-an-online-meeting).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto meetingAttendanceReport](../resources/meetingAttendanceReport.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="example-1-get-the-attendance-report-for-an-online-meeting-by-id"></a>Exemplo 1: Obter o relatório de participação de uma reunião online por ID

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get-attendanceReport-by-id"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/attendanceReports/2c2c2454-7613-4d6e-9c7c-4cf7a6cdce89?$expand=attendanceRecords
```

#### <a name="response"></a>Resposta

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/attendanceReports('c9b6db1c-d5eb-427d-a5c0-20088d9b22d7')",
  "id": "c9b6db1c-d5eb-427d-a5c0-20088d9b22d7",
  "totalParticipantCount": 1,
  "meetingStartDateTime": "2021-10-05T04:38:23.945Z",
  "meetingEndDateTime": "2021-10-05T04:43:49.77Z",
  "attendanceRecords": [
    {
      "emailAddress": "(email address)",
      "totalAttendanceInSeconds": 1152,
      "role": "Presenter",
      "identity": {
        "id": "(redacted)",
        "displayName": "(redacted)",
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

### <a name="example-2-get-the-latest-attendance-report-for-an-online-meeting"></a>Exemplo 2: Obter o relatório de participação mais recente de uma reunião online

O exemplo a seguir mostra uma solicitação para obter um relatório de participação de reunião para a sessão mais recente de uma reunião online.

#### <a name="request"></a>Solicitação

A solicitação a seguir usa permissão delegada.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_attendance_report"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/meetingAttendanceReport
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attendance-report-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attendance-report-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attendance-report-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-attendance-report-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

A solicitação a seguir usa a permissão do aplicativo.
<!-- { "blockType": "ignored" }-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/dc74d9bb-6afe-433d-8eaa-e39d80d3a647/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/meetingAttendanceReport
```

#### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingAttendanceReport",
  "name": "get_attendance_report"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('dc74d9bb-6afe-433d-8eaa-e39d80d3a647')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy')/meetingAttendanceReport/$entity",
  "attendanceRecords": [
    {
      "emailAddress": "email address",
      "totalAttendanceInSeconds": 1558,
      "role": "Organizer",
      "identity": {
        "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
        "displayName": "(redacted)",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-03-16T18:59:46.598956Z",
          "leaveDateTime": "2021-03-16T19:25:45.4473057Z",
          "durationInSeconds": 1558
        }
      ]
    },
    {
      "emailAddress": "email address",
      "totalAttendanceInSeconds": 1152,
      "role": "Presenter",
      "identity": {
        "id": "(redacted)",
        "displayName": "(redacted)",
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
  ],
  "totalParticipantCount": 2
}
```
