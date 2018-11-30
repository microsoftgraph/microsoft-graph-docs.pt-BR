---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: Excluir uma página de um site do SharePoint
ms.openlocfilehash: c537acec2e205ffd556a35789f75be95e2b94017
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035060"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a>Excluir página na lista de páginas de site de um site

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Remove um [sitePage][] de páginas do site [lista][] em um [site][].

[sitePage]: ../resources/sitepage.md
[lista]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

>**Observação:** Para excluir um item, o usuário deve ter concedido ao acesso de gravação do aplicativo até o item a ser excluído.

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Nome       | Valor | Descrição
|:-----------|:------|:--------------------------------------------------------
| _if-match_ | etag  | Se este cabeçalho de solicitação estiver incluso e a eTag fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` será exibida e o item não será excluído.

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação com esse método.
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a>Resposta

Se tiver êxito, essa chamada retornará um `204 No Content` resposta para indicar que o recurso foi excluído e não houve nothing para retornar.

## <a name="example"></a>Exemplo

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a>Solicitação

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a>Resposta

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete"
} -->
