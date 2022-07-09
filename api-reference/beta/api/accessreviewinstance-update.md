---
title: Atualizar accessReviewInstance
description: Atualize as propriedades de um objeto accessReviewInstance.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 72ebfe8f84d73e2c64ee27f2e8deb2eae8fbd2ad
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697320"
---
# <a name="update-accessreviewinstance"></a>Atualizar accessReviewInstance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [um objeto accessReviewInstance](../resources/accessreviewinstance.md) . Somente as **propriedades reviewers** e **fallbackReviewers** podem ser atualizadas, mas a propriedade **de** escopo também é necessária no corpo da solicitação. Você só pode adicionar revisores à propriedade **fallbackReviewers** , mas não pode remover **fallbackReviewers existentes**.

Para atualizar um **accessReviewInstance**, seu **status** deve ser `InProgress`.

> [!NOTE]
> 
> Atualizar um **accessReviewInstance** atualizará apenas essa instância. O **accessReviewScheduleDefinition** pai e quaisquer objetos **accessReviewInstance** futuros não mudarão. Para fazer atualizações que se aplicam a todas as instâncias futuras, atualize o objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) pai.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo                            | AccessReview.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|fallbackReviewers|[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Essa coleção de escopos de revisores é usada para definir a lista de revisores de fallback. Esses revisores de fallback serão notificados para tomar medidas se nenhum usuário for encontrado na lista de revisores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe. Opcional. Atualizável.|
|Revisores|[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Essa coleção de escopos de revisão de acesso é usada para definir quem são os revisores. Para obter exemplos de opções para atribuir revisores, consulte Atribuir revisores à sua definição de revisão de acesso [usando o Microsoft API do Graph](/graph/accessreviews-scope-concept). Opcional. Atualizável.|
|scope|[accessReviewScope](../resources/accessreviewscope.md)|Criado com base **no escopo** **e instanceEnumerationScope** no [nível accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) . Define o escopo dos usuários revisados em um grupo. Somente leitura. Obrigatório, mas não atualizado.|


## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `200 OK` de resposta e um objeto [accessReviewInstance](../resources/accessreviewinstance.md) atualizado no corpo da resposta.

A tentativa de remover **fallbackReviewers existente** retorna um código `409 Conflict` de resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessreviewinstance"
}
-->
```msgraph-interactive
PATCH https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5dcfcc88-da88-4252-8629-a0807b4b076d/instances/720b8ee0-cee4-42ac-b164-894c48703acc
Content-Type: application/json

{
    "scope": {
        "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
        "principalScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/users",
                "queryType": "MicrosoftGraph"
            },
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups",
                "queryType": "MicrosoftGraph"
            }
        ],
        "resourceScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/beta/roleManagement/directory/roleDefinitions/9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
                "queryType": "MicrosoftGraph"
            }
        ]
    },
    "reviewers": [
        {
            "query": "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
            "queryType": "MicrosoftGraph"
        }
    ],
    "fallbackReviewers": [
        {
            "query": "/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e",
            "queryType": "MicrosoftGraph"
        },
        {
            "query": "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
            "queryType": "MicrosoftGraph"
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-accessreviewinstance-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('5dcfcc88-da88-4252-8629-a0807b4b076d')/instances/$entity",
    "id": "720b8ee0-cee4-42ac-b164-894c48703acc",
    "startDateTime": "2021-12-14T11:15:43.207Z",
    "endDateTime": "2021-12-15T11:15:43.207Z",
    "status": "InProgress",
    "scope": {
        "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
        "principalScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/users",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        ],
        "resourceScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/beta/roleManagement/directory/roleDefinitions/9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        ]
    },
    "reviewers": [
        {
            "query": "/v1.0/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "fallbackReviewers": [
        {
            "query": "/v1.0/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        },
        {
            "query": "/v1.0/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ]
}
```

