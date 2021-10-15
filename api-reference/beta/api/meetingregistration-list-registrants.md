---
title: Listar registrantes
description: Obter uma lista dos meetingRegistrants de um onlineMeeting.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8a221365b030412a4988f4b33fff859328924e42
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2021
ms.locfileid: "60370318"
---
# <a name="list-registrants"></a>Listar registrantes

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista dos [meetingRegistrants](../resources/meetingregistrant.md) de um [onlineMeeting](../resources/onlinemeeting.md) em nome do organizador.

Você pode usar esse método para obter o relatório de registro de [um Microsoft Teams webinar](https://support.microsoft.com/en-us/office/get-started-with-teams-webinars-42f3f874-22dc-4289-b53f-bbc1a69013e3).

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetings.Read, OnlineMeetings.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{id}/registration/registrants
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos meetingRegistrant](../resources/meetingRegistrant.md) no corpo da resposta. As **propriedades joinWebUrl** **e questionId** serão `null` .

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "list-registratrants"
}-->

```http
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
```

### <a name="response"></a>Resposta

> **Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.

<!-- {
  "blockType": "response",
  "name": "list-registratrants",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.meetingRegistrant)"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants",
  "value": [
    {
      "id": "gWWckDBR6UOI8_yzWCzeNw,6pAAiSU1bkGqc8soJZw5Pg,3aMJxgQBxEufdo7_Qube_w,YgKy1Rtx-0SFjRbv-ww1ag,Cuzk8JP_iTTWqCOyVcalVA",
      "registrationDateTime": "2021-10-02T00:07:16.882602Z",
      "joinWebUrl": null,
      "firstName": "Frederick",
      "lastName": "Cormier",
      "email": "frederick.cormier@contoso.com",
      "status": "registered",
      "customQuestionAnswers": [
        {
          "questionId": null,
          "displayName": "Are you a developer?",
          "value": "Yes"
        },
        {
          "questionId": null,
          "displayName": "Where did you hear about us?",
          "value": "Company"
        }
      ]
    },
    {
      "id": "gWWckDBR6UOI8_yzWCzeNw,6pAAiSU1bkGqzLnbHG_muA,b0ezc8soJZw5Pg,3aMJxgQBxEufdo7_Qube_w,YgKy1Rtx-0SFjRbv-ww1ag,UwWARTlCT0dzO0jsuuq5EA",
      "registrationDateTime": "2021-10-02T00:08:49.1053222Z",
      "joinWebUrl": null,
      "firstName": "Lisa",
      "lastName": "Adkins",
      "email": "lisa.adkins@contoso.com",
      "status": "registered",
      "customQuestionAnswers": [
        {
          "questionId": null,
          "displayName": "Are you a developer?",
          "value": "No"
        },
        {
          "questionId": null,
          "displayName": "Where did you hear about us?",
          "value": ""
        }
      ]
    }
  ]
}
```
