---
title: Remover um membro
description: Use essa API para remover um membro (usuário, grupo ou dispositivo) de uma unidade administrativa.
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 199e0ba76a61b8279dcd79acb59ef14d9001a35d
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898165"
---
# <a name="remove-a-member"></a>Remover um membro

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use essa API para remover um membro (usuário, grupo ou dispositivo) de uma unidade administrativa.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | AdministrativeUnit.ReadWrite.All   |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | AdministrativeUnit.ReadWrite.All |

Para remover um membro de uma unidade administrativa, a entidade de chamada deve receber uma das seguintes funções do [Azure AD](/azure/active-directory/roles/permissions-reference):

* Administrador de Função Com Privilégios
* Administrador Global

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
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

```msgraph-interactive
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
 
```http
HTTP/1.1 204 No Content
```


