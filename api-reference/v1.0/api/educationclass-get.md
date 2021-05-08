---
title: Obter educationClass
description: Recuperar uma classe do sistema
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 52f24e1f3c02b955874a78cdba447b697485f4a3
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232008"
---
# <a name="get-educationclass"></a>Obter educationClass

Namespace: microsoft.graph

Recupere uma aula do sistema. Uma aula é um grupo universal com uma propriedade especial que indica ao sistema que o grupo é uma aula. Os membros do grupo representam os alunos; os administradores de grupo representam os professores da classe. Se estiver usando o token delegado, o usuário verá apenas as aulas das quais são membros.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  EduRoster.ReadBasic  |
|Delegado (conta pessoal da Microsoft) |  Sem suporte  |
|Aplicativo | EduRoster.Read.All, EduRoster.ReadWrite.All | 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
É possível usar a opção de consulta `$select` para obter propriedades específicas do grupo, inclusive aquelas que não são retornadas por padrão.

Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.
## <a name="response"></a>Resposta
Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}
-->

```http
GET /education/classes/{educationClassId}
```

### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationClass",
    "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
    "displayName": "String",
    "mailNickname": "String",
    "description": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "classCode": "String",
    "externalName": "String",
    "externalId": "String",
    "externalSource": "String",
    "externalSourceDetail": "String",
    "grade": "String",
    "term": {
      "@odata.type": "microsoft.graph.educationTerm"
    }
  }
}
```
