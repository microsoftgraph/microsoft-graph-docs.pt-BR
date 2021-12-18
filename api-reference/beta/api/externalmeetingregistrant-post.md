---
title: Criar externalMeetingRegistrant
description: Registre um registro de reunião externo.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 226cb77bcc68612982769168945d1d1d556d4027
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565130"
---
# <a name="create-externalmeetingregistrant"></a>Criar externalMeetingRegistrant

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Registrar um [externalMeetingRegistrant em](../resources/externalmeetingregistrant.md) uma reunião online que tenha [externalMeetingRegistration](../resources/externalmeetingregistration.md) habilitado. O organizador da reunião registra alguém fornecendo uma **id** exclusiva no sistema de registro externo e obtém o **joinWebUrl** exclusivo desse registro.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetings.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | OnlineMeetings.ReadWrite.All |

Para usar a permissão do aplicativo para [](/graph/cloud-communication-online-meeting-application-access-policy) essa API, os administradores de locatários devem criar uma política de acesso a aplicativos e concedi-la a um usuário para autorizar o aplicativo configurado na política a buscar reuniões online e/ou artefatos de reunião online em nome desse usuário (com a ID do usuário especificada no caminho da solicitação).

## <a name="http-request"></a>Solicitação HTTP

Para criar um registro de reunião externa com permissão delegada ( `/me` ) e app ( ) `/users/{userId}/` :

<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/{meetingId}/registration/registrants
POST /users/{userId}/onlineMeetings{meetingId}/registration/registrants
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

- Se o valor da propriedade **allowedRegistrant** do [objeto externalMeetingRegistration](../resources/externalmeetingregistration.md) for , fornecer a id do sistema de registro `organization` externo, **tenantId** e **userId** do registro no Azure Active Directory. 
- Se o valor da **propriedade allowedRegistrant** do [objeto externalMeetingRegistration](../resources/externalmeetingregistration.md) for , apenas fornecerá a `everyone` **id** do sistema de registro externo.

> [!IMPORTANT]
>
>- A **id do** sistema de registro externo pode ser qualquer forma de cadeia de caracteres.
>- Você deve fornecer a **propriedade @odata.type** para especificar o tipo de registro. Para obter mais detalhes, consulte os [exemplos a seguir](#examples).

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de `200 OK` resposta e um objeto [externalMeetingRegistrant](../resources/externalmeetingregistrant.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-enroll-a-registrant-when-the-meeting-registration-has-allowedregistrant-set-to-everyone"></a>Exemplo 1: Registrar um registro quando o registro da reunião tiver permitidoRegistrant definido como "todos"

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "add-externalregistratrant-public"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "9d96988d-a66a-46ce-aad7-0b245615b297"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "name": "add-externalregistratrant-public",
  "@odata.type": "microsoft.graph.externalMeetingRegistrant"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants/$entity",
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "30494ab7-7338-4592-bfec-a4333be2a0a6",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NjliNTYxNjktNzAwNi00OTlhLWFmMWEtMGZhY2JjZGM5NmEy%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5130-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%2216664f75-11dc-4870-bec6-38c1aaa81431%22%2c%22prid%22%3a%229d96988d-a66a-46ce-aad7-0b245615b297%22%2c%22isPublic%22%3atrue%7d",
  "userId": null,
  "tenantId": null
}
```

### <a name="example-2-enroll-a-registrant-when-the-meeting-registration-has-allowedregistrant-set-to-organization"></a>Exemplo 2: Registrar um registro quando o registro de reunião tiver permitidoRegistrant definido como "organização"

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "add-externalregistratrant-private"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "30494ab7-7338-4592-bfec-a4333be2a0a6",
  "tenantId": "909c6581-5130-43e9-88f3-fcb3582cde37",
  "userId": "cc515404-b55c-466e-b896-992c918ecc01"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "name": "add-externalregistratrant-private",
  "@odata.type": "microsoft.graph.externalMeetingRegistrant"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants/$entity",
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "30494ab7-7338-4592-bfec-a4333be2a0a6",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NjliNTYxNjktNzAwNi00OTlhLWFmMWEtMGZhY2JjZGM5NmEy%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5130-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%2216664f75-11dc-4870-bec6-38c1aaa81431%22%2c%22prid%22%3a%2230494ab7-7338-4592-bfec-a4333be2a0a6%22%2c%22isPublic%22%3afalse%7d",
  "userId": "909c6581-5130-43e9-88f3-fcb3582cde37",
  "tenantId": "cc515404-b55c-466e-b896-992c918ecc01"
}
```
