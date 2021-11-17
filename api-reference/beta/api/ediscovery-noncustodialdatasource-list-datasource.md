---
title: Listar dadosSource
description: Obter os recursos dataSource da propriedade de navegação dataSource.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: c349a4bb4b705c84a1d9995368353c1f7a014496
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60998805"
---
# <a name="list-datasource"></a>Listar dadosSource

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter a lista de dadosSources associados a uma fonte de dados não custodial.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/noncustodialDataSources/{noncustodialDataSourceId}/dataSource
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos dataSource](../resources/ediscovery-datasource.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_datasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources/8e402dd7f3c94a3abc086e5d07db1c6d/datasource
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-datasource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-datasource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-datasource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-datasource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-datasource-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.dataSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/noncustodialDataSources('8e402dd7f3c94a3abc086e5d07db1c6d')/dataSource/$entity",
        "@odata.type": "#microsoft.graph.ediscovery.userSource",
        "displayName": "Adele Vance",
        "createdDateTime": "2021-02-17T19:41:22.5902664Z",
        "id": "8e402dd7f3c94a3abc086e5d07db1c6d",
        "email": "AdeleV@contoso.com",
        "includedSources": "mailbox",
        "createdBy": {
            "user": {
                "id": "ediscovery admin",
                "displayName": "c1db6f13-332a-4d84-b111-914383ff9fc9"
            }
        }
      }
  ]

}
```
