---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Carregar arquivos pequenos
ms.openlocfilehash: 44d3d3033014067af968720d24e87ec5047416ae
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a>Carregar ou substituir o conteúdo de um DriveItem

A API de upload simples permite que você forneça o conteúdo de um novo arquivo ou atualize o conteúdo de um arquivo existente em uma única chamada à API. Este método só dá suporte a arquivos com até 4 MB de tamanho.

Para carregar arquivos grandes, confira [Carregar arquivos grandes com uma sessão de carregamento](driveitem_createuploadsession.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.ReadWrite, Files.ReadWrite.All    |
|Aplicativo | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request-to-replace-an-existing-item"></a>Solicitação HTTP (para substituir um item existente)

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a>Solicitação HTTP (para carregar um novo arquivo)

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a>Corpo da solicitação

O conteúdo do corpo da solicitação deve ser o fluxo binário do arquivo a ser carregado.

## <a name="response"></a>Resposta

Se for bem-sucedido, este método retornará um objeto [driveItem](../resources/driveitem.md) no corpo da resposta para o arquivo recém-criado ou atualizado.

## <a name="example-upload-a-new-file"></a>Exemplo (carregar um novo arquivo)

Este exemplo carrega a cadeia de caracteres "O conteúdo do arquivo fica aqui". para um arquivo na unidade do usuário conectado em FolderA chamado FileB.txt.

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a>Resposta

Se for bem-sucedido, esse método retornará um recurso [driveItem][item-resource] no corpo da resposta para o arquivo recém-criado.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="example-updating-an-existing-file"></a>Exemplo (atualizando um arquivo existente)

Este exemplo substitui o conteúdo de um arquivo com uma ID conhecida.

<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a>Resposta

Se for bem-sucedido, esse método retornará um recurso [driveItem][item-resource] no corpo da resposta para o arquivo recém-criado.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="error-responses"></a>Respostas de erro

Confira mais detalhes sobre como os erros são retornados em [Respostas de erro][error-response].

[error-response]: ../../../concepts/errors.md
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation"
} -->
