---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: obter um arquivo ou uma pasta
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 094987d5898dcab02c704bdec8e6261811270341
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987157"
---
# <a name="get-a-driveitem-resource"></a>Obter um recurso DriveItem

Recupere os metadados de um [DriveItem](../resources/driveitem.md) em um [Drive](../resources/drive.md) por ID ou caminho do sistema de arquivos.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Aplicativo | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}
GET /drives/{drive-id}/root:/{item-path}
GET /groups/{group-id}/drive/items/{item-id}
GET /groups/{group-id}/drive/root:/{item-path}
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /sites/{siteId}/drive/items/{itemId}
GET /sites/{siteId}/drive/root:/{item-path}
GET /users/{userId}/drive/items/{itemId}
GET /users/{userId}/drive/root:/{item-path}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) `$expand` e `$select` para personalizar a resposta.

É possível usar o parâmetro de cadeia de caracteres de consulta [`$expand` ](/graph/query-parameters) para incluir os filhos de um item na mesma chamada de recuperação de metadados de um item se item tiver um relacionamento **children**.

## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Nome          | Valor  | Descrição                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | String | Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida. |

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna o código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Eis um exemplo de solicitação para a pasta raiz do OneDrive do usuário.

<!-- { "blockType": "request", "name": "get-drive-root", "tags": "service.graph" }-->

```http
GET /me/drive/root
```

## <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "createdDateTime": "2016-03-21T20:01:37Z",
  "cTag": "\"c:{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},0\"",
  "eTag": "\"{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},1\"",
  "folder": { "childCount": 120 },
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "lastModifiedBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "name": "OneDrive",
  "root": { },
  "size": 157286400,
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents"
}
```

## <a name="remarks"></a>Comentários

Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].

[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive-get-specialfolder.md

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item"
} -->
