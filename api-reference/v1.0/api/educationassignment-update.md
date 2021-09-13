---
title: Atualizar educationassignment
description: Atualizar um objeto educationAssigment.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f754a8e4e79bd0043199924acbaf28eec8261716
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020039"
---
# <a name="update-educationassignment"></a>Atualizar educationassignment

Namespace: microsoft.graph

Atualizar um objeto educationAssigment. 

Somente os professores podem executar essa ação. 

Como alternativa, solicite alterar o status de uma atribuição com a [ação de](../api/educationassignment-publish.md) publicação. Não use uma operação PATCH para essa finalidade.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) |  EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite  |
|Delegada (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | Sem suporte. | 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454
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
|allowLateSubmissions|Boolean| Se os alunos podem enviar envio após a data de vencimento.|
|allowStudentsToAddResourcesToSubmission|Booliano| Se um aluno pode adicionar recursos a um envio ou não. Além disso, indica se todos os recursos no envio correspondem à lista de recursos de atribuição. |
|assignDateTime|DateTimeOffset| Indica a data para publicar a atribuição aos alunos. |
|assignTo|educationAssignmentRecipient| Alunos que receberão a atribuição.|
|closeDateTime|DateTimeOffset| Data em que a atribuição será fechada para envios. Este é um campo opcional que pode ser nulo se a atribuição não permitirLateSubmissions ou closeDateTime for igual ao dueDateTime, mas se especificado, ele deve ser maior ou igual ao dueDateTime.|
|displayName|Cadeia de caracteres| Nome da atribuição. |
|dueDateTime|DateTimeOffset| A atribuição de data é devido. |
|grading|educationAssignmentGradeType| Como a atribuição será gradeada.|
|instructions|itemBody| Instruções a serem fornecidas aos alunos juntamente com a atribuição. |
|notificationChannelUrl|String| O canal para comunicar notificações relacionadas à atribuição. Para alterar a URL, de definir `assignTo` o valor [como educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md). A URL do canal não pode ser mudada após a publicação da atribuição.|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [educationAssignment](../resources/educationassignment.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8
Content-type: application/json
Content-length: 279

{
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z"
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
Content-length: 279

{
  "classId": "11021",
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "closeDateTime": "2014-02-11T00:00:00Z",
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!0sGAoOieeE6iSj1WXCV-nYYTuh2luKRDvUVGQBLOmvYpRzc5ARnCRorRht6P3MhU/items/01N74NOEZL7P3VK22SQFDKBZ3PHVPKDVAQ",
}
```

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


