---
title: Criar meetingRegistrant
description: Registre um registro de reunião.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 3c05e94883baaf2109672adf44d7ef268e56f467
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2021
ms.locfileid: "60370316"
---
# <a name="create-meetingregistrant"></a>Criar meetingRegistrant

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Registre [um registro de reunião](../resources/meetingregistrant.md) em uma reunião online que tenha o registro de reunião habilitado em nome do registro. [](../resources/meetingregistration.md) Esta operação tem dois cenários:

- Se o valor da **propriedade allowedRegistrant** do objeto [meetingRegistration](../resources/meetingregistration.md) for , os registros serão necessários para entrar antes de se registrarem `organization` na reunião. O **firstName**, **lastName** e **email devem** corresponder às informações armazenadas Azure Active Directory (Azure AD).
- Se o valor da **propriedade allowedRegistrant** do objeto [meetingRegistration](../resources/meetingregistration.md) for , os registrantes não serão necessários para entrar e serão considerados `everyone` anônimos.

Em qualquer cenário, o registro receberá uma notificação por email que contém suas informações de registro.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetings.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Application | OnlineMeetings.Read.All |

> [!TIP]
>
> - Se o valor da **propriedade allowedRegistrant** do [objeto meetingRegistration](../resources/meetingregistration.md) for , use a permissão delegada `organization` do registro para se inscrever.
> - Se o valor da **propriedade allowedRegistrant** do [objeto meetingRegistration](../resources/meetingregistration.md) for , use a permissão delegada `everyone` do registro para se inscrever.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/onlineMeetings/{id}/registration/registrants
```

> **Observação:** `userId` é o **objectID** do organizador da reunião.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON das propriedades editáveis de um [objeto meetingRegistrant.](../resources/meetingRegistrant.md)

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto meetingRegistrant](../resources/meetingRegistrant.md) parcial no corpo da resposta.

> [!TIP]
> O corpo da resposta conterá informações diferentes, dependendo do valor **de allowedRegistrant**.
>
> - Se o valor da **propriedade allowedRegistrant** for , somente id e joinWebUrl serão retornados `organization` no objeto [meetingRegistrant.](../resources/meetingRegistrant.md)   Os registrantes podem usar **a id** para cancelar seu registro ou **ingressar noWebUrl** para ingressar na reunião.
> - Se o valor da **propriedade allowedRegistrant** for `everyone` , um objeto [meetingRegistrant](../resources/meetingRegistrant.md) vazio será retornado. Os registrantes precisam usar os links no email que recebem para cancelar o registro ou ingressar na reunião.

## <a name="examples"></a>Exemplos

### <a name="example-1-enroll-a-signed-in-registrant"></a>Exemplo 1: Registrar um registrante de assinatura

O exemplo a seguir mostra como registrar um registro inscrito com a permissão delegada do registro quando a reunião **tiver permitidoRegistrant** definido como `organization` .

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "add-registratrant-user"
}-->

```http
POST https://graph.microsoft.com/beta/users/16664f75-11dc-4870-bec6-38c1aaa81431/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
Content-Type: application/json

{
  "firstName": "Frederick",
  "lastName": "Cormier",
  "email": "frederick.cormier@contoso.com",
  "customQuestionAnswers": [
    {
      "questionId": "MSM5YjlmM2Q4ZS03ZmVkLTRmN3gwMDIw94MDAyMF9hX3gwMDIwX2RldmU=",
      "value": "No"
    },
    {
      "questionId": "MSM5M2E2OWQ1Ni1jZTc4LTQDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8=",
      "value": "Internet"
    }
  ]
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "name": "add-registratrant-user",
  "@odata.type": "microsoft.graph.meetingRegistrant"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants/$entity",
  "id": "gWWckDBR6UOI8_yzWCzeNw,6pAAiSU1bkGqzLnbHG_muA,bzLh6uR-5EGYsCvtvIvs6Q,E4jbleVFdE6BDf6ei3YBOA,KvXQzK4zfU-5LQj_ZLWgow,A7_SArco00S-Qr707l0vBA,UFakyZrk1K9vBacExW1muA",
  "registrationDateTime": null,
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MmE4Mzg1OTItYjg2Ni00ZmNmLWI5NjMtODNkZDJiMWNlNTVi%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5131-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%22dc17674c-81d9-4adb-bfb2-8f6a442e4622%22%2c%22prid%22%3a%22gWWckDBR6UOI8_yzWCzeNw%2c6pAAiSa1bkGqzLnbHG_muA%2cbzLh6uR-5EGdsCvtvIvs6Q%2cE4jbleVFdE6BDf6ei3YBOA%2cKvXQzK4zfU-5LQj_ZLWgow%2cA7_SArco00S-Qr707l0vBA%2cUFaiyZrk1K9vBacExW1muA%22%2c%22isPublic%22%3afalse%7d",
  "firstName": null,
  "lastName": null,
  "email": null,
  "status": null,
  "customQuestionAnswers": []
}
```

### <a name="example-2-enroll-an-anonymous-registrant"></a>Exemplo 2: Registrar um registro anônimo

O exemplo a seguir mostra como registrar um registro anônimo com permissão de aplicativo quando a reunião **tiver permitidoRegistrant** definido como `everyone` .

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "add-registratrant-app"
}-->

```http
POST https://graph.microsoft.com/beta/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
Content-Type: application/json

{
  "firstName": "Lisa",
  "lastName": "Adkins",
  "email": "lisa.adkins@contoso.com",
  "customQuestionAnswers": [
    {
      "questionId": "MSM5YjlmM2Q4ZS03ZmVkLTRmN3gwMDIw94MDAyMF9hX3gwMDIwX2RldmU=",
      "value": "No"
    },
    {
      "questionId": "MSM5M2E2OWQ1Ni1jZTc4LTQDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8=",
      "value": "Internet"
    }
  ]
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "name": "add-registratrant-app",
  "@odata.type": "microsoft.graph.meetingRegistrant"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants/$entity",
    "id": "",
    "registrationDateTime": null,
    "joinWebUrl": "",
    "firstName": null,
    "lastName": null,
    "email": null,
    "status": null,
    "customQuestionAnswers": []
}
```
