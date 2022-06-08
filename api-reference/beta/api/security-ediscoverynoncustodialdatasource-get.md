---
title: Obter ediscoveryNoncustodialDataSource
description: Leia as propriedades e as relações de um objeto ediscoveryNoncustodialDataSource.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 86c456a7b1321d28dd1bad215d1edc81dc09dbdb
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945116"
---
# <a name="get-ediscoverynoncustodialdatasource"></a>Obter ediscoveryNoncustodialDataSource
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/noncustodialDataSources/{ediscoveryNoncustodialDataSourceId}
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

Se bem-sucedido, este método retorna `200 OK` um código de resposta [e um objeto ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "get_ediscoverynoncustodialdatasource"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources/35393639323133394345384344303043?$expand=dataSource
```


### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryNoncustodialDataSource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/noncustodialDataSources(dataSource())/$entity",
    "status": "active",
    "holdStatus": "applied",
    "createdDateTime": "2022-05-23T02:09:11.1395287Z",
    "lastModifiedDateTime": "2022-05-23T02:09:11.1395287Z",
    "releasedDateTime": "0001-01-01T00:00:00Z",
    "id": "35393639323133394345384344303043",
    "displayName": "U.S. Sales",
    "dataSource@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/noncustodialDataSources('35393639323133394345384344303043')/dataSource/$entity",
    "dataSource": {
        "@odata.type": "#microsoft.graph.security.siteSource",
        "@odata.id": "https://graph.microsoft.com/v1.0/sites/169718e3-a8df-449d-bef4-ee09fe1ddc5d",
        "displayName": "U.S. Sales",
        "createdDateTime": "2022-05-23T02:09:11.1395535Z",
        "holdStatus": "0",
        "id": "169718e3-a8df-449d-bef4-ee09fe1ddc5d",
        "createdBy": {
            "application": null,
            "user": {
                "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                "displayName": null
            }
        },
        "site": {
            "webUrl": "https://m365x809305.sharepoint.com/sites/USSales",
            "id": "169718e3-a8df-449d-bef4-ee09fe1ddc5d",
            "createdDateTime": "2022-05-23T02:09:11.1395535Z"
        }
    }
}
```