---
title: Obter educationCategory
description: Recupere um objeto category.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fed72875c029c2080af7f8e2133a2f2a6d94b3ba
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061781"
---
# <a name="get-educationcategory"></a>Obter educationCategory

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere um [objeto educationCategory.](../resources/educationcategory.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                                                                         |
| Application*                           | EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite |

*As permissões de aplicativo estão disponíveis apenas para clientes de visualização privada.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho        | Valor                     |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [educationCategory](../resources/educationcategory.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories/{id}
```

##### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 85

{
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get category",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->