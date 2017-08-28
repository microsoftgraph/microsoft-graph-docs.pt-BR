# <a name="list-thumbnails-for-a-driveitem"></a>Listar miniaturas para um DriveItem

Recupere uma coleção de recursos [ThumbnailSet](../resources/thumbnailset.md) para um recurso [DriveItem](../resources/driveitem.md).

Um DriveItem pode ser representado por zero ou mais recursos [ThumbnailSet](../resources/thumbnailset.md). Cada **thumbnailSet** pode ter um ou mais objetos [**thumbnail**](../resources/thumbnail.md), que são imagens que representam o item. Por exemplo, um **thumbnailSet** podem incluir objetos **thumbnail**, como objetos comuns que incluem `small`, `medium` ou `large`.

Há várias maneiras de trabalhar com miniaturas no OneDrive. Veja a seguir as mais comuns:

* Enumerar miniaturas disponíveis para um item
* Recuperar uma única miniatura para um item
* Recuperar o conteúdo da miniatura
* Recuperar miniaturas de vários itens em uma única solicitação
* Recuperar tamanhos personalizados de miniaturas
* Carregar uma miniatura personalizada para um item
* Determinar se uma miniatura personalizada carregada existe


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              | 
|:--------------------|:---------------------------------------------------------| 
|Delegado (conta corporativa ou de estudante) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    | 
|Delegado (conta pessoal da Microsoft) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    | 
|Aplicativo | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All | 

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [ThumbnailSet](../resources/thumbnailset.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

<!-- {
  "blockType": "request",
  "name": "get_thumbnails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails
```


##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0",
      "small": { "height": 64, "width": 96, "url": "https://sn3302files..."},
      "medium": { "height": 117, "width": 176, "url": "https://sn3302files..."},
      "large": { "height": 533, "width": 800, "url": "https://sn3302files..."}
    }
  ]
}
```

## <a name="retrieve-a-single-thumbnail"></a>Recuperar uma única miniatura

Recupere os metadados de uma única miniatura e tamanho tratando-os diretamente em uma solicitação.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "request", "name": "get-one-thumbnail" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

## <a name="path-parameters"></a>Parâmetros do caminho

| Nome         | Tipo   | Descrição                                                                         |
|:-------------|:-------|:------------------------------------------------------------------------------------|
| **item-id**  | string | O identificador exclusivo do item referenciado.                                      |
| **thumb-id** | number | O índice da miniatura, geralmente de 0 a 4.                                            |
| **size**     | string | O tamanho da miniatura solicitada. Ele deve ser um dos tamanhos padrão listados. |


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "http://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-content"></a>Recuperar o conteúdo da miniatura

Você pode recuperar diretamente o conteúdo da miniatura solicitando a propriedade **content** dessa miniatura.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "request", "name":"get-thumbnail-content" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

## <a name="response"></a>Resposta

O serviço responde com um redirecionamento para a URL da miniatura.

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

URLs de conteúdo de miniaturas são pré-autenticadas e não exigem o download de um cabeçalho de autorização. Essas URLs são de curta duração, permanecem válidas somente por algumas horas e não devem ser armazenadas em cache por aplicativos.


## <a name="size-values"></a>Valores de tamanho

Essa tabela define os possíveis tamanhos de miniaturas. Embora você possa solicitar qualquer tamanho de miniatura arbitrário, os valores definidos provavelmente existem e retornam um valor rapidamente:

| Nome           | Resolução  | Taxa de proporção | Descrição                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | 96 mais longa  | Original     | Miniatura pequena e altamente compactada, recortada em uma taxa de proporção quadrada. |
| `medium`       | 176 mais longa | Original     | Recortada no tamanho do item padrão para o modo de exibição de Web do OneDrive.         |
| `large`        | 800 mais longa | Original     | Miniatura com a borda mais longa redimensionada para 800 pixels.               |

## <a name="remarks"></a>Comentários

**Observação** No OneDrive for Business e no SharePoint:

* O uso dessas chamadas para expandir a coleção de miniaturas não funcionará: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->
