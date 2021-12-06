---
title: 'educationAssignment: publish'
description: Altere o estado de um educationAssignment de seu status de rascunho original para o status publicado.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: bc5c105157e671e25f36e75219a6e13af8a9f631
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61000352"
---
# <a name="educationassignment-publish"></a>educationAssignment: publish

Namespace: microsoft.graph

Publicar uma atribuição de educação.

Altere o estado de [um educationAssignment](../resources/educationassignment.md) de seu status original `draft` para o `published` status. 

Você pode alterar o estado de `draft` para `scheduled` se a **atribuição** estiver agendada para uma data futura. 

Somente um professor da classe pode fazer essa chamada. Quando uma atribuição estiver no status de rascunho, os alunos não verão a atribuição, nem haverá objetos de envio. Chamar essa API [cria objetos educationSubmission](../resources/educationsubmission.md) e exibe a atribuição na lista de cada aluno.

O estado da atribuição volta para se houver alguma falha `draft` de back-end durante o processo de publicação.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite  |
|Delegado (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | Sem suporte. | 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Não fornece um corpo de solicitação para este método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 Ok` [objeto educationAssignment](../resources/educationassignment.md) no corpo da resposta.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","1b6df208-ea5a-475c-8dd2-b92f693c928a"],
  "name": "educationassignment_publish_2"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1b6df208-ea5a-475c-8dd2-b92f693c928a/publish
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/educationassignment-publish-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
Veja a seguir um exemplo de uma resposta. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->

```http
HTTP/1.1 200 Ok

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#educationAssignment",
    "@odata.type": "#microsoft.graph.educationAssignment",
    "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
    "displayName": "Reading Test 09.03 3",
    "closeDateTime": null,
    "dueDateTime": "2021-09-05T06:59:00Z",
    "assignDateTime": null,
    "assignedDateTime": null,
    "allowLateSubmissions": true,
    "resourcesFolderUrl": null,
    "createdDateTime": "2021-09-03T23:26:35.4182773Z",
    "lastModifiedDateTime": "2021-09-03T23:28:05.0704312Z",
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "published",
    "notificationChannelUrl": null,
    "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%221b6df208-ea5a-475c-8dd2-b92f693c928a%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
    "addedStudentAction": "none",
    "id": "1b6df208-ea5a-475c-8dd2-b92f693c928a",
    "grading": null,
    "instructions": {
        "content": "",
        "contentType": "text"
    },
    "assignTo": {
        "@odata.type": "#microsoft.graph.educationAssignmentClassRecipient"
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
    }
}
```

## <a name="see-also"></a>Confira também

* [Estados, transições e limitações para atribuições e envios](/graph/assignments-submissions-states-transition)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


