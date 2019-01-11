---
author: chackman
ms.author: chackman
title: Listar itens visitados
localization_priority: Normal
ms.openlocfilehash: e8892bc96c53efef49f91d92b24b3ea97c937845
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849431"
---
# <a name="list-followed-items"></a>Listar itens visitados

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Lista os [itens](../resources/driveitem.md) que foram visitados pelo usuário conectado.
Esta coleção inclui itens que estão na unidade do usuário, bem como os itens que eles têm acesso a partir de outras unidades.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a>Resposta

Esse método retorna uma coleção de recursos de [driveItem](../resources/driveitem.md) para itens que o proprietário da unidade está seguindo.
Se nenhum item foi encontrado, uma coleção vazia é retornada.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "name": "March Proposal.docx",
      "size": 19121,
      "lastModifiedDateTime": "2017-12-12T10:40:59Z"
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "size": 37810,
      "lastModifiedDateTime": "2016-10-18T10:40:59Z"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items"
} -->
