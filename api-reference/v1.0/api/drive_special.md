# <a name="get-a-special-folder-by-name"></a>Obtenha uma pasta especial por nome

Use a coleção especial para acessar uma pasta especial pelo nome.

Pastas especiais fornecem aliases simples para acessar pastas conhecidas no OneDrive sem a necessidade de pesquisar a pasta pelo caminho (o que exigiria a localização) ou fazer referência à pasta com uma ID. Se uma pasta especial for renomeada ou movida para outro local na unidade de disco, esta sintaxe continuará a localizar a pasta.

As pastas especiais são criadas automaticamente na primeira vez que um aplicativo tenta gravar em uma, caso ainda não existam. Se um usuário excluir uma, ela será recriada quando algo for gravado nela novamente.

**Observação:**  Se tiver permissões somente leitura e solicitar uma pasta especial que não exista, você receberá um erro `403 Forbidden`.

## <a name="prerequisites"></a>Pré-requisitos
Um dos seguintes **escopos** é obrigatório para executar esta API:

* Files.Read
* Files.ReadWrite
* Files.Read.All
* Files.ReadWrite.All
* Files.ReadWrite.AppFolder
* Sites.Read.All
* Sites.ReadWrite.All

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/special/{name}
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Tipo   | Descrição               |
|:--------------|:-------|:--------------------------|
| Autorização | string | {token} de portador. Obrigatório. |


## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [driveItem](../resources/driveitem.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação
Eis um exemplo da solicitação de unidades do usuário.

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "folder": { },
  "id": "s!lkjqwlkj124912049an",
  "name": "Photos",
  "specialFolder": { "name": "photos" },
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents/Photos",
}
```

## <a name="remarks"></a>Comentários

Para solicitar os filhos de uma pasta especial, você pode solicitar a coleção `children` ou usar a opção [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para expandir a coleção de filhos.


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->
