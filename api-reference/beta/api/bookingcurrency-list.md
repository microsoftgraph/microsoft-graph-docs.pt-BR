---
title: Lista bookingCurrencies
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: 146fc1197a8ef206e78304d81c30878a67eeafad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033091"
---
# <a name="list-bookingcurrencies"></a>Lista bookingCurrencies

 > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.
 
Obtenha uma lista de objetos de [bookingCurrency](../resources/bookingcurrency.md) disponíveis para uma empresa Microsoft Bookings.
## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | Sem suporte.  | 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método oferece suporte para os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta, incluindo $count, $filter, $select, $skip, Skip e $top.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.
## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [bookingCurrency](../resources/bookingcurrency.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a>Resposta
Este é um exemplo de resposta. Observação: No objeto response mostrado aqui é truncado para fins de concisão. Serão retornados todos os moedas com suporte e as propriedades de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingCurrencies",
    "value":[
        {
            "id":"AED",
            "symbol":"د.إ.‏"
        },
        {
            "id":"AFN",
            "symbol":"؋"
        },
        {
            "id":"ALL",
            "symbol":"Lekë"
        },
        {
            "id":"AMD",
            "symbol":"֏"
        },
        {
            "id":"USD",
            "symbol":"$"
        },
        {
            "id":"YER",
            "symbol":"ر.ي.‏"
        },
        {
            "id":"ZAR",
            "symbol":"R"
        },
        {
            "id":"ZMW",
            "symbol":"K"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List bookingCurrencies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->