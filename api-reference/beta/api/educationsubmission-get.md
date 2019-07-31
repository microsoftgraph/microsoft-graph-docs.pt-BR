---
title: Obter educationSubmission
description: 'Recupere um determinado envio. Um objeto de envio representa o trabalho de um aluno para uma atribuição. Os recursos associados ao envio representam esse trabalho. Somente o aluno ao qual o envio é atribuído pode ver e modificar o envio. Um professor tem acesso total a todos os envios. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d33fea58845fb9c9034d4fef100e3393bcdd4188
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955122"
---
# <a name="get-educationsubmission"></a>Obter educationSubmission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere um determinado envio. Um objeto de envio representa o trabalho de um aluno para uma atribuição. Os recursos associados ao envio representam esse trabalho. Somente o aluno ao qual o envio é atribuído pode ver e modificar o envio. Um professor tem acesso total a todos os envios. 

A classificação e os comentários de um professor também fazem parte desse objeto. Somente os professores podem adicionar ou alterar notas e comentários. Os alunos não verão a nota ou os comentários até que a atribuição tenha sido liberada. As permissões básicas não incluem a classificação e o feedback, mas incluem tudo o mais.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite |
|Delegado (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | Sem suporte. | 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.
## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationSubmission](../resources/educationsubmission.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmission"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
##### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 712

{
    "feedback": {
      text: {
        "content": "Good work!",
        "contentType": "Text"
      },
      feedbackDateTime: "2014-01-01T00:00:00Z",
      feedbackBy: {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012"
        }
      },
      "@odata.type": "microsoft.graph.educationFeedback"
      },
      "grade": {
         "gradedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
        "gradedDateTime": "2014-01-01T00:00:00Z"
      },
      "id": "33223",
      "recipient": {
        "userId": "13015"
      },
      "releasedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "releasedDateTime": "2014-01-01T00:00:00Z",
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
      "submittedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "submittedDateTime": "2014-01-01T00:00:00Z"
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
