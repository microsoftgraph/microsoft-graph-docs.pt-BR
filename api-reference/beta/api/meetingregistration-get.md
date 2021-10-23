---
title: Obter meetingRegistration
description: Obter informações de registro de uma reunião online.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 893fc26d2328540d9e27daa261d6f7ab554ddf4c
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561483"
---
# <a name="get-meetingregistration"></a>Obter meetingRegistration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter os [detalhes meetingRegistration](../resources/meetingregistration.md) associados a um [onlineMeeting](../resources/onlinemeeting.md) em nome do organizador.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetings.Read, OnlineMeetings.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{id}/registration
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

> [!TIP]
> A **propriedade customQuestions** não é retornada por padrão. Para recuperar **customQuestions** na linha, use a opção de consulta, conforme `expand` mostrado no exemplo mais adiante neste tópico.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto meetingRegistration](../resources/meetingregistration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-registration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration?$expand=customQuestions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

> **Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.

<!-- {
  "blockType": "response",
  "name": "get-registration",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingRegistration"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration(customQuestions())/$entity",
  "id": "gWWckDBR6UOI8_yzWCzeNw,6pABiSU1bkGqzLnbHG_muA,bzLh6uR-5EGYsCvtvIvs6Q,luiTigKrcUGE6Cm33MyQgA,29OIGSH4skyQNu6mNxJr3w,m2bnpmqE_EqwV1Q8dr280E",
  "registrationPageWebUrl": "https://teams.microsoft.com/registration/gWWckDBR6UOI8_yzWCzeNw,6pABiSU1bkGqzLnbHG_muA,bzLh6uR-5EGYsCvtvIvs6Q,luiTigKrcUGE6Cm33MyQgA,29OIGSH4skyQNu6mNxJr3w,m2bnpmqE_EqwV1Q8dr280E?mode=read&tenantId=eefc0b3a-a334-4fb7-ac60-2f1cf13ec00d",
  "allowedRegistrant": "everyone",
  "subject": "Microsoft Ignite",
  "description": "Join us November 2–4, 2021 to explore the latest tools, training sessions, technical expertise, networking opportunities, and more.",
  "startDateTime": "2021-11-02T016:00:00Z",
  "endDateTime": "2021-11-04T12:00:00Z",
  "registrationPageViewCount": 0,
  "speakers": [
    {
      "displayName": "Henry Ross",
      "bio": "Chairman and Chief Executive Officer"
    },
    {
      "displayName": "Hailey Clark",
      "bio": "CFO"
    }
  ],
  "customQuestions@odata.context": "https://graph.microsoft.com/beta/$metadata#users('dc17674c-81d9-4adb-bfb2-8f6a442e4622')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/customQuestions",
  "customQuestions": [
    {
      "id": "MSNhMjVlZmUyMy01MDBhLTQwYjItYjUwZS04YWU5EG9hX3gwMDIwX2RldmU=",
      "displayName": "Are you a developer?",
      "isRequired": true,
      "answerInputType": "radioButton",
      "answerOptions": [
          "Yes",
          "No"
      ]
    },
    {
      "id": "MSM5MjViYzIxYi1mNTI3LTQ1ZmEtODYwYi1hZDT5ZGNjX3lvdV94MDAyMF8=",
      "displayName": "Where did you hear about us?",
      "isRequired": false,
      "answerInputType": "text",
      "answerOptions": []
    }
  ]
}
```
