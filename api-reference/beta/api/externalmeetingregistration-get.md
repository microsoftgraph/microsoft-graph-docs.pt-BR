---
title: Obter externalMeetingRegistration
description: Obter informações de registro externo de uma reunião online.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: c93650519d484d043850a31e36625a500b974b6e
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565136"
---
# <a name="get-externalmeetingregistration"></a>Obter externalMeetingRegistration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter [os detalhes externalMeetingRegistration](../resources/externalmeetingregistration.md) associados a [um onlineMeeting](../resources/onlinemeeting.md).

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetings.Read, OnlineMeetings.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All |

Para usar a permissão do aplicativo para [](/graph/cloud-communication-online-meeting-application-access-policy) essa API, os administradores de locatários devem criar uma política de acesso a aplicativos e concedi-la a um usuário para autorizar o aplicativo configurado na política a buscar reuniões online e/ou artefatos de reunião online em nome desse usuário (com a ID do usuário especificada no caminho da solicitação).

## <a name="http-request"></a>Solicitação HTTP

Para obter o registro de reunião externa com permissão delegada ( `/me` ) e app ( ) `/users/{userId}/` :

<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}/registration
GET /users/{userId}/onlineMeetings/{meetingId}/registration
```

> [!TIP]
>
>- `userId` é o **objectId** do organizador da reunião.
>- `meetingId`é a **id** do [objeto onlineMeeting.](../resources/onlinemeeting.md)

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto externalMeetingRegistration](../resources/externalmeetingregistration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get-externalregistration"
}-->

```http
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "name": "get-externalregistration",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalMeetingRegistration"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/$entity",
  "@odata.type": "#microsoft.graph.externalMeetingRegistration",
  "id": "f23714a3-a2f4-4b1d-96d2-bfe9097e7163",
  "allowedRegistrant": "everyone"
}
```
