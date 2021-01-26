---
title: 'searchEntity: query'
description: Executa a consulta especificada no corpo da solicitação. Os resultados da pesquisa são fornecidos na resposta.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: e675b9b9301e7b0fc918c4631757a9bb21f82ce7
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983759"
---
# <a name="searchentity-query"></a>searchEntity: query

Namespace: microsoft.graph

Executa a consulta especificada no corpo da solicitação. Os resultados da pesquisa são fornecidos na resposta.


## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference). 

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Mail.Read, Mail.ReadWrite, Calendars.Read, Calendars.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All, ExternalItem.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

```HTTP
POST /search/query
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo        | Descrição |
|:-------------|:------------|:------------|
|requests|[Coleção searchRequest](../resources/searchrequest.md)|Uma coleção de uma ou mais solicitações de pesquisa cada formatada em um blob JSON. Cada blob JSON contém os tipos de recursos esperados na resposta, as fontes subjacentes, os parâmetros de paging, os campos solicitados e a consulta de pesquisa real. <br> Esteja ciente das [limitações conhecidas](../resources/search-api-overview.md#known-limitations) em pesquisar combinações específicas de tipos de entidade e classificar ou agregar resultados de pesquisa. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta e um objeto da coleção `HTTP 200 OK` [searchResponse](../resources/searchresponse.md) no corpo da resposta.
 

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "message"
      ],
      "query": {
        "queryString": "contoso"
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.searchResponse",
  "isCollection": true
} -->

```HTTP
HTTP/1.1 200 OK
Content-type: application/json
```

```json
{
    "value": [
        {
            "searchTerms": [
                "searchTerms-value"
            ],
            "hitsContainers": [
                {
                    "hits": [
                        {
                            "hitId": "AAMkADdmODdhN2NjLTMwZWYtNDBiNy1iMDYxLWZhZTkyOGM4YmRhZABGAAAAAACsLZF5BeQoRLYm4UlvnOXZBwCav2PZy/7/R52ssyzmS9f0AAAAAAEMAACav2PZy/7/R52ssyzmS9f0AABM0pr/AAA=",
                            "rank": 1,
                            "summary": "...Identity Protection Weekly Digest <c0>Contoso</c0> New risky users detected <https://azure.microsoft.com/email/?destination=https%3A%2F%2Fportal.azure.com%2Fcontoso.com%23blade%2FMicrosoft_AAD_IAM%2FIdentityProtectionMenuBlade%2FRiskyUsers%2F...",
                            "resource": {
                                "@odata.type": "#microsoft.graph.message",
                                "createdDateTime": "2020-11-17T16:02:34Z",
                                "lastModifiedDateTime": "2020-11-17T16:02:37Z",
                                "changeKey": "CQAAAA==",
                                "receivedDateTime": "2020-11-17T16:02:34Z",
                                "sentDateTime": "2020-11-17T16:02:27Z",
                                "hasAttachments": false,
                                "internetMessageId": "<1e506769-c6da-4f44-bb54-6ba1bd59d300@az.northcentralus.production.microsoft.com>",
                                "subject": "Azure AD Identity Protection Weekly Digest",
                                "bodyPreview": "...Identity Protection Weekly Digest Contoso New risky users detected <https://azure.microsoft.com/email/?destination=https%3A%2F%2Fportal.azure.com%2Fcontoso.com%23blade%2FMicrosoft_AAD_IAM%2FIdentityProtectionMenuBlade%2FRiskyUsers%2F...",
                                "importance": "normal",
                                "parentFolderId": "AQMkADdmODdhN2NjAC0zMGVmLTQwYjctYjA2MS1mYWU5MjhjOGJkYWQALgAAA6wtkXkF5ChEtibhSW+c5dkBAJq/Y9nL/v9HnayzLOZL1/QAAAIBDAAAAA==",
                                "conversationId": "AAQkADdmODdhN2NjLTMwZWYtNDBiNy1iMDYxLWZhZTkyOGM4YmRhZAAQAKQ6a/rTEmVCtGMTER183jw=",
                                "isRead": false,
                                "isDraft": false,
                                "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADdmODdhN2NjLTMwZWYtNDBiNy1iMDYxLWZhZTkyOGM4YmRhZABGAAAAAACsLZF5BeQoRLYm4UlvnOXZBwCav2PZy%2F7%2FR52ssyzmS9f0AAAAAAEMAACav2PZy%2F7%2FR52ssyzmS9f0AABM0pr%2FAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
                                "inferenceClassification": "focused",
                                "replyTo": [
                                    {
                                        "emailAddress": {
                                            "name": "MOD Administrator"
                                        }
                                    }
                                ],
                                "sender": {
                                    "emailAddress": {
                                        "name": "Microsoft Azure",
                                        "address": "azure-noreply@contoso.com"
                                    }
                                },
                                "from": {
                                    "emailAddress": {
                                        "name": "Microsoft Azure",
                                        "address": "azure-noreply@contoso.com"
                                    }
                                }
                            }
                        }
                    ],
                    "total": 47,
                    "moreResultsAvailable": true
                }
            ]
        }
    ]
}
```

## <a name="see-also"></a>Confira também
- Pesquisar [mensagens de email](/graph/search-concept-messages)
- Pesquisar [eventos de calendário](/graph/search-concept-events)
- Pesquisar conteúdo no SharePoint e no OneDrive[(arquivos, listas e sites)](/graph/search-concept-files)
- Pesquisar [dados de tipos personalizados (Conectores do Graph)](/graph/search-concept-custom-types)


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


