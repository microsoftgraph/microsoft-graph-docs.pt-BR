---
title: Criar thread de bate-papo
description: Crie um novo segmento de bate-papo no canal especificado, fornecendo as mensagens de raiz.
author: nkramer
ms.openlocfilehash: fcd1c08c05b29d2150f4c436eac7765f40900920
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325610"
---
# <a name="create-chat-thread"></a>Criar thread de bate-papo

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Crie um novo segmento de bate-papo no [canal](../resources/channel.md) especificado, fornecendo as mensagens de raiz.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

> Atualmente, somente [permissões delegadas](/graph/permissions-reference) têm suporte para esta operação.  Permissões de aplicativo dará suporte a versões futuras. 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/chatThreads
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um objeto [chatThread](../resources/chatthread.md) que contém a propriedade rootMessage.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` código de resposta com o corpo de uma resposta vazia.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "create_chatthread_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/chatThreads
Content-type: application/json

{
  "rootMessage": {
      "body": {
        "contentType": 1,
        "content": "<h1>Hello world</h1>"
      }
  }
}
```

> Atualmente, o contentType deve ser especificado como um inteiro, em vez de uma cadeia de caracteres: 0 para "text" ou 1 para "html".  Versões futuras do API corrigirá.

##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
