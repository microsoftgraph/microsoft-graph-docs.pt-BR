---
title: Obter as configurações da caixa de correio do usuário
description: 'Obtenha mailboxSettings do usuário. Isso inclui configurações para respostas automáticas (notificar as pessoas automaticamente ao '
localization_priority: Normal
ms.openlocfilehash: 2d1e2ce16d82e89e701bbe90386c28b76d1607c0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880175"
---
# <a name="get-user-mailbox-settings"></a>Obter as configurações da caixa de correio do usuário

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Obtenha do usuário [mailboxSettings](../resources/mailboxsettings.md). Isso inclui configurações para respostas automáticas (notificar as pessoas automaticamente após o recebimento de seus emails), (país/região e idioma) de localidade, fuso horário e horário de trabalho.

Você pode exibir todas as configurações de caixa de correio ou obter configurações específicas.

O fuso horário é uma das configurações de preferência que um usuário pode fazer na caixa de correio. O usuário escolhe-lo de que o [suporte para fusos horários](outlookuser-supportedtimezones.md) que um administrador tiver configurado para o servidor de caixa de correio do usuário. O administrador configura fusos horários no formato de fuso horário do Windows ou o [fuso horário de autoridade de números atribuídos da Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário Olson). O formato do Windows é o padrão. 

Ao obter o fuso horário de preferência de um usuário, ele é retornado no formato em que foi configurado. Se quiser que o fuso horário esteja em um formato específico (Windows ou IANA), você pode primeiro [atualizar o fuso horário de preferência nesse formato como uma configuração de caixa de correio](user-update-mailboxsettings.md). Posteriormente, você poderá obter o fuso horário nesse formato. Como alternativa, você pode gerenciar a conversão de formato separadamente no seu aplicativo.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | MailboxSettings.Read, MailboxSettings.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | MailboxSettings.Read, MailboxSettings.ReadWrite    |
|Aplicativo | MailboxSettings.Read, MailboxSettings.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP
Para obter todas as definições de caixa de correio de um usuário:<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

Para obter configurações específicas - apenas as configurações de respostas automáticas, localidade, fuso horário ou horário de trabalho:<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se for bem-sucedido, este método retornará um código de resposta `200 OK` e um dos seguintes objetos solicitados no corpo da resposta:

- Objeto [mailboxSettings](../resources/mailboxsettings.md)
- Objeto [automaticRepliesSetting](../resources/automaticrepliessetting.md)
- Objeto [localeInfo](../resources/localeinfo.md)
- cadeia de caracteres (para **timeZone**)
- [workingHours](../resources/workinghours.md)

## <a name="example"></a>Exemplo
##### <a name="request-1"></a>Solicitação 1
O primeiro exemplo obtém todas as configurações da caixa de correio do usuário conectado, que incluem configurações de fuso horário, respostas automáticas, localidade (idioma e país/região) e horário de trabalho.
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
##### <a name="response-1"></a>Resposta 1
A resposta inclui todas as configurações de caixa de correio do usuário conectado. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "externalAudience": "All",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-14T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
        "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    },
    "timeZone":"UTC",
    "language":{
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    "workingHours":{
        "daysOfWeek":[
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday"
        ],
        "startTime":"08:00:00.0000000",
        "endTime":"17:00:00.0000000",
        "timeZone":{
            "name":"Pacific Standard Time"
        }
    }
}
```

##### <a name="request-2"></a>Solicitação 2
O segundo exemplo obtém especificamente as configurações de respostas automáticas da caixa de correio do usuário conectado.
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a>Resposta 2
A resposta inclui apenas as configurações de respostas automáticas. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings/automaticRepliesSetting",
    "status": "alwaysEnabled",
    "externalAudience": "None",
    "scheduledStartDateTime": {
        "dateTime": "2016-03-19T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "scheduledEndDateTime": {
        "dateTime": "2016-03-20T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
}
```


##### <a name="request-3"></a>Solicitação 3
O terceiro exemplo obtém especificamente as configurações de horário de trabalho da caixa de correio do usuário conectado.
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a>Resposta 3
A resposta inclui apenas as configurações de horário de trabalho. As horas de trabalho do usuário estão em um [fuso horário personalizado](../resources/customtimezone.md). Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3",
  "truncated": true,
  "@odata.type": "microsoft.graph.workingHours"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings/workingHours",
    "daysOfWeek":[
        "monday",
        "tuesday",
        "wednesday",
        "thursday",
        "friday",
        "saturday"
    ],
    "startTime":"09:00:00.0000000",
    "endTime":"18:30:00.0000000",
    "timeZone":{
        "@odata.type":"#microsoft.graph.customTimeZone",
        "bias":-200,
        "name":"Customized Time Zone",
        "standardOffset":{
            "time":"02:00:00.0000000",
            "dayOccurrence":4,
            "dayOfWeek":"sunday",
            "month":5,
            "year":0
        },
        "daylightOffset":{
            "daylightBias":-100,
            "time":"02:00:00.0000000",
            "dayOccurrence":2,
            "dayOfWeek":"sunday",
            "month":10,
            "year":0
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
