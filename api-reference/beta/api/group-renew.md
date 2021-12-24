---
title: 'group: renew'
description: Renova a expiração de um grupo. Quando um grupo é renovado, a expiração do grupo é estendida pelo número de dias definido na política.
ms.localizationpriority: medium
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d1b83cfa1072e8fe2eb7ac9b27beb8342815edcb
ms.sourcegitcommit: 9759b647acfbed99d5675a6f512aaa33932a723f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/23/2021
ms.locfileid: "61604368"
---
# <a name="group-renew"></a>group: renew

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Renova a expiração de um grupo. Quando um grupo é renovado, a expiração do grupo é estendida pelo número de dias definido na política.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).
 

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.ReadWrite.All ou Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte |
|Aplicativo | Group.ReadWrite.All ou Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório. |


## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/renew
```


### <a name="response"></a>Resposta
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```