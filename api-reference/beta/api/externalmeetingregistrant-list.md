---
title: Listar externalMeetingRegistrants
description: Obter uma lista dos externalMeetingRegistrants de um onlineMeeting.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: c232d26a57481f0cab4542f8f769522bc75e9bc1
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565129"
---
# <a name="list-externalmeetingregistrants"></a>Listar externalMeetingRegistrants

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista dos [externalMeetingRegistrants](../resources/externalmeetingregistrant.md) de um [onlineMeeting](../resources/onlinemeeting.md).

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetings.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | OnlineMeetings.ReadWrite.All |

Para usar a permissão do aplicativo para [](/graph/cloud-communication-online-meeting-application-access-policy) essa API, os administradores de locatários devem criar uma política de acesso a aplicativos e concedi-la a um usuário para autorizar o aplicativo configurado na política a buscar reuniões online e/ou artefatos de reunião online em nome desse usuário (com a ID do usuário especificada no caminho da solicitação).

## <a name="http-request"></a>Solicitação HTTP

Para obter uma lista de todos os registrantes de reuniões externas com permissão delegada ( `/me` ) e de aplicativo ( ) `/users/{userId}/` :

<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}/registration/registrants
GET /users/{userId}/onlineMeetings{meetingId}/registration/registrants
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

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos externalMeetingRegistrant](../resources/externalmeetingregistrant.md) no corpo da resposta. A **propriedade joinWebUrl** será `null` .

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "list-externalregistratrants"
}-->

```http
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
```

### <a name="response"></a>Resposta

> **Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.

<!-- {
  "blockType": "response",
  "name": "list-externalregistratrants",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalMeetingRegistrant",
  "isCollection": true
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants",
  "value": [
    {
        "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
        "id": "30494ab7-7338-4592-bfec-a4333be2a0a6",
        "joinWebUrl": null,
        "userId": null,
        "tenantId": null
    },
    {
        "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
        "id": "e264916d-f65d-48ec-9c04-c2107fd5b61f",
        "joinWebUrl": null,
        "userId": null,
        "tenantId": null
    }
  ]
}
```
