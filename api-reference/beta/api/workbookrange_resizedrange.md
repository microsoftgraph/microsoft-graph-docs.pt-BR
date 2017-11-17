# <a name="workbookrange-resizedrange"></a>workbookRange: resizedRange
Obtém um objeto range semelhante ao objeto range atual, mas com seu canto inferior direito expandido (ou recolhido) por um determinado número de linhas e colunas.

### <a name="prerequisites"></a>Pré-requisitos
Os seguintes **escopos** são necessários para executar esta API: _Files.Read, Files.ReadWrite_
### <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```
### <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | <code> de portador|
| Workbook-Session-Id  | ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.|

### <a name="parameters"></a>Parâmetros

| Parâmetro	       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|deltaRows|Int32|O número de linhas pelo qual expandir o canto inferior direito, referente ao intervalo atual. Use um número positivo para expandir o intervalo ou um número negativo para diminuí-lo|
|deltaColumns|Int32|O número de colunas pelo qual expandir o canto inferior direito, em relação ao intervalo atual. Use um número positivo para expandir o intervalo ou um número negativo para diminuí-lo.|

### <a name="request-body"></a>Corpo da solicitação
Forneça os seguintes parâmetros de consulta com valores na URL solicitada.

| Parâmetro       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|deltaRows|Int32||
|deltaColumns|Int32||

### <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `200, OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.

### <a name="example"></a>Exemplo
Eis um exemplo de como chamar esta API.
##### <a name="request"></a>Solicitação
Veja a seguir um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/{ver}/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
