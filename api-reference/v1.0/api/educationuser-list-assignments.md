---
title: Listar atribuições de um usuário
description: Retorna uma lista de atribuições atribuídas a um usuário para todas as classes.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4e3a9cfac827c7bc6e2b6d7c8afe9d838b25d291
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516135"
---
# <a name="list-assignments-of-a-user"></a>Listar atribuições de um usuário

Namespace: microsoft.graph

Retorna uma lista [de educationAssignment atribuído](../resources/educationassignment.md) a um [educationUser](../resources/educationuser.md) para todas as [classes](../resources/educationclass.md). 

Esse método permite que um chamador encontre todas as atribuições **pertencentes** a um aluno ou professor em uma única chamada, em vez de precisar solicitar **atribuições** de cada **classe**. A **lista** de atribuições contém o que é necessário para obter as informações detalhadas para a atribuição **de dentro** do namespace **de** classe. Use os métodos definidos para a **atribuição** para todas as outras operações.

> **Observação:** As `instructions`propriedades , `assignTo``assignedDateTime`e `resourcesFolderUrl` sempre `webUrl` serão exibidas nulas.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                                                                         |
| Aplicativo                            | EduAssignments.ReadBasic.All, EduAssignments.ReadWriteBasic.All, EduAssignments.Read.All, EduAssignments.ReadWrite.All |

Chamar o ponto de extremidade `/me` exige um usuário conectado e, portanto, uma permissão delegada. Não há suporte para permissões do aplicativo ao usar o ponto de extremidade `/me`.

O `/users/{user-id}` ponto de extremidade funciona com permissões delegadas e de aplicativo.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments
GET /education/users/{user-id}/assignments
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte aos `$submissions` Parâmetros `$categories` de [Consulta E OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor                     |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de [objetos educationAssignment](../resources/educationassignment.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-the-assignments-of-the-logged-in-user"></a>Exemplo 1: Obter as atribuições do usuário conectado

#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_me_assignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/me/assignments
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-me-assignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-me-assignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-me-assignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-me-assignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-me-assignments-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-me-assignments-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

#### <a name="response"></a>Resposta

Este é um exemplo de resposta. 

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/me/assignments",
    "value": [
        {
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Expand options 3.1",
            "closeDateTime": "2021-11-19T07:59:00Z",
            "dueDateTime": "2021-11-19T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": null,
            "allowLateSubmissions": false,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:56:21.1575202Z",
            "lastModifiedDateTime": "2021-11-17T16:00:30.0523446Z",
            "allowStudentsToAddResourcesToSubmission": false,
            "status": "published",
            "notificationChannelUrl": null,
            "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%223b870c07-21fe-47fb-8562-cdd6f2c281d6%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "id": "3b870c07-21fe-47fb-8562-cdd6f2c281d6",
            "instructions": null,
            "grading": null,
            "assignTo": null,
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            }
        },
        {
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Expand options 4",
            "closeDateTime": null,
            "dueDateTime": "2021-11-12T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": null,
            "allowLateSubmissions": true,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:58:41.5064997Z",
            "lastModifiedDateTime": "2021-11-10T23:58:41.5304842Z",
            "allowStudentsToAddResourcesToSubmission": false,
            "status": "draft",
            "notificationChannelUrl": null,
            "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%2234ab8c17-eaae-4996-9c04-53696934e6ff%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "id": "34ab8c17-eaae-4996-9c04-53696934e6ff",
            "instructions": null,
            "grading": null,
            "assignTo": null,
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            }
        }
    ]
}
```

### <a name="example-2-get-assignments-of-a-user"></a>Exemplo 2: Obter atribuições de um usuário

#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_assignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/users/f3a5344e-dbde-48b0-be24-b5b62a243836/assignments
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-assignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-assignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-assignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-assignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-user-assignments-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-user-assignments-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a>Resposta

Se o usuário tentar consultar uma ID de usuário diferente da sua, este método retornará um `403 Forbidden` código de resposta.

Este é um exemplo de resposta. 

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/users('f3a5344e-dbde-48b0-be24-b5b62a243836')/assignments",
    "value": [
        {
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Expand options 3.1",
            "closeDateTime": "2021-11-19T07:59:00Z",
            "dueDateTime": "2021-11-19T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": null,
            "allowLateSubmissions": false,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:56:21.1575202Z",
            "lastModifiedDateTime": "2021-11-17T16:00:30.0523446Z",
            "allowStudentsToAddResourcesToSubmission": false,
            "status": "published",
            "notificationChannelUrl": null,
            "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%223b870c07-21fe-47fb-8562-cdd6f2c281d6%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "id": "3b870c07-21fe-47fb-8562-cdd6f2c281d6",
            "instructions": null,
            "grading": null,
            "assignTo": null,
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            }
        },
        {
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Expand options 4",
            "closeDateTime": null,
            "dueDateTime": "2021-11-12T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": null,
            "allowLateSubmissions": true,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:58:41.5064997Z",
            "lastModifiedDateTime": "2021-11-10T23:58:41.5304842Z",
            "allowStudentsToAddResourcesToSubmission": false,
            "status": "draft",
            "notificationChannelUrl": null,
            "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%2234ab8c17-eaae-4996-9c04-53696934e6ff%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "id": "34ab8c17-eaae-4996-9c04-53696934e6ff",
            "instructions": null,
            "grading": null,
            "assignTo": null,
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            }
        }
    ]
}
```

