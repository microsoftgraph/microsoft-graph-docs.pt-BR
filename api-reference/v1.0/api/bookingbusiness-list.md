---
title: Listar bookingBusinesses
description: Obtenha uma coleção de objetos bookingBusiness que foram criados para o locatário.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: deed802ca412e3b44e4e16e2798fb82af60ae6ab
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856019"
---
# <a name="list-bookingbusinesses"></a>Listar bookingBusinesses

Namespace: microsoft.graph

Obtenha uma coleção de [objetos bookingBusiness](../resources/bookingbusiness.md) que foram criados para o locatário.

Essa operação retorna apenas a **ID e** **displayName** de cada Microsoft Bookings negócios na coleção. Para considerações de desempenho, ele não retorna outras propriedades. Você pode obter as outras propriedades de uma empresa do Bookings especificando sua **ID em** uma [operação GET](bookingbusiness-get.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | BookingsAppointment.ReadWrite.All, Bookings.Read.All  |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /solutions/bookingBusinesses
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método dá suporte aos $count e $expand de consulta [OData](/graph/query-parameters) para ajudar a personalizar a resposta.

Esse método também dá suporte ao parâmetro `query` que aceita um valor de cadeia de caracteres. Esse parâmetro limita os resultados GET a empresas que correspondem à cadeia de caracteres especificada. Para obter mais detalhes, consulte [o exemplo](#request-2).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Authorization  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `200 OK` de resposta e uma coleção de [objetos bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-bookings-businesses-in-a-tenant"></a>Exemplo 1: Obter empresas do Bookings em um locatário

#### <a name="request-1"></a>Solicitação 1

O exemplo a seguir obtém as empresas do Bookings em um locatário.

<!-- {
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses
```

#### <a name="response-1"></a>Resposta 1

Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/solutions/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"Contosolunchdelivery@contoso.onmicrosoft.com",
            "displayName":"Contoso lunch delivery",
        },
        {
            "id":"Fabrikam@contoso.onmicrosoft.com",
            "displayName":"Fabrikam",
        }
    ]
}
```

### <a name="example-2-use-query-to-get-one-or-more-matching-bookings-businesses-in-a-tenant"></a>Exemplo 2: usar 'query' para obter uma ou mais empresas do Bookings correspondentes em um locatário

#### <a name="request-2"></a>Solicitação 2

O exemplo a seguir mostra como usar o parâmetro `query` para obter uma ou mais empresas do Bookings correspondentes no locatário.

<!-- {
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses?query=Adventure
```

#### <a name="response-2"></a>Resposta 2

Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/solutions/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"AdventureWorksCycles@M365B960066.onmicrosoft.com",
            "displayName":"Adventure Works Cycles",
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
