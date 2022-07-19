---
title: Listar lastIndexOperation
description: Obtenha uma lista de ediscoveryIndexOperations associada a um ediscoveryCustodian.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 725644ef9b266d52022fb51974163a2cd610e254
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839213"
---
# <a name="list-lastindexoperation"></a>Listar lastIndexOperation
Namespace: microsoft.graph.security



Obtenha uma lista de [ediscoveryIndexOperations](../resources/security-ediscoveryindexoperation.md) associada a [um ediscoveryCustodian](../resources/security-ediscoverycustodian.md).

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
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians/{ediscoverycustodianId}/lastIndexOperation
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/noncustodialSources/{ediscoveryNoncustodialDataSourceId}/lastIndexOperation
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

Se bem-sucedido, este método `200 OK` retorna um código de resposta e uma coleção de [objetos microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "list_ediscoveryindexoperation"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/lastIndexOperation
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryIndexOperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.security.ediscoveryIndexOperation",
    "createdDateTime": "2022-05-23T02:35:43.1932326Z",
    "completedDateTime": "0001-01-01T00:00:00Z",
    "percentProgress": 0,
    "status": "running",
    "action": "index",
    "id": "b23821836460441891d16a2cb7463392",
    "createdBy": {
        "application": null,
        "user": {
            "id": null,
            "displayName": null,
            "userPrincipalName": "c25c3914-f9f7-43ee-9cba-a25377e0cec6"
        }
    }
}
```

