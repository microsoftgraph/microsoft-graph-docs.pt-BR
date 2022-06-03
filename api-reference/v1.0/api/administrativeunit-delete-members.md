---
title: Remover um membro
description: Use essa API para remover um membro (usuário, grupo ou dispositivo) de uma unidade administrativa.
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 449b154059bb869abf894c315516ac65f585af23
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884287"
---
# <a name="remove-a-member"></a>Remover um membro

Namespace: microsoft.graph

Use essa API para remover um membro (usuário, grupo ou dispositivo) de uma unidade administrativa.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | AdministrativeUnit.ReadWrite.All    |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Application | AdministrativeUnit.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo de solicitação. No exemplo abaixo, `{id1}` representa o identificador `{id2}` da unidade administrativa de destino e representa o identificador exclusivo para o usuário membro, grupo ou dispositivo a ser removido da unidade administrativa de destino. 

<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit_members"
} -->
```msgraph-interactive
DELETE https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id1}/members/{id2}/$ref
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
