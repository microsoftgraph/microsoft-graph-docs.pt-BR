---
author: swapnil1993
title: Excluir contentType
description: Exclua um tipo de conteúdo de uma SharePoint ou de um site.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 7fe42ef5c030839bf9db20a0c5b28eae642b8e10
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696471"
---
# <a name="delete-contenttype"></a>Excluir contentType
Namespace: microsoft.graph



Remover um [tipo de conteúdo][contentType] de uma [lista][] ou de um [site][].


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.Manage.All, Sites.FullControl.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sites.Manage.All, Sites.FullControl.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/contentTypes/{contentType-id}
DELETE /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|


## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação com esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "delete_contenttype"
}
-->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/{contentType-id}
```

### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
