# <a name="process-resource-type"></a>tipo de recurso processo

Contém informações com estado sobre o processo relacionado ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|accountName|Sequência de caracteres|Identificador da conta do usuário (o contexto de conta do usuário no qual o processo foi executado) por exemplo, AccountName, SID, entre outros.|
|commandLine|Sequência de caracteres|A commandline de invocação do processo completo, incluindo todos os parâmetros.|
|createdDateTime|DateTimeOffset|Hora em que o processo foi iniciado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|fileHash|[fileHash](filehash.md)|Tipo Complex contendo hashes de arquivo (criptográficos e sensíveis à localização).|
|integrityLevel|processIntegrityLevel|O nível de integridade do processo. Os valores possíveis são: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.|
|isElevated|Booleano|True se o processo for elevado.|
|name|Sequência de caracteres|O nome do arquivo de imagem do processo.|
|parentProcessCreatedDateTime|DateTimeOffset|Data e hora em que o processo pai foi iniciado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|parentProcessId|Int32|A ID de Processo (PID) do processo pai.|
|parentProcessName|Sequência de caracteres|O nome do arquivo de imagem do processo pai.|
|path|Sequência de caracteres|Caminho completo, incluindo nome do arquivo.|
|processId|Int32|A ID de Processo (PID) do processo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->