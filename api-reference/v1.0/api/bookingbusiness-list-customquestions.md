---
title: Listar customQuestions
description: Obter os recursos bookingCustomQuestion associados a um bookingBusiness.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: aff86534505575fc047118890abc936d78072743
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525007"
---
# <a name="list-customquestions"></a>Listar customQuestions

Namespace: microsoft.graph

Obter os [recursos bookingCustomQuestion](../resources/bookingcustomquestion.md) associados a [um bookingBusiness](../resources/bookingbusiness.md).

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                    |
| :------------------------------------- | :----------------------------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                                                                 |
| Aplicativo                            | Sem suporte.                                                                 |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}-->

```http
GET /bookingBusinesses/{bookingBusinessesId}/customQuestions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, consulte $count e $expand parâmetros de consulta [OData.](/graph/query-parameters)

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [bookingCustomQuestion](../resources/bookingcustomquestion.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customQuestions
```

### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomQuestion",
  "isCollection": true
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "@odata.type": "#microsoft.graph.bookingCustomQuestion",
        "id": "3bc6fde0-4ad3-445d-ab17-0fc15dba0774",
        "displayName": "What is your age?",
        "answerInputType": "text",
        "answerOptions": [],
    },
    {
        "@odata.type": "#microsoft.graph.bookingCustomQuestion",
        "id": "dbb865a6-530d-46e1-8e88-5d76789034b2",
        "displayName": "What is your nationality?",
        "answerInputType": "radioButton",
        "answerOptions": [
          "US",
          "UK",
          "Canada",
          "India"
        ],
    }
  ]
}
```
