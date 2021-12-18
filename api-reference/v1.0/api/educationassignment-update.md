---
title: Atualizar educationassignment
description: Atualizar um objeto educationAssigment.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 786d364847297edea5538251c5701502c3ced7f2
ms.sourcegitcommit: 15dd0e98e69f872ed5a709600608b244759b0967
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2021
ms.locfileid: "61567304"
---
# <a name="update-educationassignment"></a>Atualizar educationassignment

Namespace: microsoft.graph

Atualize [um objeto educationAssignment.](../resources/educationassignment.md) 

Somente os professores podem executar essa ação. 

Como alternativa, solicite alterar o status de uma **atribuição com** a [ação de](../api/educationassignment-publish.md) publicação. Não use uma operação PATCH para essa finalidade.

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
PATCH /education/classes/{class-id}/assignments/{assignment-id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece apenas os valores dos campos que você deseja atualizar. 

Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|addedStudentAction|Cadeia de caracteres| Descreve se a atribuição deve ser distribuída aos alunos que são adicionados após a data de publicação da atribuição.|
|addToCalendarAction|educationAddToCalendarOptions|Campo opcional para controlar o comportamento **de atribuição** para adicionar atribuições aos **calendários** dos alunos e professores quando a **atribuição** for publicada. Os valores possíveis são: `none`, `studentsAndPublisher`, `studentsAndTeamOwners`, `unknownFutureValue`, `studentsOnly`. Observe que você deve usar o header de solicitação para obter os seguintes valores nesta `Prefer: include - unknown -enum-members` [enum evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `studentsOnly` . Opcional.|
|allowLateSubmissions|Booliano| Se os alunos podem enviar envio após a data de vencimento.|
|allowStudentsToAddResourcesToSubmission|Booliano| Se um aluno pode adicionar recursos a um envio ou não. Além disso, indica se todos os recursos no envio correspondem à lista de recursos de atribuição. |
|assignDateTime|DateTimeOffset| Indica a data para publicar a atribuição aos alunos. |
|assignTo|educationAssignmentRecipient| Alunos que receberão a atribuição.|
|closeDateTime|DateTimeOffset| Data em que a atribuição será fechada para envios. Este é um campo opcional que pode ser nulo se a atribuição não permitirLateSubmissions ou closeDateTime for igual ao dueDateTime, mas se especificado, ele deve ser maior ou igual ao dueDateTime.|
|displayName|Cadeia de caracteres| Nome da atribuição. |
|dueDateTime|DateTimeOffset| A atribuição de data é devido. |
|grading|educationAssignmentGradeType| Como a atribuição será gradeada.|
|instructions|itemBody| Instruções a serem fornecidas aos alunos juntamente com a atribuição. |
|notificationChannelUrl|Cadeia de caracteres| O canal para comunicar notificações relacionadas à atribuição. Para alterar a URL, de definir `assignTo` o valor [como educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md). A URL do canal não pode ser mudada após a publicação da atribuição.|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [educationAssignment](../resources/educationassignment.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","4679bc1b-90c5-45af-ae1a-d5357672ed39"],
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/4679bc1b-90c5-45af-ae1a-d5357672ed39
Content-type: application/json

{
    "displayName": "Reading and review test 09.03 #5",
    "instructions": {
        "contentType": "text",
        "content": "Read chapter 5 and write your review"
    },
    "dueDateTime": "2021-09-10T00:00:00Z",
    "addedStudentAction": "none"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-educationassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments/$entity",
    "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
    "displayName": "Reading and review test 09.03 #5",
    "closeDateTime": null,
    "dueDateTime": "2021-09-10T00:00:00Z",
    "assignDateTime": null,
    "assignedDateTime": null,
    "allowLateSubmissions": true,
    "resourcesFolderUrl": null,
    "createdDateTime": "2021-09-03T23:57:14.6088791Z",
    "lastModifiedDateTime": "2021-09-04T15:01:35.3361649Z",
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "draft",
    "notificationChannelUrl": null,
    "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%224679bc1b-90c5-45af-ae1a-d5357672ed39%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
    "addedStudentAction": "none",
    "id": "4679bc1b-90c5-45af-ae1a-d5357672ed39",
    "instructions": {
        "content": "Read chapter 5 and write your review",
        "contentType": "text"
    },
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 50
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
            "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
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
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


