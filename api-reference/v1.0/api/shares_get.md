# <a name="accessing-shared-driveitems"></a>Acessando DriveItems compartilhados

Acesse um [DriveItem](../resources/driveitem.md) compartilhado ou uma coleção de itens compartilhados usando um **shareId** ou uma URL de compartilhamento.

Para usar uma URL de compartilhamento com esta API, seu aplicativo precisa [transformar a URL em um token de compartilhamento](#transform-a-sharing-url).

## <a name="prerequisites"></a>Pré-requisitos

Um dos seguintes **escopos** é obrigatório para executar esta API:

* Files.ReadWrite
* Files.ReadWrite.All
* Sites.ReadWrite.All

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
GET /shares/{sharingIdOrUrl}
```

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [sharedDriveItem](../resources/shareddriveitem.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Veja a seguir um exemplo da solicitação para recuperar um item compartilhado:

<!-- {
  "blockType": "request",
  "name": "get_shares_by_url"
}-->
```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}
```
##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharedDriveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "B64397C8-07AE-43E4-920E-32BFB4331A5B",
  "name": "contoso project.docx",
  "owner": {
    "user": {
      "id": "98E88F1C-F8DC-47CC-A406-C090248B30E5",
      "displayName": "Ryan Gregg"
    }
  }
}
```

## <a name="access-the-shared-item-directly"></a>Acessar diretamente o item compartilhado

Embora [**SharedDriveItem**](../resources/shareddriveitem.md) contenha algumas informações úteis, a maioria dos aplicativos acessará diretamente o [DriveItem](../resources/driveitem.md) compartilhado. O recurso **SharedDriveItem** inclui **root** e relações **itens** que podem acessar o conteúdo no escopo do item compartilhado.

## <a name="example-single-file"></a>Exemplo (arquivo único)

##### <a name="request"></a>Solicitação

Solicitando a relação **root**, o **DriveItem** que foi compartilhado será retornado.

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root
```

##### <a name="response"></a>Resposta

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

## <a name="example-shared-folder"></a>Exemplo (pasta compartilhada)

##### <a name="request"></a>Solicitação

Solicitando a relação **root** e expandindo a coleção **children**, o **DriveItem** que foi compartilhado será retornado junto com os arquivos da pasta compartilhada.

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root?$expand=children
```

##### <a name="response"></a>Resposta

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {}
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <a name="transform-a-sharing-url"></a>Transformar uma URL de compartilhamento

Para acessar uma URL compartilhamento usando a API **shares**, a URL deve ser transformada em um token de compartilhamento.

Transformar uma URL em um token de compartilhamento:

1. Codifique na Base 64 a URL de compartilhamento.
2. Converta os dados codificados na Base 64 para o [formato base64url sem preenchimento](https://en.wikipedia.org/wiki/Base64) da seguinte forma:
  1. Cortar `=` caracteres à direita da cadeia de caracteres
  2. Substitua caracteres não seguros da URL por um caractere equivalente; substitua `/` por `_` e `+` por `-`.
3. Acrescente `u!` ao início da cadeia de caracteres.

Por exemplo, o seguinte método cC transforma uma cadeia de entrada em um token de compartilhamento:

```csharp
string UrlToSharingToken(string inputUrl) {
  var base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(inputUrl));
  return "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
