---
title: Criar educationCategory
description: Cria uma nova categoria.
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 45e7bfd5affd70574ade93daba94caedc75735a6
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223744"
---
# <a name="create-educationcategory"></a>Criar educationCategory

Namespace: microsoft.graph

Cria uma nova [educationCategory](../resources/educationcategory.md) em uma [educationClass](../resources/educationclass.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) |  EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite  |
|Delegado (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | Sem suporte. | 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignmentCategories/$entity
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um [objeto educationCategory.](../resources/educationcategory.md)


## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto educationCategory](../resources/educationcategory.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["60eaa744-aa87-4276-b985-1633683119f8"],
  "name": "create_educationcategory_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/60eaa744-aa87-4276-b985-1633683119f8/assignmentCategories/$entity
Content-type: application/json

{ 
  "displayName": "Quizzes"
}
```
# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-educationcategory-from-educationclass-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('60eaa744-aa87-4276-b985-1633683119f8')/assignmentCategories/$entity",
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


