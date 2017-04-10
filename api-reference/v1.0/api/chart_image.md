# <a name="chart-image"></a>Chart: Image

Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.
## <a name="prerequisites"></a>Pré-requisitos
Os seguintes **escopos** são necessários para executar esta API: 
## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets(<id|name>)/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | <code> de portador|


## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|height|number|Opcional. A altura desejada da imagem resultante.|
|width|number|Opcional. A largura desejada da imagem resultante.|
|fittingMode|cadeia de caracteres|Opcional. O método usado para dimensionar o gráfico para as dimensões especificadas (se height e width tiverem sido definidas).  Os valores possíveis são: `Fit`, `FitAndCenter` e `Fill`.|

## <a name="response"></a>Resposta
Se bem sucedido, este método retorna o código de resposta `200, OK` e a cadeia de caracteres de imagem em base64 no corpo da resposta.

## <a name="example"></a>Exemplo
Eis um exemplo de como chamar esta API.
##### <a name="request"></a>Solicitação
Veja a seguir um exemplo da solicitação.
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets(<id|name>)/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
Content-type: application/json
Content-length: 77

{
  "height": {
  },
  "width": {
  },
  "fittingMode": "fittingMode-value"
}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
