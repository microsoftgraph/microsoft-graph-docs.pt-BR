---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Obter Unidade
ms.openlocfilehash: 6ff71104c18a5a9354d18689c62a96be72b7fe12
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004713"
---
# <a name="get-drive"></a>Obter Unidade

Recupere as propriedades e as relações de um recurso [Drive](../resources/drive.md).

Uma unidade é um contêiner de nível superior para um sistema de arquivos como as bibliotecas de documentos do OneDrive ou do SharePoint.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Aplicativo | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="get-current-users-onedrive"></a>Obter o OneDrive do usuário atual

A unidade do usuário conectado (ao usar a autenticação delegada) poderá ser acessada pelo `me` singleton.

Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.

### <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a>Obtenha o OneDrive de um usuário

Para acessar o OneDrive ou o OneDrive for Business de um usuário, seu aplicativo deve solicitar a relação **drive** no recurso User.

Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.

### <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a>Parâmetros do caminho

| Nome do parâmetro | Valor  | Descrição                                       |
|:---------------|:-------|:--------------------------------------------------|
| _idOrUserPrincipalName_     | string | Obrigatório. O identificador de objeto do usuário proprietário do OneDrive. |

## <a name="get-the-document-library-associated-with-a-group"></a>Obtenha a biblioteca de documentos associada a um grupo

Para acessar uma biblioteca de documentos padrão de um Grupo, o aplicativo solicita a relação **drive** no grupo.

### <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a>Parâmetros do caminho

| Nome do parâmetro | Valor  | Descrição                                       |
|:---------------|:-------|:--------------------------------------------------|
| _groupId_      | string | Obrigatório. O identificador do grupo proprietário da biblioteca de documentos. |

## <a name="get-the-document-library-for-a-site"></a>Obter a biblioteca de documentos de um site

Para acessar uma biblioteca de documentos padrão [de um Site](../resources/site.md), o aplicativo solicita a relação **drive** no Site.

### <a name="http-request"></a>Solicitação HTTP

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a>Parâmetros do caminho

| Nome do parâmetro | Valor  | Descrição                                       |
|:---------------|:-------|:--------------------------------------------------|
| _siteId_       | string | Obrigatório. O identificador do site que contém a biblioteca de documentos. |

## <a name="get-a-drive-by-id"></a>Obtenha uma unidade por ID

Se tiver o identificador exclusivo de uma unidade, você poderá acessá-lo diretamente da coleção de unidades de nível superior.

### <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```

### <a name="path-parameters"></a>Parâmetros do caminho

| Nome do parâmetro | Valor  | Descrição                                       |
|:---------------|:-------|:--------------------------------------------------|
| _driveId_      | string | Obrigatório. O identificador da unidade solicitada. |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método é compatível com o [parâmetro de consulta $select][odata-query-parameters] para formar a resposta.

## <a name="http-response"></a>Resposta HTTP

Cada um desses métodos retorna um [recurso de unidade][drive-resource] para a unidade correspondente no corpo da resposta.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default"] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

### <a name="error-response-codes"></a>Códigos de resposta de erro

Se a unidade não existir e não puder ser provisionada automaticamente (ao usar autenticação delegada) uma resposta `HTTP 404` será retornada.

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/drive-get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get-drive-default, get-drive-by-user, get-drive-by-group, get-drive-by-id
            Unmapped tables:
        Permissions - AuthScopes, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters"
  ],
  "tocPath": "Drives/Get drive"
} -->
