---
title: Criar bookingCustomer
description: Crie um novo objeto bookingCustomer.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 67007b24605b9adbb77b7454ec4f3b75ca016caa
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014205"
---
# <a name="create-bookingcustomer"></a>Criar bookingCustomer

Namespace: microsoft.graph

Crie um novo [objeto bookingCustomer.](../resources/bookingcustomer.md)
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | Sem suporte.  |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /solutions/bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {code} do portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um [objeto bookingCustomer.](../resources/bookingcustomer.md)


## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customers
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.bookingCustomer",
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com",
    "addresses": [
        {
            "postOfficeBox":"",
            "street":"4567 Main Street",
            "city":"Buffalo",
            "state":"NY",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "type":"home"
        },
        {
            "postOfficeBox":"",
            "street":"4570 Main Street",
            "city":"Buffalo",
            "state":"NY",
            "countryOrRegion":"USA",
            "postalCode":"98054",
            "type":"business"
        }
    ],
    "phones": [
        {
            "number": "206-555-0100",
            "type": "home"
        },
        {
            "number": "206-555-0200",
            "type": "business"
        }
     ]
}
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.bookingCustomer",
    "@odata.context": "https://graph.microsoft.com/v1.0/solutions/$metadata#bookingBusinesses('Contosolunchdelivery%40contoso.onmicrosoft.com')/customers/$entity",
    "id": "36038f36-634e-44e4-9415-d7d59c2347aa",
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com",
    "addresses": [
        {
            "postOfficeBox":"",
            "street":"4567 Main Street",
            "city":"Buffalo",
            "state":"NY",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "type":"home"
        },
        {
            "postOfficeBox":"",
            "street":"4570 Main Street",
            "city":"Buffalo",
            "state":"NY",
            "countryOrRegion":"USA",
            "postalCode":"98054",
            "type":"business"
        }
    ],
    "phones": [
        {
            "number": "206-555-0100",
            "type": "home"
        },
        {
            "number": "206-555-0200",
            "type": "business"
        }
     ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


