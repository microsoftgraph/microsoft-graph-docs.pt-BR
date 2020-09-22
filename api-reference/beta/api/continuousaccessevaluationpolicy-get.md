---
title: Obter continuousAccessEvaluationPolicy
description: Ler as propriedades de um objeto continuousAccessEvaluationPolicy.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bea54ea801ee9d41314f1fbd2c87070ac4e92773
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023403"
---
# <a name="get-continuousaccessevaluationpolicy"></a>Obter continuousAccessEvaluationPolicy
Namespace: Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e os relacionamentos de um objeto [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)     | Policy.Read.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Policy.Read.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {  "blockType": "ignored"} -->
``` http
GET /identity/continuousAccessEvaluationPolicy
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte ao parâmetro de consulta OData ' $select ' para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get_continuousaccessevaluationpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
```


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy"
} -->

``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/continuousAccessEvaluationPolicy/$entity",
  "id": "00000000-0000-0000-0000-000000000006",
  "description": "Continuous Access Evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.",
  "displayName": "Continuous Access Evaluation",
  "isEnabled": true,
  "users": [ "1608be63-df14-42a4-8932-1c9d963b026f" ],
  "groups": [ "4308b567-df14-0000-8932-1c9d963b026f" ]
}
```