### <a name="example-3-get-user-assignments-with-expand-submissions"></a>Exemplo 3: Obter atribuições de usuário com envios de expansão

#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_assignments_expand_submissions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/users/80cefd93-8d88-40e2-b5d3-67898383e226/assignments?expand=submissions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-assignments-expand-submissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-assignments-expand-submissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-assignments-expand-submissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-assignments-expand-submissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-user-assignments-expand-submissions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-user-assignments-expand-submissions-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta. 

> **Observação:** Ele expandirá os envios se o usuário tiver uma função de aluno e será nulo para a função de professor.


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/users('80cefd93-8d88-40e2-b5d3-67898383e226')/assignments(submissions())",
    "value": [
        {
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Reading test 09.03 #4",
            "closeDateTime": null,
            "dueDateTime": "2021-09-07T00:00:00Z",
            "assignDateTime": null,
            "assignedDateTime": null,
            "allowLateSubmissions": true,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-09-13T19:18:35.2587894Z",
            "lastModifiedDateTime": "2021-09-13T19:19:56.6381405Z",
            "allowStudentsToAddResourcesToSubmission": false,
            "status": "assigned",
            "notificationChannelUrl": null,
            "webUrl": null,
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "id": "1618dfb0-3ff2-4edf-8d5c-b8f81df00e80",
            "instructions": null,
            "assignTo": null,
            "grading": {
                "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints": 50
            },
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "AAAAAAAA-0123-4567-89AB-1B4BB48C3119",
                    "displayName": null
                }
            },
            "submissions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/users('80cefd93-8d88-40e2-b5d3-67898383e226')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/submissions",
            "submissions": [
                {
                    "status": "working",
                    "submittedDateTime": null,
                    "unsubmittedDateTime": null,
                    "returnedDateTime": null,
                    "reassignedDateTime": null,
                    "resourcesFolderUrl": null,
                    "id": "da443246-384d-673b-32db-bdba9d7f2b51",
                    "recipient": {
                        "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
                        "userId": "80cefd93-8d88-40e2-b5d3-67898383e226"
                    },
                    "submittedBy": {
                        "application": null,
                        "device": null,
                        "user": {
                            "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
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
                            "id": null,
                            "displayName": null
                        }
                    },
                    "reassignedBy": {
                        "application": null,
                        "device": null,
                        "user": {
                            "id": null,
                            "displayName": null
                        }
                    }
                }
            ]
        }
    ]
}        
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
