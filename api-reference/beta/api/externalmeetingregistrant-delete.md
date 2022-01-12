---
title: Excluir externalMeetingRegistrant
description: Exclua um externalMeetingRegistrant de uma reunião online.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9699a08517a2b4be495671abb76de00b0204f2e5
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860014"
---
# <a name="delete-externalmeetingregistrant"></a>Excluir externalMeetingRegistrant

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O organizador da reunião remove [um externalMeetingRegistrant](../resources/externalmeetingregistrant.md) de uma reunião online que tem [externalMeetingRegistration](../resources/externalmeetingregistration.md) habilitado.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetings.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | OnlineMeetings.ReadWrite.All |

Para usar a permissão do aplicativo para [](/graph/cloud-communication-online-meeting-application-access-policy) essa API, os administradores de locatários devem criar uma política de acesso a aplicativos e concedi-la a um usuário para autorizar o aplicativo configurado na política a buscar reuniões online e/ou artefatos de reunião online em nome desse usuário (com a ID do usuário especificada no caminho da solicitação).

## <a name="http-request"></a>Solicitação HTTP

Para remover um registro de reunião externa com permissão delegada ( `/me` ) e app ( ) `/users/{userId}/` :

<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onlineMeetings/{meetingId}/registration/registrants/{registrantId}
DELETE /users/{userId}/onlineMeetings/{meetingId}/registration/registrants/{registrantId}
```

> [!TIP]
>
> - `userId` é o **objectId** do organizador da reunião.
> - `meetingId`é a **id** de um [objeto onlineMeeting.](../resources/onlinemeeting.md)
> - `registrantId`é a **id** de [um objeto externalMeetingRegistrant.](../resources/externalmeetingregistrant.md)

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará apenas um `204 No Content` código de resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "delete-externalregistratrant"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants/9d96988d-a66a-46ce-aad7-0b245615b297
```

### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "name": "delete-externalregistratrant"
}-->

```http
HTTP/1.1 204 No Content
```
