---
title: Usar a API de Pesquisa da Microsoft no Microsoft Graph para solicitar correções ortográficas
description: Você pode usar a API de Pesquisa da Microsoft para obter a sugestão ortográfica ou a modificação ortográfica para a consulta de pesquisa.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 9d7f935f2de7e0777679266fc479b302fcfaf2a9
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067660"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-request-spelling-correction-preview"></a>Use a API de Pesquisa da Microsoft no Microsoft Graph para solicitar correção ortográfica (visualização)

Você pode usar a API de Pesquisa da Microsoft para solicitar correções ortográficas para lidar com incompatibilidades entre erros de digitação em consultas do usuário e palavras corretas em conteúdos matched. Para solicitar correções ortográficas, especifique as seguintes propriedades na **propriedade queryAlterationOptions** do corpo da solicitação do [método de](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) consulta:

- **enableSuggestion** to enable/disable spelling suggestions for the user query. Você pode passar `true` para obter as informações de correção ortográfica sugeridas para erros de digitação na consulta do usuário.

- **enableModification** para habilitar/desabilitar modificações ortográficas para a consulta do usuário. Você pode passar para obter os resultados da pesquisa para a consulta corrigida quando não houver resultados para a consulta original com erros de digitação e obter as informações de `true` correção correspondentes. 

A prioridade da modificação ortográfica é maior do que a sugestão ortográfica se ambas estão habilitadas.

Todas as cadeias de caracteres de consulta do usuário devem ser as mesmas para habilitar correções ortográficas para pesquisas de várias entidades.

## <a name="example-1-request-spelling-suggestions"></a>Exemplo 1: Solicitar sugestões ortográficas

O exemplo a seguir consulta **recursos listItem** que contêm a cadeia de caracteres "accountt" e solicita uma sugestão ortográfica para a consulta.

A resposta contém [objetos alterationResponse](/graph/api/resources/alterationResponse?view=graph-rest-beta&preserve-view=true) para a sugestão ortográfica.

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
            "size": 25
        }
    ],
    "queryAlterationOptions": {
        "enableSuggestion": true,
        "enableModification": false
    }
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
        "queryAlterationType": "Suggestion"
    }
}
```

## <a name="example-2-request-spelling-modifications"></a>Exemplo 2: Solicitar modificações ortográficas

O exemplo a seguir consulta **recursos listItem** que contêm a cadeia de caracteres "accountt" e solicita uma modificação ortográfica para a consulta.

Neste exemplo, não há resultados para consulta original com typo "accountt". A resposta contém resultados relacionados aos objetos "account" e [alterationResponse](/graph/api/resources/alterationResponse?view=graph-rest-beta&preserve-view=true) da cadeia de caracteres corrigidos para a modificação ortográfica.

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
            "size": 25
        }
    ],
    "queryAlterationOptions": {
        "enableSuggestion": true,
        "enableModification": true
    }
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
```

## <a name="known-limitations"></a>Limitações conhecidas

A correção ortográfica só é suportada para os seguintes recursos: **message**, **event**, **site**, **drive**, **driveItem**, **list**, **listItem** **e externalItem**.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
