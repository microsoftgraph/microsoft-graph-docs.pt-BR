---
author: JeremyKelley
title: Obter pacote
description: Obter um pacote de driveItems
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 41d8c613095e9a3b167f25f457167ca3393fb207
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561568"
---
# <a name="get-bundle"></a>Obter pacote

Namespace: microsoft.graph

Recupere os metadados de [um pacote][] com base na ID exclusiva do pacote.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte.                             |
|Delegado (conta pessoal da Microsoft) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Aplicativo          | Sem suporte.                                           |

## <a name="http-request"></a>Solicitação HTTP

```http
GET /drive/bundles/{bundle-id}
GET /drive/items/{bundle-id}
```

Como os pacotes são itens, você pode usar a coleção **items** para retornar metadados sobre um pacote.
Você também pode usar a coleção **bundles** como uma conveniência para garantir que você está recebendo um pacote em resposta.

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Você pode usar os [parâmetros de consulta OData][odata-parameters] para restringir a forma dos objetos retornados dessa chamada.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição  |
|:------------- |:------------ |
| Autorização | \{token\} de portador. Obrigatório. |
| if-none-match | eTag. Opcional. Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será retornada.

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação com esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará [um driveItem][driveItem] resource with the [bundle][bundle] no corpo da resposta.

Para obter informações sobre respostas de erro, consulte [Respostas de erro][error-response].

## <a name="examples"></a>Exemplos

### <a name="example-1-get-a-bundle"></a>Exemplo 1: Obter um pacote

#### <a name="request"></a>Solicitação

<!-- { "blockType": "request", "name": "get-bundle-metadata" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles/{bundle-id}
```

#### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "My Photo Album Bundle",
  "eTag": "etag",
  "cTag": "etag",
  "createdBy": { "user": { "id": "1234", "displayName": "Ryan Gregg" } },
  "createdDateTime": "datetime",
  "lastModifiedBy": { "user": { "id": "1234", "displayName": "Ryan Gregg" } },
  "lastModifiedDateTime": "datetime",
  "size": 1234,
  "webUrl": "http://onedrive.com/...",
  "bundle": {
    "childCount": 4,
     "album": { }
  }
}
```

O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.

### <a name="example-2-get-a-bundle-and-its-children-in-a-single-call"></a>Exemplo 2: Obter um pacote e seus filhos em uma única chamada

Você pode usar o [`expand`](/graph/query-parameters) parâmetro de cadeia de caracteres de consulta para incluir os filhos de um pacote na mesma chamada que recuperar os metadados de um pacote.

#### <a name="request"></a>Solicitação

<!-- { "blockType": "request", "name": "get-bundle-and-children" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{bundle-id}?expand=children
```

#### <a name="response"></a>Resposta

Essa chamada retornará os metadados do pacote e uma lista de filhos do pacote.
Se o pacote não tiver filhos, ele retornará uma coleção vazia.

Se o número de filhos no pacote for maior do que o tamanho padrão da página, a propriedade **children@odata.nextLink** será retornada com uma URL que pode ser usada para solicitar a próxima página de filhos no pacote.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "101230100alkc",
  "name": "My Cool Day at the Beach",
  "children": [
    { "id": "120100abab", "name": "image1.jpg", "file": {} },
    { "id": "120100abo1", "name": "image2.jpg", "file": {} }
  ],
  "children@odata.nextLink": "https://api.onedrive.com/v1.0/..."
}
```

O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters


<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about a bundle and its children in OneDrive",
  "keywords": "retrieve,item,bundle,metadata",
  "section": "documentation",
  "tocPath&quot;: &quot;Bundles/Get Bundle Metadata"
} -->


