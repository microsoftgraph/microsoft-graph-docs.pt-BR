---
author: JeremyKelley
ms.date: 09/10/2017
title: Listar quem tem acesso a um arquivo
ms.localizationpriority: medium
ms.prod: sharepoint
description: Listar as permissões de compartilhamento eficazes de em um driveItem.
doc_type: apiPageType
ms.openlocfilehash: dd18d5874be75d76fbd724b2c52e7b84bede420e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063444"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a>Listar permissões de compartilhamento em um driveItem

Namespace: microsoft.graph

Listar as permissões de compartilhamento eficazes em [um driveItem](../resources/driveitem.md).

## <a name="access-to-sharing-permissions"></a>Acessar permissões de compartilhamento

A coleção de permissões inclui informações potencialmente confidenciais e pode não estar disponível para todos os chamadores.

* Para o proprietário do item, todas as permissões de compartilhamento serão retornadas. Isto inclui os coproprietários.
* Para um chamador não proprietário, somente as permissões de compartilhamento que se aplicam ao chamador são retornadas.
* Propriedades de permissão de compartilhamento que contêm segredos (por exemplo, `shareId` e `webUrl`) são retornadas somente para chamadores que são capazes de criar a permissão de compartilhamento.

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
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$select` para personalizar as resposta.

## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Name          | Tipo   | Descrição                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | string | Se este cabeçalho de solicitação estiver incluso e a etag fornecida corresponder à marca atual do item, uma resposta `HTTP 304 Not Modified` será exibida. |

## <a name="response"></a>Resposta

Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de recursos [Permission](../resources/permission.md) no corpo da resposta.

As permissões efetivas de compartilhamento de um DriveItem podem vir de duas fontes:

* Permissões de compartilhamento aplicadas diretamente ao próprio DriveItem
* Permissões de compartilhamento herdadas de ancestrais do DriveItem

Os chamadores podem diferenciar se a permissão é herdada ou não verificando a propriedade **inheritedFrom**. Esta propriedade é um recurso [**itemReference**](../resources/itemreference.md) que referencia o ancestral do qual a permissão é herdada.

## <a name="example"></a>Exemplo

Este exemplo recupera a coleção de permissões em um item na unidade do usuário conectado.

# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/permissions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-permissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-permissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-permissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-permissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Esta resposta de exemplo inclui três permissões, a primeira é um link de compartilhamento com permissões de edição, a segunda é uma permissão explícita para um usuário chamado John, que foi herdada da pasta pai, e a terceira é um link de compartilhamento de leitura e gravação criado por um aplicativo.

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "Contoso Time Manager"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a>Comentários

A relação **permissions** de um DriveItem não pode ser expandida como parte de uma chamada para [get DriveItem](driveitem-get.md) ou uma coleção de DriveItems. Você deve acessar a propriedade permissions diretamente.

## <a name="error-responses"></a>Respostas de erro

Leia o tópico [Respostas de Erro][error-response] para obter mais informações sobre como os erros são retornados.

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions",
  "suppressions": [
  ]
} -->
