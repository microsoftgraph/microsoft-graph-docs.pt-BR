---
title: Atualizar as configurações de caixa de correio do usuário
description: Atualize uma ou mais configurações da caixa de correio do usuário. Isso inclui as configurações para respostas automáticas (notificar as pessoas automaticamente no recebimento de seus emails), localidade (idioma e país/região), fuso horário e horário de trabalho.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d8b03e004939e205ba3f8150e8072b07723c1d63
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278646"
---
# <a name="update-user-mailbox-settings"></a>Atualizar as configurações de caixa de correio do usuário

Atualize uma ou mais configurações da caixa de correio do usuário. Isso inclui configurações de [respostas automáticas](../resources/automaticrepliessetting.md) (notificar pessoas automaticamente ao receber emails), [localidade](../resources/localeinfo.md) (idioma e país/região), fuso horário e [horário de trabalho](../resources/workinghours.md).

Você pode habilitar, configurar ou desabilitar um ou mais destas configurações como parte de [mailboxSettings](../resources/mailboxsettings.md).

**Observação** você não pode criar nem excluir configurações da caixa de correio.

Ao atualizar o fuso horário preferencial de um usuário, você pode especificá-lo no formato do Windows ou da [Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | MailboxSettings.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | MailboxSettings.ReadWrite    |
|Aplicativo | MailboxSettings.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para as propriedades relevantes que devem ser atualizadas. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter o melhor desempenho, não inclua valores existentes que não foram alterados. Estas são as propriedades graváveis/atualizáveis:

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|automaticRepliesSetting|[automaticRepliesSetting](../resources/automaticrepliessetting.md)|Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado. Você pode definir essas notificações para apenas um intervalo de datas futuras.|
|idioma|[localeInfo](../resources/localeinfo.md)|Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.|
|timeZone|string|O fuso horário padrão para a caixa de correio do usuário.|
|workingHours|[workingHours](../resources/workinghours.md)|As horas, os dias de uma semana e o fuso horário em que o usuário trabalha.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [mailboxSettings](../resources/mailboxsettings.md) no corpo da resposta.


## <a name="errors"></a>Erros

Definir horas de trabalho com valores inadequados pode retornar os seguintes erros.

| Cenário   | Código de status de HTTP | Código de erro | Mensagem de erro |
|:-----------|:------|:----------|:----------|
| **startTime** ou **endTime** inválido | 400 | RequestBodyRead | Não é possível converter o literal '08"para o tipo 'Edm.TimeOfDay' esperado.|
| A hora de início é maior do que a hora de término | 400 | ErrorInvalidTimeSettings | A Hora de Início deve ocorrer antes da Hora de Término. |
| Dia inválido em **daysOfWeek** | 400 | InvalidArguments | O valor solicitada "RandomDay" não foi encontrado.|
| **timeZone** inválido | 400 | InvalidTimeZone | As configurações de Fuso Horário fornecidas são inválidas.|


## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
O primeiro exemplo habilita as respostas automáticas de um intervalo de datas, definindo as seguintes propriedades da propriedade **automaticRepliesSetting**: **status**, **scheduledStartDateTime** e **scheduledEndDateTime**.

<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "scheduledStartDateTime": {
          "dateTime": "2016-03-20T18:00:00.0000000",
          "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
          "dateTime": "2016-03-28T18:00:00.0000000",
          "timeZone": "UTC"
        }
    }
}
```
##### <a name="response"></a>Resposta
A resposta inclui apenas as configurações atualizadas de respostas automáticas. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "scheduled",
        "externalAudience": "all",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-20T02:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T02:00:00.0000000",
            "timeZone": "UTC"
        },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    }
}
```
#### <a name="sdk-sample-code"></a>Código de amostra do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/update_mailboxsettings-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_mailboxsettings-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_mailboxsettings-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-2"></a>Solicitação 2
O segundo exemplo personaliza o fuso horário das horas de trabalho do usuário conectado definindo a propriedade **timeZone** para um [fuso horário personalizado](../resources/customtimezone.md).

<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailboxSettings
Content-Type: application/json

{
  "workingHours": {
      "endTime" : "18:30:00.0000000", 
      "daysOfWeek": [ 
          "Monday", 
          "Tuesday", 
          "Wednesday", 
          "Thursday", 
          "Friday", 
          "Saturday" 
      ], 
      "timeZone" : { 
         "@odata.type": "#microsoft.graph.customTimeZone", 
         "bias":-300, 
         "name": "Customized Time Zone",
         "standardOffset":{   
           "time":"02:00:00.0000000", 
           "dayOccurrence":2, 
           "dayOfWeek":"Sunday", 
           "month":10, 
           "year":0 
         }, 
         "daylightOffset":{   
           "daylightBias":100, 
           "time":"02:00:00.0000000", 
           "dayOccurrence":4, 
           "dayOfWeek":"Sunday", 
           "month":5, 
           "year":0 
         } 
      } 
  }
} 
```
##### <a name="response-2"></a>Resposta 2
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings",
    "workingHours":{
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
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-update-mailboxsettings.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-update-mailboxsettings.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #errors (score: 5)",
    "Error: /api-reference/v1.0/api/user-update-mailboxsettings.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
