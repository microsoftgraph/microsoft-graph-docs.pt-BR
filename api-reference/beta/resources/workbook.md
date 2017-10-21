# <a name="workbook-resource-type"></a>Tipo de recurso de pasta de trabalho

A pasta de trabalho é o objeto de nível superior que inclui os objetos workbook relacionados, como planilhas, tabelas, intervalos, etc.

## <a name="properties"></a>Propriedades
Nenhuma

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar Sessão](../api/workbook_createsession.md) | [workbookSessionInfo](workbooksessioninfo.md) |Crie uma sessão de pasta de trabalho para iniciar uma sessão persistente ou não persistente.|
|[Fechar Sessão](../api/workbook_closesession.md) | None |Fechar uma sessão existente.|
|[Atualizar Sessão](../api/workbook_refreshsession.md) | None |Atualizar uma sessão existente.|


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|names|Coleção [NamedItem](nameditem.md)|Representa uma coleção de itens denominados de escopo da pasta de trabalho (chamados intervalos e constantes). Somente leitura.|
|tabelas|Coleção [Table](table.md)|Representa uma coleção de tabelas associadas à pasta de trabalho. Somente leitura.|
|worksheets|Coleção [Worksheet](worksheet.md)|Representa uma coleção de planilhas associadas à pasta de trabalho. Somente leitura.|

## <a name="functions"></a>Funções

[Funções do Excel](#functions): Invoque uma função de pasta de trabalho usando a sintaxe `POST /workbook/functions/{function-name}` e fornecendo os argumentos de função no corpo usando um objeto JSON. O `value` resultante da função e quaisquer cadeias de caracteres `error` são retornados no objeto de resultado de função. O valor `error` de `null` indica a execução bem-sucedida da função. 

A lista completa de funções com suporte está listada [aqui](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Confira a assinatura de função para tipos de dados e nomes de parâmetro específicos.

_Observações importantes:_ 
* O parâmetro de entrada do intervalo é fornecido usando um objeto range, em vez da cadeia de caracteres de endereço do intervalo.  
* O parâmetro index é indexado como -1, diferentemente do índice 0 usado na maioria das APIs. 

Exemplo: 

No exemplo abaixo, a função `vlookup` é chamada passando o valor de pesquisa, o intervalo de entrada e o valor a ser retornado. 

Solicitação: 

```http 
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/vlookup
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
    "lookupValue": "Temperature",
    "tableArray": { "Address": "Sheet1!E1:G5" },
    "colIndexNum": 2,
    "rangeLookup": false
}
```

Resposta:

```http
HTTP code: 200, OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

Exemplo: 

No exemplo abaixo, a função `median` é chamada passando o(s) intervalo(s) de entrada em uma matriz. 

Solicitação: 

```http 
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/median
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"values" :  [
        { "address": "Sheet2!A1:A5" },
        { "address": "Sheet2!B1:B5" },
      ] 
}
```

Resposta:

```http
HTTP code: 200, OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
  "@odata.type": "#microsoft.graph.workbookFunctionResult",
  "@odata.id": "/users('2abcad6a-2fca-4b6e-9577-e358a757d77d')/drive/root/workbook/functions/median()",
  "error": null,
  "value": 30
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Workbook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
