---
title: Listar additionalSources
description: Obtenha a lista de fontes adicionais associadas a uma pesquisa de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 812a9500e1c56bc6fa99596499959a5855508a40
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839012"
---
# <a name="list-additionalsources"></a>Listar additionalSources
Namespace: microsoft.graph.security



Obtenha a lista de [fontes adicionais](../resources/security-datasource.md) associadas a [uma pesquisa de Descoberta Eletrônica](../resources/security-ediscoverysearch.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|eDiscovery.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/additionalSources
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

Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de [objetos microsoft.graph.security.dataSource](../resources/security-datasource.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "list_ediscoverynoncustodialdatasource"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/additionalSources
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoveryNoncustodialDataSource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/searches('c61a5860-d634-4d14-aea7-d82b6f4eb7af')/additionalSources",
    "value": [
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "43434642-3137-3138-3432-374142313639",
            "email": "AlexW@M365x809305.OnMicrosoft.com",
            "includedSources": "mailbox",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "38423145-4639-4244-4437-464630424139",
            "email": "IrvinS@M365x809305.OnMicrosoft.com",
            "includedSources": "mailbox",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "36304536-3033-3845-4639-394538443235",
            "email": "AllanD@M365x809305.OnMicrosoft.com",
            "includedSources": "mailbox",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.siteSource",
            "@odata.id": "https://graph.microsoft.com/v1.0/sites/",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "46454445-3936-3941-4145-463642313642",
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.siteSource",
            "@odata.id": "https://graph.microsoft.com/v1.0/sites/",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "37383041-3143-3731-3744-384643453341",
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.siteSource",
            "@odata.id": "https://graph.microsoft.com/v1.0/sites/",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "30394337-4541-4632-4532-423832464235",
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        }
    ]
}
```

