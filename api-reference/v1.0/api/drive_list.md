---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Listar unidades
ms.openlocfilehash: 84771e589a65d11fc06707eb01b6211cf90a8581
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="list-available-drives"></a>Listar as unidades disponíveis

Recupera a lista de recursos [Drive](../resources/drive.md) disponíveis para um User, Group ou [Site](../resources/site.md) de destino.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Aplicativo | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="list-a-groups-drives"></a>Lista as unidades de um grupo

Para listar as bibliotecas de documentos de um grupo, seu aplicativo solicita a relação de **unidades** no Grupo.

### <a name="http-request"></a>Solicitação HTTP

<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all" } -->

```http
GET /groups/{groupId}/drives
```

## <a name="list-a-sites-drives"></a>Lista as unidades do site

Para listar as bibliotecas de documentos de um site, seu aplicativo solicita a relação de **unidades** no Site.

<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all" } -->

```http
GET /sites/{siteId}/drives
```

## <a name="list-a-users-drives"></a>Lista as unidades de um usuário

<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read.all" } -->

```http
GET /users/{userId}/drives
```

## <a name="list-the-current-users-drives"></a>Lista as unidades do usuário atual

<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read" } -->

```http
GET /me/drives
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método oferece suporte aos [parâmetros de consulta OData](../../../concepts/query_parameters.md) `$expand`, `$select`, `$skipToken`, `$top` e `$orderby` para personalizar a resposta.


## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Drive](../resources/drive.md) no corpo da resposta.

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.drive)",
       "name": ["group-list-drives", "site-list-drives", "user-list-drives", "enum-drives"],
       "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "942CAEB0-13AE-491B-85E4-7557CDC0F25F",
      "driveType": "documentLibrary",
      "name": "Shared Documents",
      "owner": {
        "user": {
          "id": "AE2A1EE9-81A7-423C-ABE4-B945F47509BB",
          "displayName": "Ryan Gregg"
        }
      }
    },
    {
      "id": "C1CD3ED9-0E98-4B0B-82D3-C8FB784B9DCC",
      "driveType": "documentLibrary",
      "name": "Contoso Project Files",
      "owner": {
        "user": {
          "id": "406B2281-18E8-4416-9857-38C531B904F1",
          "displayName": "Daron Spektor"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a>Comentários

A maioria dos usuários só terá um único recurso Drive.

Grupos e Sites podem ter vários recursos de unidade disponíveis.

Unidades com a faceta [sistema][] estão ocultas por padrão.
Para listá-los, inclua `system` na instrução `$select`.

[system]: ../resources/systemFacet.md

<!-- {
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives"
} -->
