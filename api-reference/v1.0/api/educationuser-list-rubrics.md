---
title: Listar rubricas
description: Recupere uma lista de objetos educationrubric.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1ad3b67a0438542b04e78ac47b4de2a23f0d33fb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59114579"
---
# <a name="list-rubrics"></a>Listar rubricas

Namespace: microsoft.graph

Recupere uma lista de [objetos educationRubric.](../resources/educationrubric.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/rubrics
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

Não fornece um corpo de solicitação para este método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos educationRubric](../resources/educationrubric.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rubrics"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/me/rubrics
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rubrics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rubrics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rubrics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rubrics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "displayName":"Example Credit Rubric",
            "id":"c4459fcb-a761-4f70-ac5b-e9466cb77c2a",
            "description":{
                "content":"This is an example of a credit rubric (no points)",
                "contentType":"text"
            },
            "levels":[
                {
                    "levelId":"dec665d4-cf1b-4481-ac61-1d5b6188f4f5",
                    "displayName":"Good",
                    "description":{
                        "content":"",
                        "contentType":"text"
                    }
                },
                {
                    "levelId":"3f2e4b0f-508e-4005-984b-17e061bc5377",
                    "displayName":"Poor",
                    "description":{
                        "content":"",
                        "contentType":"text"
                    }
                }
            ],
            "qualities":[
                {
                    "qualityId":"dc79dcbf-b536-4797-9c5b-902f28129fd0",
                    "description":{
                        "content":"Argument",
                        "contentType":"text"
                    },
                    "criteria":[
                        {
                            "id":"8937fa15-4a7c-4f27-bd01-ca3471d2d1d5",
                            "description":{
                                "content":"The essay's argument is persuasive.",
                                "contentType":"text"
                            }
                        },
                        {
                            "id":"4dfb5263-1d3f-4f0a-93ef-d24d800d0f69",
                            "description":{
                                "content":"The essay's argument does not make sense.",
                                "contentType":"text"
                            }
                        }
                    ]
                },
                {
                    "qualityId":"7e087062-ac25-4629-8386-a946350936db",
                    "description":{
                        "content":"Spelling and Grammar",
                        "contentType":"text"
                    },
                    "criteria":[
                        {
                            "id":"12276eb2-122c-4ad2-ba92-335ea798c88e",
                            "description":{
                                "content":"The essay uses proper spelling and grammar with few or no errors.",
                                "contentType":"text"
                            }
                        },
                        {
                            "id":"3db7e6b2-2b1b-4f8e-9fca-bea701159145",
                            "description":{
                                "content":"The essay has numerous errors in spelling and/or grammar.",
                                "contentType":"text"
                            }
                        }
                    ]
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rubrics",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


