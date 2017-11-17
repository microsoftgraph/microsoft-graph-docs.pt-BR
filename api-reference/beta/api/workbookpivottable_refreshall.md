# <a name="workbookpivottable-refreshall"></a>workbookPivotTable: refreshAll

Atualiza a tabela dinâmica dentro de uma determinada planilha.

### <a name="prerequisites"></a>Pré-requisitos
Os seguintes **escopos** são necessários para executar esta API: _Files.Read, Files.ReadWrite_
### <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
### <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | Portador {código}|
| Workbook-Session-Id  | ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.|

### <a name="request-body"></a>Corpo da solicitação

### <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.

### <a name="example"></a>Exemplo
Eis um exemplo de como chamar esta API.
##### <a name="request"></a>Solicitação
Veja a seguir um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/{ver}/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
