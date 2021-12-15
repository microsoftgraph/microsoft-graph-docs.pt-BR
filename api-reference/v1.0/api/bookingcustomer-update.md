---
title: Atualizar bookingCustomer
description: Atualize as propriedades de um objeto bookingCustomer.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d1576887ff634aa955246e63c3f57b560fc263d3
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525008"
---
# <a name="update-bookingcustomer"></a>Atualizar bookingCustomer

Namespace: microsoft.graph

Atualize as propriedades de um [objeto bookingCustomer.](../resources/bookingcustomer.md)
## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegada (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | Sem suporte.  |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:-----------|:-----------|
| Authorization  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|addresses|[Coleção physicalAddress](../resources/physicaladdress.md)|Endereços associados ao cliente. O tipo **de** atributo physicalAddress não é suportado em v1.0. Internamente, mapeemos os endereços para o tipo `others` .|
|displayName|Cadeia de caracteres|O nome do cliente.|
|emailAddress|String|O endereço SMTP do cliente.|
|telefones|Coleção [phone](../resources/phone.md)|Telefone números associados ao cliente, incluindo números móveis, comerciais e de residência.|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [bookingCustomer](../resources/bookingcustomer.md) atualizado no corpo da resposta.
## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- {
  "blockType": "request"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.bookingCustomer",
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```

### <a name="response"></a>Resposta
Eis um exemplo da resposta. Observação: o objeto de resposta exibido aqui pode ser reduzido para facilitar a leitura.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.bookingCustomer",
    "@odata.context": "https://graph.microsoft.com/v1.0/solutions/$metadata#bookingBusinesses('Contosolunchdelivery%40contoso.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


