# <a name="worksheetprotection-resource-type"></a>Tipo de recurso WorksheetProtection

Representa a proteção de um objeto de planilha.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get WorksheetProtection](../api/worksheetprotection_get.md) | [WorksheetProtection](worksheetprotection.md) |Leia as propriedades e os relacionamentos do objeto worksheetProtection.|
|[Protect](../api/worksheetprotection_protect.md)|Nenhum|Protege uma planilha. Gera uma exceção se a planilha estiver protegida.|
|[Unprotect](../api/worksheetprotection_unprotect.md)|Nenhum|Desprotege uma planilha.|

## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|protected|booliano|Indica se a planilha está protegida.  Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|options|[WorksheetProtectionOptions](worksheetprotectionoptions.md)|Opções de proteção da planilha. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtection"
}-->

```json
{
  "protected": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->