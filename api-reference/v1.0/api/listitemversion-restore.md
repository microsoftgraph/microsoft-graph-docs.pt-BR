---
title: Restaura uma versão anterior de um ListItem
description: Restaura uma versão anterior de um ListItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3ba63f56838d07a0031baf613dec8e0847aaf2e6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963392"
---
# <a name="restore-a-previous-version-of-a-listitem"></a>Restaura uma versão anterior de um ListItem

Restaura uma versão anterior de um ListItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|            Tipo de permissão             |         Permissões (da com menos para a com mais privilégios)          |
| :------------------------------------- | :----------------------------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |
| Delegada (conta pessoal da Microsoft) | n/d                                                          |
| Aplicativo                            | Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a>Corpo da solicitação

Nenhum corpo de solicitação é obrigatório.

## <a name="example"></a>Exemplo

Este exemplo restaura uma versão de um listItem identificado por `{item-id}` e `{version-id}`.

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a>Resposta

Se tiver êxito, a chamada API retorna um código `204 No Content`.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
