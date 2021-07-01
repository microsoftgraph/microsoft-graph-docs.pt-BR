---
author: JeremyKelley
description: Use a coleção especial para acessar uma pasta especial pelo nome.
title: Obter Pastas Especiais
localization_priority: Normal
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: 48a20da153eaf1e74d34b2ecfa3b7c30f8a794aa
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236174"
---
# <a name="get-a-special-folder-by-name"></a>Obtenha uma pasta especial por nome

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use a coleção especial para acessar uma pasta especial pelo nome.

Pastas especiais fornecem aliases simples para acessar pastas conhecidas no OneDrive sem a necessidade de pesquisar a pasta pelo caminho (o que exigiria a localização) ou fazer referência à pasta com uma ID. Se uma pasta especial for renomeada ou movida para outro local na unidade de disco, esta sintaxe continuará a localizar a pasta.

As pastas especiais são criadas automaticamente na primeira vez que um aplicativo tenta gravar em uma, caso ainda não existam. Se um usuário excluir uma, ela será recriada quando algo for gravado nela novamente.

> **Observação:**  Se tiver permissões somente leitura e solicitar uma pasta especial que não exista, você receberá um erro `403 Forbidden`.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|            Tipo de permissão             |                                           Permissões (da com menos para a com mais privilégios)                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All                            |
| Delegado (conta pessoal da Microsoft) | Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |
| Aplicativo                            | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All                                                         |

## <a name="http-request"></a>Solicitação HTTP


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/special/{name}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-folder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-folder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-folder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-special-folder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="special-folder-names"></a>Nomes de pasta especial
[!INCLUDE [files-special-folder-list](../includes/files-special-folder-list.md)]


### <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) `$expand` e `$select` para personalizar a resposta.

## <a name="response"></a>Resposta

Este método retorna um código de resposta `200 OK` e um objeto [driveItem](../resources/driveitem.md) no corpo da resposta.

Você pode usar esse método de lidar com uma pasta especial em linha com chamadas adicionais para propriedades ou relações no driveItem.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "Documents",
  "eTag": "012345819293.1",
  "specialFolder": {
    "name": "documents"
  }
}
```

## <a name="get-children-of-a-special-folder"></a>Obter filhos de uma pasta especial

Para solicitar os filhos de uma pasta especial, você pode solicitar a coleção `children` ou usar a opção [expand](/graph/query-parameters) para expandir a coleção de filhos.

### <a name="http-request"></a>Solicitação HTTP


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/special/{name}/children
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-special-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048 },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ]
}
```

## <a name="remarks"></a>Comentários

> **Observação:** A faceta `specialFolder` de DriveItems indica que o item é uma pasta especial e pode ser acessado pelo conjunto `special`.

Se seu aplicativo tiver permissões somente leitura, a solicitação para obter uma pasta especial ou os filhos de uma pasta especial poderá falhar com um erro `404 Not Found` ou `403 Forbidden`, se a pasta especial ainda não existir.

<!--
{
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders",
  "suppressions": [
  ]
}
-->


