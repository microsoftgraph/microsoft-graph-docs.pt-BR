---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Excluir um arquivo ou uma pasta
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 39c7706fab229e52c394c30c6daf478a1fefd581
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966864"
---
# <a name="delete-a-driveitem"></a>Excluir um DriveItem

Excluir um [DriveItem](../resources/driveitem.md) usando sua ID ou seu caminho. Observe que a exclusão de itens usando esse método moverá os itens para a Lixeira, ao invés de excluir permanentemente o item.

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
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Nome          | Tipo   | Descrição                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | String | Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído. |

## <a name="example"></a>Exemplo

Eis um exemplo de como chamar esta API.

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
DELETE /me/drive/items/{item-id}
```

## <a name="response"></a>Resposta

Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a>Respostas de erro

Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete"
} -->
