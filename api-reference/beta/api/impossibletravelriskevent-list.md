---
title: Listar impossibleTravelRiskEvents
description: Recupere uma lista de objetos impossibletravelriskevent.
localization_priority: Normal
doc_type: apiPageType
author: cloudhandler
ms.prod: identity-and-sign-in
ms.openlocfilehash: 5ab2f3a075a248d0d8b2bcea1bcc2290fc0fac7e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435095"
---
# <a name="list-impossibletravelriskevents-deprecated"></a>Listar impossibleTravelRiskEvents (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020. Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

Recupere uma lista de objetos impossibletravelriskevent.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | IdentityRiskEvent.Read.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | IdentityRiskEvent.Read.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /impossibleTravelRiskEvents
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Workbook-Session-Id  | ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "get_impossibletravelriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/impossibleTravelRiskEvents
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 313

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.impossibleTravelRiskEvent",
      "closedDateTime": "2016-01-29T20:03:57.7872426Z",
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab",
      "ipAddress": "176.10.104.240",
      "isAtypicalLocation": true,
      "location": "Bern, CH",
      "previousIPAddress": "95.31.18.119",
      "previousLocation": "Moskva, Russia, RU",
      "previousSigninDateTime": "2016-01-29T00:00:55.3859274Z",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "ImpossibleTravelRiskEvent",
      "userAgent": "Mozilla",
      "userDisplayName": "Jon Doe",
      "userId": "0bfdc7a8-6a16-c33e-7de9-a60a28ae533b",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List impossibleTravelRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


