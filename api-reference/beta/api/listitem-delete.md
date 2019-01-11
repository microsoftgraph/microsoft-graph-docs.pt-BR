---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Excluir uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.openlocfilehash: 71be680ae2d29d083d06c9d18aa79675ebdd01dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849277"
---
# <a name="delete-an-item-from-a-list"></a>Excluir um item de uma lista.

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Remover um item de uma [list][].

[list]: ../resources/list.md

## <a name="permissions"></a>Permissões

Para excluir um item, o usuário deve ter concedido o acesso de gravação do aplicativo para o item a ser excluído.

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Nome       | Valor | Descrição
|:-----------|:------|:--------------------------------------------------------
| _if-match_ | etag  | Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será excluído.

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação com esse método.

## <a name="example"></a>Exemplo

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a>Resposta

Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete"
} -->
