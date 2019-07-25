---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Listar arquivos recentes
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e0e7d6fc4dc16f11f76b4c021f957a8ae580acba
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861499"
---
# <a name="list-recent-files"></a>Liste arquivos recentes

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Listar uma coleção de itens que foram usados recentemente pelo usuário conectado. Esta coleção inclui itens que estão na unidade do usuário, assim como itens aos quais ele tem acesso por meio de outras unidades.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Aplicativo | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- { "blockType": "request",
       "name": "view-recent-files", 
       "scopes": "files.read",
       "target": "action" } -->

```http
GET /me/drive/recent
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/view-recent-files-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/view-recent-files-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objetivo-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/view-recent-files-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/view-recent-files-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a>Resposta

Esse método retorna uma coleção de recursos [DriveItem](../resources/driveitem.md) para itens que o proprietário da unidade acessou recentemente.

<!-- { "blockType": "response",
       "@odata.type": "Collection(microsoft.graph.driveItem)",
       "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "remoteItem":
      {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T19:13:00Z"
      }
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "file": { },
      "size": 37810,
      "parentReference": {
        "driveId": "1312def",
        "id": "1312def!123"
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T16:43:21Z"
      }
    }
  ]
}
```

## <a name="remarks"></a>Comentários

Alguns driveItems retornados da ação **recent** incluirão a faceta **remoteItem** que indica que eles são itens de outra unidade. Para acessar o objeto driveItem original, você precisará fazer uma solicitação usando as informações fornecidas em **remoteItem** no seguinte formato:

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!--
{
  "type": "#page.annotation",
  "description": "Retrieve a list of recently used files for the owner of the drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Drives/Recent files",
  "suppressions": [
  ]
}
-->
