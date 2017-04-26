# <a name="upload-or-replace-the-contents-of-a-driveitem"></a>Carregue ou substitua o conteúdo de um driveItem

A API de upload simples permite que você forneça o conteúdo de um novo arquivo ou atualize o conteúdo de um arquivo existente em uma única chamada à API. Este método só dá suporte a arquivos com até 4 MB de tamanho.

Para carregar arquivos grandes, confira [Carregar arquivos grandes com uma sessão de carregamento](item_createuploadsession.md).

## <a name="prerequisites"></a>Pré-requisitos
Um dos seguintes **escopos** é obrigatório para executar esta API:

  * Files.ReadWrite

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/root:/{parent-path}/{filename}:/content
PUT /me/drive/items/{parent-id}/children/{filename}/content
PUT /groups/{id}/drive/items/{parent-id}/children/{filename}/content
```

## <a name="request-body"></a>Corpo da solicitação
O conteúdo do corpo da solicitação deve ser o fluxo binário do arquivo a ser carregado.

## <a name="response"></a>Resposta
Se for bem-sucedido, este método retornará um objeto [driveItem](../resources/driveitem.md) no corpo da resposta para o arquivo recém-criado.

## <a name="example"></a>Exemplo
Este exemplo carrega um arquivo pelo caminho do OneDrive do usuário conectado.

<!-- {
  "blockType": "request",
  "name": "upload_item"
}-->
```http
PUT /me/drive/root:/{item-path}:/content
Content-type: text/plain

The contents of the file goes here.
```

## <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "myfile.jpg",
  "size": 10191,
  "file": { }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
