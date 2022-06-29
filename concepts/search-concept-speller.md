---
title: Usar a API de Pesquisa da Microsoft para solicitar correções ortográficas
description: Use a API de Pesquisa da Microsoft no Microsoft Graph para solicitar correções ortográficas para lidar com incompatibilidades entre erros de digitação em consultas de usuário e palavras corretas em conteúdos correspondentes.
author: nmoreau
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 16375f1c0e38cc5e0acf3f2f89e668d32a042e51
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438259"
---
# <a name="use-the-microsoft-search-api-to-request-spelling-corrections"></a>Usar a API de Pesquisa da Microsoft para solicitar correções ortográficas

Você pode usar a API de Pesquisa da Microsoft no Microsoft Graph para solicitar correções ortográficas para lidar com incompatibilidades entre erros de digitação em consultas de usuário e palavras corretas em conteúdos correspondentes. Para solicitar correções ortográficas, especifique as seguintes propriedades na **propriedade queryAlterationOptions** da [searchRequest](/graph/api/resources/searchrequest):

- **enableSuggestion** para habilitar/desabilitar sugestões de ortografia para a consulta do usuário. Você pode passar para `true` obter as informações de correção ortográfica sugeridas para erros de digitação na consulta do usuário.

- **enableModification** para habilitar/desabilitar modificações de ortografia para a consulta do usuário. Você pode passar `true` para obter os resultados da pesquisa para a consulta corrigida  quando não houver resultados para a consulta original com erros de digitação e obter as informações de correção correspondentes.

A prioridade de modificação ortográfica será maior do que a sugestão ortográfica se ambas estiverem habilitadas.

Todas as cadeias de caracteres de consulta do usuário devem ser iguais para habilitar correções ortográficas para pesquisas de várias entidades.

## <a name="example-1-request-spelling-suggestions"></a>Exemplo 1: solicitar sugestões de ortografia

O exemplo a seguir consulta **recursos listItem que contêm** `accountt` a cadeia de caracteres e solicita uma sugestão de ortografia para a consulta.

A resposta contém [objetos alterationResponse](/graph/api/resources/alterationResponse) para a sugestão de ortografia.

### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "listItem"
            ],
            "query": {
                "queryString": "accountt"
            },
            "from": 0,
            "size": 25,
            "queryAlterationOptions": {
                "enableSuggestion": true,
                "enableModification": false
            }
        }
    ]
}
```

### <a name="response"></a>Resposta

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "searchTerms": [
                "accountt"
            ],
            "hitsContainers": [
                {
                    "total": 0,
                    "moreResultsAvailable": false
                }
            ],
            "queryAlterationResponse": {
                "@odata.type": "#microsoft.substrateSearch.alterationResponse",
                "originalQueryString": "accountt",
                "queryAlteration": {
                    "@odata.type": "#microsoft.substrateSearch.searchAlteration",
                    "alteredQueryString": "account",
                    "alteredHighlightedQueryString": "account",
                    "alteredQueryTokens": [
                        {
                            "offset": 0,
                            "length": 8,
                            "suggestion": "account"
                        }
                    ]
                },
                "queryAlterationType": "Suggestion"
            }
        }
    ]
}
```

## <a name="example-2-request-spelling-modifications"></a>Exemplo 2: solicitar modificações ortográficas

O exemplo a seguir consulta **recursos listItem que contêm** `accountt` a cadeia de caracteres e solicita uma modificação ortográfica para a consulta.

Neste exemplo, não há resultados para a consulta original com erro de digitação `accountt`. A resposta contém resultados relacionados à cadeia de caracteres corrigida `account` e [aos objetos alterationResponse](/graph/api/resources/alterationResponse) para a modificação ortográfica.

### <a name="request"></a>Solicitação

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "listItem"
            ],
            "query": {
                "queryString": "accountt"
            },
            "from": 0,
            "size": 25,
            "queryAlterationOptions": {
                "enableSuggestion": true,
                "enableModification": true
            }
        }
    ]
}
```

### <a name="response"></a>Resposta

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "searchTerms": [
                "account"
            ],
            "hitsContainers": [
                {
                    "total": 1,
                    "moreResultsAvailable": false,
                    "hits": [
                        {
                            "hitId": "FlULeN/ui/1GjLx1rUfio5UAAEl",
                            "rank": 1,
                            "summary": "",
                            "resource": {
                                "@odata.type": "#microsoft.graph.listItem",
                                "createdDateTime": "2019-06-10T06:37:43Z",
                                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                                "name": "web_part_test_long Notebook",
                                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/Lists/Issue tracker list/DispForm.aspx?ID=1",
                                "sharepointIds": {
                                    "listId": "33498de0-d695-4d23-ac26-e1bf95a3206e",
                                    "listItemId": "13"
                                },
                                "createdBy": {
                                    "user": {
                                        "displayName": "System Account"
                                    }
                                },
                                "lastModifiedBy": {
                                    "user": {
                                        "displayName": "System Account"
                                    }
                                },
                                "parentReference": {
                                    "sharepointIds": {
                                        "listId": "da61a2b0-4120-4a3f-812b-0fc0d79bf16b"
                                    },
                                    "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
                                }
                            }
                        }
                    ]
                }
            ],
            "queryAlterationResponse": {
                "@odata.type": "#microsoft.substrateSearch.alterationResponse",
                "originalQueryString": "accountt",
                "queryAlteration": {
                    "@odata.type": "#microsoft.substrateSearch.searchAlteration",
                    "alteredQueryString": "account",
                    "alteredHighlightedQueryString": "account",
                    "alteredQueryTokens": [
                        {
                            "offset": 0,
                            "length": 8,
                            "suggestion": "account"
                        }
                    ]
                },
                "queryAlterationType": "Modification"
            }
        }
    ]
}
```

## <a name="known-limitations"></a>Limitações conhecidas

A correção ortográfica só tem suporte para os seguintes recursos: **mensagem****, evento**, **site**, **unidade**, **driveItem**, **lista**, **listItem** e **externalItem**.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview)
