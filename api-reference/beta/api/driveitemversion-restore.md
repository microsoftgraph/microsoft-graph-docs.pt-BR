---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Restaurar uma versão anterior
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9f8492b3a6e4b01b61288b235cc0dfa19ffd78d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946074"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a>Restaurar uma versão anterior de um DriveItem

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Restaura uma versão anterior de um DriveItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do arquivo.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.ReadWrite, Files.ReadWrite.All    |
|Aplicativo | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a>Corpo da solicitação

Nenhum corpo de solicitação é obrigatório.

## <a name="example"></a>Exemplo

Este exemplo restaura uma versão de um arquivo identificado por `{item-id}` e `{version-id}`.

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a>Resposta

Se tiver êxito, a chamada API retorna um código `204 No content`.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
