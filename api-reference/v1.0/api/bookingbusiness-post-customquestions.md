---
title: Criar bookingCustomQuestion
description: Crie um novo objeto bookingCustomQuestion.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 056de1e6db71fea98fea3023fc852843102dd34f
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014198"
---
# <a name="create-bookingcustomquestion"></a>Criar bookingCustomQuestion

Namespace: microsoft.graph

Crie um novo [objeto bookingCustomQuestion.](../resources/bookingcustomquestion.md)

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
}-->

```http
POST /solutions/bookingBusinesses/{bookingBusinessesId}/customQuestions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                 |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON de um [objeto bookingCustomQuestion.](../resources/bookingcustomquestion.md)

Você pode especificar as seguintes propriedades ao criar **um bookingCustomQuestion**.

| Propriedade        | Tipo              | Descrição                                                                                                         |
| :-------------- | :---------------- | :------------------------------------------------------------------------------------------------------------------ |
| answerInputType | answerInputType   | O tipo de resposta esperado. Os valores possíveis são: `text`, `radioButton`, `unknownFutureValue`. Opcional.    |
| answerOptions   | Coleção de cadeias de caracteres | Lista de valores de resposta possíveis. Opcional.                                                                     |
| displayName     | String            | A pergunta. Obrigatório. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto bookingCustomQuestion](../resources/bookingcustomquestion.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request"
}
-->

```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customQuestions/
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.bookingCustomQuestion",
  "displayName": "What is your age?",
  "answerInputType": "text",
  "answerOptions" : []
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
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.bookingCustomQuestion",
  "id": "3bc6fde0-4ad3-445d-ab17-0fc15dba0774",
  "displayName": "What is your age?",
  "answerInputType": "text",
  "answerOptions": [],
}
```
