# <a name="add-named-item-formulalocal"></a>Adicionar item nomeado FormulaLocal
Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.

## <a name="prerequisites"></a>Pré-requisitos
Um dos seguintes **escopos** é obrigatório para executar esta API:

  * Files.ReadWrite
  * Sites.Read.All
  
## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | Portador {código}|


## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|name|string|O nome do item nomeado.|
|formula|string|A fórmula ou o intervalo ao qual o nome fará referência.|
|comentário|string|O comentário associado ao item nomeado|

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [NamedItem](../resources/NamedItem.md) no corpo da resposta.

## <a name="example"></a>Exemplo
Eis um exemplo de como chamar esta API.
##### <a name="request"></a>Solicitação
Veja a seguir um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "myRange",
  "formula": "=A10+B10",
  "comment": "Comment for the named item"
}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "name": "myRange",
  "comment": "Sample range",
  "scope": "Workbook",
  "type": "String",
  "visible": true,
  "value": "=A10+B10"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
