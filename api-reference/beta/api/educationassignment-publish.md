---
title: 'educationAssignment: publicar'
description: Esta ação altera o estado de uma atribuição de seu status de rascunho original para o status publicado. Somente um professor na classe pode fazer essa chamada. Quando uma atribuição está no status de rascunho, alunos não verá a atribuição, nem haverá quaisquer objetos de envio. Quando você chamar essa API, são criados objetos de envio e a atribuição aparece na lista de student.
localization_priority: Normal
ms.openlocfilehash: 09261da506113f53c6b6b9ff98af69c7dba4c784
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854737"
---
# <a name="educationassignment-publish"></a>educationAssignment: publicar

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Esta ação altera o estado de uma atribuição de seu status de rascunho original para o status publicado. Somente um professor na classe pode fazer essa chamada. Quando uma atribuição está no status de rascunho, alunos não verá a atribuição, nem haverá quaisquer objetos de envio. Quando você chamar essa API, são criados objetos de envio e a atribuição aparece na lista de student.

## <a name="permissions"></a>Permissions
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
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.
##### <a name="request"></a>Solicitação
O exemplo a seguir é um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```

##### <a name="response"></a>Resposta
O exemplo a seguir é um exemplo de uma resposta. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
