---
title: 'reportRoot: getCredentialUsageSummary'
description: Relatar o estado atual de quantos usuários em sua organização estão usando recursos de redefinição de senha de autoatendado.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 56015afd7bc5589d518277df555ac511b7f91657
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131352"
---
# <a name="reportroot-getcredentialusagesummary"></a>reportRoot: getCredentialUsageSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Relatar o estado atual de quantos usuários em sua organização usaram os recursos de redefinição de senha de autoatendado.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Reports.Read.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Reports.Read.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUsageSummary
```

## <a name="function-parameters"></a>Parâmetros de função

Você pode usar o parâmetro de função a seguir para ajustar a resposta.

| Parâmetro | Tipo | Descrição |
|:--------- |:---- |:----------- |
| ponto | String | Especifica o período de tempo para o qual você precisa dos dados de uso. Por exemplo: `/reports/getCredentialUsageSummary(period='D30')`. Períodos com suporte: `D1` `D7` , e `D30` . O ponto não faz falta de maiúsculas e minúsculas. |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esta função dá suporte ao parâmetro opcional de consulta OData **$filter**. Você pode aplicar **$filter** em uma ou mais das seguintes propriedades do [recurso credentialUsageSummary.](../resources/credentialusagesummary.md)

| Propriedades | Descrição e exemplo |
|:---- |:----------- |
| recurso | Especifica o tipo de dados de uso que você deseja (registro versus redefinição). Por exemplo: `/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`. Operadores de filtro com suporte: `eq` . |

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | Portador {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta e um novo objeto da coleção `200 OK` [credentialUsageSummary](../resources/credentialusagesummary.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialusagesummary"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialusagesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialusagesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialusagesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getcredentialusagesummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades são retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getCredentialUsageSummary)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "successfulActivityCount":12345,
      "failureActivityCount": 123,
      "authMethod": "email"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reportRoot: getCredentialUsageSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


