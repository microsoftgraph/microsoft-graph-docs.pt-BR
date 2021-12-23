---
title: Obter educationSubmission
description: 'Recupere um envio específico. Um objeto de envio representa o trabalho de um aluno para uma atribuição. Os recursos associados ao envio representam esse trabalho. Somente o aluno ao que o envio é atribuído pode ver e modificar o envio. Um professor ou aplicativo com permissões de aplicativo tem acesso total a todos os envios. '
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fe05dce0628d8829184fd6e60b4bcff7bd23b207
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525981"
---
# <a name="get-educationsubmission"></a>Obter educationSubmission

Namespace: microsoft.graph

Recuperar um envio [específico](../resources/educationsubmission.md).

Um **objeto de** envio representa o trabalho de um aluno para uma [atribuição](../resources/educationassignment.md). Os recursos associados ao **envio representam** esse trabalho.

Somente o **aluno assignedTo** pode ver e modificar o **envio**. Um professor ou aplicativo com permissões de aplicativo tem acesso total a todos os **envios.**

As notas e os comentários de um professor fazem parte do [educationOutcome](../resources/educationoutcome.md) associado a esse objeto. Somente professores ou aplicativos com permissões de aplicativo podem adicionar ou alterar notas e comentários. Os alunos não verão a nota ou os comentários até que **a atribuição** seja lançada.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite |
|Delegada (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | EduAssignments.ReadBasic.All, EduAssignments.ReadWriteBasic.All, EduAssignments.Read.All, EduAssignments.ReadWrite.All | 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{class-id}/assignments/{assignment-id}/submissions/{submission-id}
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

Veja a seguir as opções disponíveis para este método: , , e , que `$expand` inclui todas as opções `outcomes` `resources` `submittedResources` `*` anteriores. Para obter detalhes, consulte a seção exemplos.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Não fornece um corpo de solicitação para este método.
## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationSubmission](../resources/educationsubmission.md) no corpo da resposta.

## <a name="examples"></a>Exemplos
### <a name="example-1-get-submission"></a>Exemplo 1: Obter envio
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationsubmission"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/59069eb2-2a09-4d90-bb19-2089cc69d613/assignments/80da1069-a635-4913-813f-d775a5470a8f/submissions/869369de-3e5a-89eb-6f2d-83cd88f860b5
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsubmission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsubmission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsubmission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsubmission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-educationsubmission-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observações:** O objeto de resposta mostrado aqui pode ser reduzido para a capacidade de leitura. 
>
>Se [setUpResourcesFolder](educationsubmission-setupResourcesFolder.md) ainda não tiver sido chamado neste [recurso educationSubmission,](../resources/educationsubmission.md) a propriedade **resourcesFolderUrl** será `null` .

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 712

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('59069eb2-2a09-4d90-bb19-2089cc69d613')/assignments('80da1069-a635-4913-813f-d775a5470a8f')/submissions/$entity",
    "status": "returned",
    "submittedDateTime": "2021-11-10T00:57:17.0495233Z",
    "unsubmittedDateTime": null,
    "returnedDateTime": "2021-11-10T01:03:25.7812455Z",
    "resourcesFolderUrl": null,
    "id": "869369de-3e5a-89eb-6f2d-83cd88f860b5",
    "recipient": {
        "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
        "userId": "723e2402-f503-4825-a4d5-5143fbe6f53d"
    },
    "submittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "723e2402-f503-4825-a4d5-5143fbe6f53d",
            "displayName": null
        }
    },
    "unsubmittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": null,
            "displayName": null
        }
    },
    "returnedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "afc58f1f-7c9e-4770-a448-e53ba43463a5",
            "displayName": null
        }
    }
}
```

### <a name="example-2-get-submission-with-expand-options"></a>Exemplo 2: obter envio com $expand opções
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_submission_expand"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/59069eb2-2a09-4d90-bb19-2089cc69d613/assignments/80da1069-a635-4913-813f-d775a5470a8f/submissions/869369de-3e5a-89eb-6f2d-83cd88f860b5?$expand=*
```

#### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 4492

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('59069eb2-2a09-4d90-bb19-2089cc69d613')/assignments('80da1069-a635-4913-813f-d775a5470a8f')/submissions(outcomes(),resources(),submittedResources())/$entity",
    "status": "returned",
    "submittedDateTime": "2021-11-10T00:57:17.0495233Z",
    "unsubmittedDateTime": null,
    "returnedDateTime": "2021-11-10T01:03:25.7812455Z",
    "resourcesFolderUrl": null,
    "id": "869369de-3e5a-89eb-6f2d-83cd88f860b5",
    "recipient": {
        "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
        "userId": "723e2402-f503-4825-a4d5-5143fbe6f53d"
    },
    "submittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "723e2402-f503-4825-a4d5-5143fbe6f53d",
            "displayName": null
        }
    },
    "unsubmittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": null,
            "displayName": null
        }
    },
    "returnedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "afc58f1f-7c9e-4770-a448-e53ba43463a5",
            "displayName": null
        }
    },
    "outcomes@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('59069eb2-2a09-4d90-bb19-2089cc69d613')/assignments('80da1069-a635-4913-813f-d775a5470a8f')/submissions('869369de-3e5a-89eb-6f2d-83cd88f860b5')/outcomes",
    "outcomes": [
        {
            "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
            "lastModifiedDateTime": null,
            "id": "ca05367a-b292-42d5-aff7-5d279feeace8",
            "lastModifiedBy": null,
            "feedback": null,
            "publishedFeedback": null
        },
        {
            "@odata.type": "#microsoft.graph.educationPointsOutcome",
            "lastModifiedDateTime": null,
            "id": "ea1351f6-ba33-4940-b2cb-6a7254af2dc8",
            "lastModifiedBy": null,
            "points": null,
            "publishedPoints": null
        },
        {
            "@odata.type": "#microsoft.graph.educationRubricOutcome",
            "lastModifiedDateTime": "2021-11-10T01:03:25.7712076Z",
            "id": "65a46d78-1a2b-4a7e-bcf8-78a22ac2611b",
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            },
            "rubricQualityFeedback": [
                {
                    "qualityId": "a660004a-608d-4cd2-a6dc-4f43812444ee",
                    "feedback": null
                },
                {
                    "qualityId": "2c5ae75d-d347-426b-be2c-cfc81a6f0b32",
                    "feedback": null
                },
                {
                    "qualityId": "32fdea06-5cbb-4881-9093-96e59f59b8b8",
                    "feedback": null
                },
                {
                    "qualityId": "66137bd8-b9c2-40e1-a360-40b7ee75eaef",
                    "feedback": null
                }
            ],
            "rubricQualitySelectedLevels": [
                {
                    "qualityId": "a660004a-608d-4cd2-a6dc-4f43812444ee",
                    "columnId": null
                },
                {
                    "qualityId": "2c5ae75d-d347-426b-be2c-cfc81a6f0b32",
                    "columnId": null
                },
                {
                    "qualityId": "32fdea06-5cbb-4881-9093-96e59f59b8b8",
                    "columnId": null
                },
                {
                    "qualityId": "66137bd8-b9c2-40e1-a360-40b7ee75eaef",
                    "columnId": null
                }
            ],
            "publishedRubricQualityFeedback": [
                {
                    "qualityId": "a660004a-608d-4cd2-a6dc-4f43812444ee",
                    "feedback": null
                },
                {
                    "qualityId": "2c5ae75d-d347-426b-be2c-cfc81a6f0b32",
                    "feedback": null
                },
                {
                    "qualityId": "32fdea06-5cbb-4881-9093-96e59f59b8b8",
                    "feedback": null
                },
                {
                    "qualityId": "66137bd8-b9c2-40e1-a360-40b7ee75eaef",
                    "feedback": null
                }
            ],
            "publishedRubricQualitySelectedLevels": [
                {
                    "qualityId": "a660004a-608d-4cd2-a6dc-4f43812444ee",
                    "columnId": null
                },
                {
                    "qualityId": "2c5ae75d-d347-426b-be2c-cfc81a6f0b32",
                    "columnId": null
                },
                {
                    "qualityId": "32fdea06-5cbb-4881-9093-96e59f59b8b8",
                    "columnId": null
                },
                {
                    "qualityId": "66137bd8-b9c2-40e1-a360-40b7ee75eaef",
                    "columnId": null
                }
            ]
        }
    ],
    "resources@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('59069eb2-2a09-4d90-bb19-2089cc69d613')/assignments('80da1069-a635-4913-813f-d775a5470a8f')/submissions('869369de-3e5a-89eb-6f2d-83cd88f860b5')/resources",
    "resources": [],
    "submittedResources@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('59069eb2-2a09-4d90-bb19-2089cc69d613')/assignments('80da1069-a635-4913-813f-d775a5470a8f')/submissions('869369de-3e5a-89eb-6f2d-83cd88f860b5')/submittedResources",
    "submittedResources": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
