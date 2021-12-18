---
title: Excluir externalMeetingRegistration
description: Desabilitar e excluir um registro de reunião externo.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6f9ca192567cf1b5d4073d4ed6810bc861f120e5
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565126"
---
# <a name="delete-externalmeetingregistration"></a>Excluir externalMeetingRegistration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Desabilitar e excluir [o externalMeetingRegistration](../resources/externalmeetingregistration.md) de um [onlineMeeting](../resources/onlinemeeting.md).

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetings.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | OnlineMeetings.ReadWrite.All |

Para usar a permissão do aplicativo para [](/graph/cloud-communication-online-meeting-application-access-policy) essa API, os administradores de locatários devem criar uma política de acesso a aplicativos e concedi-la a um usuário para autorizar o aplicativo configurado na política a buscar reuniões online e/ou artefatos de reunião online em nome desse usuário (com a ID do usuário especificada no caminho da solicitação).

## <a name="http-request"></a>Solicitação HTTP

Para excluir o registro de reunião externa com permissão delegada ( `/me` ) e app ( ) `/users/{userId}/` :

<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onlineMeetings/{meetingId}/registration
DELETE /users/{userId}/onlineMeetings/{meetingId}/registration
```

> [!TIP]
>
>- `userId` é o **objectId** do organizador da reunião.
>- `meetingId`é a **id** do [objeto onlineMeeting.](../resources/onlinemeeting.md)

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará apenas um `204 No Content` código de resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "delete-external-registration"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "name": "delete-external-registration"
}-->

```http
HTTP/1.1 204 No Content
```
