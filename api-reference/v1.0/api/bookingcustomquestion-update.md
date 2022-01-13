---
title: Atualizar bookingCustomQuestion
description: Atualize as propriedades de um objeto bookingCustomQuestion.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 0dd66a2edc1416dd5cae89752063ae39fb41a319
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014107"
---
# <a name="update-bookingcustomquestion"></a>Atualizar bookingCustomQuestion

Namespace: microsoft.graph

Atualize as propriedades de um [objeto bookingCustomQuestion.](../resources/bookingcustomquestion.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                    |
| :------------------------------------- | :----------------------------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                                                 |
| Aplicativo                            | Sem suporte.                                                                 |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /solutions/bookingBusinesses/{bookingBusinessesId}/customQuestions/{bookingCustomQuestionId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                 |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Propriedade        | Tipo              | Descrição                                                                                                         |
| :-------------- | :---------------- | :------------------------------------------------------------------------------------------------------------------ |
| answerInputType | answerInputType   | O tipo de resposta esperado. Os valores possíveis são: `text`, `radioButton`, `unknownFutureValue`. Opcional.    |
| answerOptions   | Coleção de cadeias de caracteres | Lista de valores de resposta possíveis. Opcional.                                                                   |
| displayName     | String            | A pergunta. Obrigatório. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto bookingCustomQuestion](../resources/bookingcustomquestion.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customQuestions/91f1ef26-ca00-451c-1c64-8f3560c80d3d
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.bookingCustomQuestion",
  "displayName": "What is your age?",
  "answerInputType": "text",
  "answerOptions": []
}
```

### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomQuestion"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.bookingCustomQuestion",
  "id": "91f1ef26-ca00-451c-1c64-8f3560c80d3d",
  "displayName": "What is your age?",
  "answerInputType": "text",
  "answerOptions": []
}
```
