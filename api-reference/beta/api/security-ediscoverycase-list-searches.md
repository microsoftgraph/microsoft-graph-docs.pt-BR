---
title: Listar ediscoverySearch
description: Obter a lista de pesquisas de um caso de Descoberta Eletrônica
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 5360dc3b1bce06075bde16a8e9fafd12f49922ec
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945075"
---
# <a name="list-ediscoverysearch"></a>Listar ediscoverySearch
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha a lista de [recursos ediscoverySearch](../resources/security-ediscoverysearch.md) de um [objeto eDiscoveryCase](../resources/security-ediscoverycase.md) .

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
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches
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

Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção [de objetos ediscoverySearch](../resources/security-ediscoverysearch.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "list_ediscoverysearch"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches
```


### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoverySearch)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/searches",
    "value": [
        {
            "dataSourceScopes": "none",
            "description": "My first search",
            "lastModifiedDateTime": "2022-05-23T04:38:07.5787454Z",
            "contentQuery": "(Author=\"edison\")",
            "id": "46867792-68e6-41db-9cd0-f651c2290d91",
            "displayName": "My search 2",
            "createdDateTime": "2022-05-23T04:38:07.5787454Z",
            "lastModifiedBy": null,
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                },
                "application": {
                    "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
                    "displayName": "Graph Explorer"
                }
            }
        },
        {
            "dataSourceScopes": "none",
            "description": "My first search",
            "lastModifiedDateTime": "2022-05-23T04:35:36.5424818Z",
            "contentQuery": "(Author=\"edison\")",
            "id": "80b9d59a-12a6-4273-a3d4-ab78f9a04ea5",
            "displayName": "My search 1",
            "createdDateTime": "2022-05-23T04:35:36.5424818Z",
            "lastModifiedBy": null,
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                },
                "application": {
                    "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
                    "displayName": "Graph Explorer"
                }
            }
        }
    ]
}
```

