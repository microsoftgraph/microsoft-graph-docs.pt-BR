---
title: Criar meetingRegistration
description: Criar e habilitar o registro para uma reunião online.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d7e8110d10b420fb00a5b48d97be700388417c38
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2021
ms.locfileid: "60370315"
---
# <a name="create-meetingregistration"></a>Criar meetingRegistration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie e habilita o registro [para um onlineMeeting](../resources/onlinemeeting.md) em nome do organizador. Uma reunião online só pode ter um registro habilitado.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetings.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/{id}/registration
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |
| Accept-Language | Idioma. Opcional.       |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON de um [objeto meetingRegistration.](../resources/meetingregistration.md)

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto meetingRegistration](../resources/meetingregistration.md) no corpo da resposta.

> [!NOTE]
>
>- A **propriedade registrationPageViewCount** não é retornada no corpo da resposta deste método. Use o [método Get meetingRegistration](meetingRegistration-get.md) para recuperar essa propriedade.
>- **customQuestions** é um recurso relacionado que só pode ser criado na linha, mas não retornado neste método. Use o [método Get meetingRegistration](meetingRegistration-get.md) ou [Get meetingRegistrationQuestion](meetingregistrationquestion-get.md) para recuperá-lo.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create-registration",
  "@odata.type": "microsoft.graph.meetingRegistration"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration
Content-Type: application/json

{
  "subject":"Microsoft Ignite",
  "description": "Join us November 2–4, 2021 to explore the latest tools, training sessions, technical expertise, networking opportunities, and more.",
  "startDateTime":"2021-11-02T08:00:00-08:00",
  "endDateTime":"2021-11-04T04:00:00-08:00",
  "allowedRegistrant": "everyone",
  "speakers": [
    {
      "displayName": "Henry Ross",
      "bio": "Chairman and Chief Executive Officer"
    },
    {
      "displayName": "Hailey Clark",
      "bio": "EVP"
    }
  ],
  "customQuestions": [
    {
      "displayName": "Are you a developer?",
      "answerInputType": "radioButton",
      "answerOptions": [ "Yes", "No" ],
      "isRequired": true
    },
    {
      "displayName": "Where did you hear about us?",
      "answerInputType": "text",
      "isRequired": false
    }
  ]
}
```

### <a name="response"></a>Resposta

> **Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.

<!-- {
  "blockType": "response",
  "name": "create-registration",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingRegistration"
}-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/$entity",
  "id": "gWWckDBR6UOI8_yzWCzeNw,6pAAiSU1bkGqzLnbHG_muA,bzLh6uR-5EGYsCvtvIvs6Q,2Hui7cZ3e0m1BblvyhKFaw,Bcn5itxWh0ui5zRxG26Akw,XCvoVSOmK0e9fivLeKuR_w",
  "registrationPageWebUrl": "https://teams.microsoft.com/registration/gWWckDBR6UOI8_yzWCzeNw,6pABiSU1bkGqzLnbHG_muA,bzLh6uR-5EGYsCvtvIvs6Q,luiTigKrcUGE6Cm33MyQgA,29OIGSH4skyQNu6mNxJr3w,m2bnpmqE_EqwV1Q8dr280E?mode=read&tenantId=eefc0b3a-a334-4fb7-ac60-2f1cf13ec00d",
  "allowedRegistrant": "everyone",
  "subject": "Microsoft Ignite",
  "description": "Join us November 2–4, 2021 to explore the latest tools, training sessions, technical expertise, networking opportunities, and more.",
  "startDateTime": "2021-11-02T016:00:00Z",
  "endDateTime": "2021-11-04T12:00:00Z",
  "registrationPageViewCount": null,
  "speakers": [
    {
      "displayName": "Henry Ross",
      "bio": "Chairman and Chief Executive Officer"
    },
    {
      "displayName": "Hailey Clark",
      "bio": "EVP"
    }
  ]
}
```
