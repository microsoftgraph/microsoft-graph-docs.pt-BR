---
title: Obter applicationSignInSummary
description: Recupere as propriedades e os relacionamentos de um objeto **applicationSigninSummary** .
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2fe08254384c4ff7123e3876ba2286068d2ddb28
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322877"
---
# <a name="get-applicationsigninsummary"></a>Obter applicationSignInSummary

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e os relacionamentos de um objeto [applicationSigninSummary](../resources/applicationsigninsummary.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Report. Read. All |
|Delegado (conta pessoal da Microsoft) | Sem suporte   |
|Aplicativo | Report. Read. All | 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
``` http
reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a>Parâmetros de função

| Parâmetro | Descrição |
|:----------|:----------|
| ponto | `D7` (Últimos sete dias) ou `D30` (últimos 30 dias); outros valores geram erros. |

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Authorization | Portador {código} |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [applicationSignInSummary](../resources/applicationsigninsummary.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** O objeto Response mostrado aqui mmight ser reduzido para facilitar a leitura. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationSignInSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "appId": "appId-value",
  "appDisplayName": "appDisplayName-value",
  "successfulSignInCount": 99,
  "failedSignInCount": 99,
  "successPercentage": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
