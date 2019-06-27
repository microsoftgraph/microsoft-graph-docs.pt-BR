---
title: Obter bookingStaffMember
description: Obtenha as propriedades e os relacionamentos de um bookingStaffMember no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f2d7a8a3a01256d2cac324cc10ab5727f140a2a5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262486"
---
# <a name="get-bookingstaffmember"></a>Obter bookingStaffMember

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha as propriedades e os relacionamentos de um [bookingStaffMember](../resources/bookingstaffmember.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | Sem suporte.  |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Authorization  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.
## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingStaffMember](../resources/bookingstaffmember.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "get_bookingstaffmember"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/71d64d0e-7225-49b6-b0b1-070d476cda51
```
##### <a name="response"></a>Resposta
Este é um exemplo de resposta. Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers/$entity",
    "id": "71d64d0e-7225-49b6-b0b1-070d476cda51",
    "displayName": "Samantha Booth",
    "emailAddress": "samanthab@M365B489948.OnMicrosoft.com",
    "availabilityIsAffectedByPersonalCalendar": true,
    "colorIndex": 0,
    "role": "administrator",
    "useBusinessHours": true,
    "workingHours": [
        {
            "day": "monday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "tuesday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "wednesday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "thursday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "friday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "saturday",
            "timeSlots": []
        },
        {
            "day": "sunday",
            "timeSlots": []
        }
    ]
}
```
#### <a name="sdk-sample-code"></a>Código de amostra do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingstaffmember-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingstaffmember-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_bookingstaffmember-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingstaffmember-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingstaffmember-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingstaffmember-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
