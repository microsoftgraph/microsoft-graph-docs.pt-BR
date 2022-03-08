---
author: JeremyKelley
title: Baixar um arquivo
ms.localizationpriority: high
ms.prod: sharepoint
description: Baixar o conteúdo do fluxo principal (arquivo) de um driveItem. Somente driveItems com a propriedade file podem ser baixados.
doc_type: apiPageType
ms.openlocfilehash: 5e5e3a2b9d174957b80c0a74e96d3a658279e44d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336330"
---
# <a name="download-the-contents-of-a-driveitem"></a>Baixe o conteúdo de um DriveItem

Namespace: microsoft.graph

[!INCLUDE [tls-1.2-required](../../includes/tls-1.2-required.md)]

Baixar o conteúdo do fluxo principal (arquivo) de um [driveItem](../resources/driveitem.md). Somente **driveItems** com a propriedade **file** podem ser baixados.

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
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /shares/{shareIdOrEncodedSharingUrl}/driveItem/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Nome          | Valor  | Descrição                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | String | Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida. |

## <a name="example"></a>Exemplo

Aqui está um exemplo para baixar um arquivo completo.

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/content
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/download-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/download-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/download-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/download-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada do arquivo. Esta é a mesma URL disponível por meio da propriedade `@microsoft.graph.downloadUrl` no DriveItem.

Para baixar o conteúdo do arquivo, seu aplicativo precisará seguir o cabeçalho `Location` na resposta. Várias bibliotecas de cliente HTTP seguirão automaticamente o redirecionamento 302 e começarão a baixar imediatamente o arquivo.

URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não requerem um cabeçalho `Authorization` para download.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="downloading-files-in-javascript-apps"></a>Download de arquivos em aplicativos JavaScript
Para baixar arquivos em um aplicativo JavaScript, não é possível usar a API `/content`, pois isso responde com um redirecionamento `302`. O redirecionamento `302` é explicitamente proibido quando uma [simulação](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) do _Cross-Origin Resource Sharing (CORS)_ é necessária, como ao fornecer o cabeçalho **Authorization**.

Em vez disso, seu aplicativo precisa selecionar a propriedade `@microsoft.graph.downloadUrl`, que retorna o mesmo URL para o qual `/content` direciona.
Essa URL pode ser solicitada diretamente usando XMLHttpRequest.
Como essas URLs são previamente autenticadas, podem ser recuperadas sem uma solicitação de simulação de CORS.

### <a name="example"></a>Exemplo

Para recuperar a URL de download de um arquivo, faça primeiro uma solicitação que inclua a propriedade `@microsoft.graph.downloadUrl`:

```http
GET /drive/items/{item-ID}?select=id,@microsoft.graph.downloadUrl
```

Isso retornará a ID e o URL de download para um arquivo:

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "12319191!11919",
  "@microsoft.graph.downloadUrl": "https://..."
}
```

Você pode fazer uma XMLHttpRequest para a URL fornecida em `@microsoft.graph.downloadUrl` para recuperar o arquivo.

## <a name="partial-range-downloads"></a>Downloads de intervalo parcial

Para baixar um intervalo parcial de bytes do arquivo, o aplicativo pode usar o cabeçalho `Range` conforme especificado em [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Observe que você deve acrescentar o cabeçalho `Range` à URL `@microsoft.graph.downloadUrl` real e não à solicitação para `/content`.

<!-- { "blockType": "request", "opaqueUrl": true, "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

Isso retornará uma resposta `HTTP 206 Partial Content` com o intervalo de solicitação de bytes do arquivo. Se o intervalo não puder ser gerado, o cabeçalho do Intervalo poderá ser ignorado, e uma resposta `HTTP 200` será retornada com todo o conteúdo do arquivo.

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048
Content-Type: application/octet-stream

<first 1024 bytes of file>
```

### <a name="error-responses"></a>Respostas de erro

Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Download the contents of a DriveItem.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Items/Download",
  "suppressions": [
  ]
} -->

