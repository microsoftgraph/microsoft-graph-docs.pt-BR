---
title: Remover acceptedSender
description: 'Remova um usuário ou grupo da lista acceptedSenders. '
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 8f728e3075d64de3b1241079c57512b8699e2262
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819135"
---
# <a name="remove-acceptedsender"></a>Remover acceptedSender

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Remova um usuário ou grupo da lista acceptedSenders. 

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)  |
|:---------------------------------------|:-------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | Group.ReadWrite.All    |
| Delegado (conta pessoal da Microsoft) | Sem suporte.|
| Aplicativo                            | Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id=<id>
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho         | Valor                      |
|:---------------|:---------------------------|
| Autorização  | {token} de portador. Obrigatório.  

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
#### <a name="request"></a>Solicitação
Estes são alguns exemplos de solicitação.

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}

DELETE https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
