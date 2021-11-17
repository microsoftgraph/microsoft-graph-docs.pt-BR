---
author: JeremyKelley
ms.date: 09/10/2017
title: Obter Unidade
ms.localizationpriority: high
ms.prod: sharepoint
description: Recupere as propriedades e as relações de um recurso Drive.
doc_type: apiPageType
ms.openlocfilehash: d8f8f9463cad0eeac2fc5a0ae3e3c7a8cd7a948d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006474"
---
# <a name="get-drive"></a>Obter Unidade

Namespace: microsoft.graph

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


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-drive-default-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a>Obtenha o OneDrive de um usuário

Para acessar o OneDrive ou o OneDrive for Business de um usuário, seu aplicativo deve solicitar a relação **drive** no recurso User.

Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.

### <a name="http-request"></a>Solicitação HTTP


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-drive-by-user-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a>Parâmetros do caminho

| Nome do parâmetro | Valor  | Descrição                                       |
|:---------------|:-------|:--------------------------------------------------|
| _idOrUserPrincipalName_     | string | Obrigatório. O identificador do objeto de usuário que possui o OneDrive. |

## <a name="get-the-document-library-associated-with-a-group"></a>Obtenha a biblioteca de documentos associada a um grupo

Para acessar uma biblioteca de documentos padrão de um Grupo, o aplicativo solicita a relação **drive** no grupo.

### <a name="http-request"></a>Solicitação HTTP


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /groups/{groupId}/drive
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-drive-by-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a>Parâmetros do caminho

| Nome do parâmetro | Valor  | Descrição                                       |
|:---------------|:-------|:--------------------------------------------------|
| _groupId_      | string | Obrigatório. O identificador do grupo que possui a biblioteca de documentos. |

## <a name="get-the-document-library-for-a-site"></a>Obter a biblioteca de documentos de um site

Para acessar uma biblioteca de documentos padrão [de um Site](../resources/site.md), o aplicativo solicita a relação **drive** no Site.

### <a name="http-request"></a>Solicitação HTTP


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /sites/{siteId}/drive
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-site-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-drive-by-site-id-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a>Parâmetros do caminho

| Nome do parâmetro | Valor  | Descrição                                       |
|:---------------|:-------|:--------------------------------------------------|
| _siteId_       | string | Obrigatório. O identificador do site que contém a biblioteca de documentos. |

## <a name="get-a-drive-by-id"></a>Obtenha uma unidade por ID

Se tiver o identificador exclusivo de uma unidade, você poderá acessá-lo diretamente da coleção de unidades de nível superior.

### <a name="http-request"></a>Solicitação HTTP


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```msgraph-interactive
GET /drives/{drive-id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-drive-by-id-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a>Parâmetros do caminho

| Nome do parâmetro | Valor  | Descrição                                       |
|:---------------|:-------|:--------------------------------------------------|
| _driveId_      | cadeia de caracteres | Obrigatório. O identificador da unidade solicitada. |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método é compatível com o [parâmetro de consulta $select][odata-query-parameters] para formar a resposta.

## <a name="response"></a>Resposta

Cada um desses métodos retorna um [Recurso de Unidade][drive-resource] para a unidade correspondente no corpo da resposta.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default" , "get-drive-by-site-id"] } -->

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
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Microsoft 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath&quot;: &quot;Drives/Get drive"
} -->

