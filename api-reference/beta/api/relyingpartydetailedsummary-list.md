---
title: Listar relyingPartyDetailedSummary
description: Recupere uma lista de objetos relyingPartyDetailedSummary.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 7512cc10db5b37cce6c899f5399f0c51194ab59c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131380"
---
# <a name="list-relyingpartydetailedsummary"></a>Listar relyingPartyDetailedSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de **objetos relyingPartyDetailedSummary.**

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Report.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Application                            | Report.Read.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getRelyingPartyDetailedSummary
```
## <a name="function-parameters"></a>Parâmetros de função

| Parâmetro | Descrição |
|:----------|:----------|
| ponto | Os valores com suporte são: D1, D7, D30. Eles seguem o formato Dn, em que n representa o número de dias em que o relatório é agregado.|

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. 

- Você pode usar o `$filter` parâmetro para filtrar por relyingPartyId, migrationStatus e outros atributos. Por exemplo, $filter= relyingPartyId eq 'identifier'.
- Você pode usar `$orderby` , `$top` e `$skip` parâmetros de consulta em qualquer solicitação GET.

Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).


## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {código}. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta e o objeto `200 OK` [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) solicitado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_relyingpartydetailedsummary"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getRelyingPartyDetailedSummary(period='period_value')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-relyingpartydetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-relyingpartydetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-relyingpartydetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-relyingpartydetailedsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1fec2821-6c43-4919-9560-ce36c820faa5",
  "relyingPartyId": "https://contosoorg-dev-ed.my.contoso.com",
  "serviceId": "287ed092-c182-4748-99a9-9ef3b5a0a0f9",
  "relyingPartyName": "contoso",
  "successfulSignInCount": 90,
  "failedSignInCount": 10,
  "totalSignInCount": 100,
  "signInSuccessRate":90.0,
  "uniqueUserCount": 10,
  "migrationStatus": "ready",
  "replyUrls": [
      "https://contosoorg-dev-ed.my.contoso.com"
  ],
  "migrationValidationDetails": [
      {
          "name": "AdditionalWSFedEndpointCheckResult",
          "value": "{\"result\": 0, \"message\": \"No additional WS-Federation endpoints were found.\"}"
      }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get relyingPartyDetailedSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


