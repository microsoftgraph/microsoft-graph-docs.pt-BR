# <a name="historyitem-resource-type"></a>Tipo de recurso historyItem

Representa um item de histórico de uma [atividade](projectrome_activity.md) em um aplicativo. As atividades do usuário representam um único destino dentro de seu aplicativo - por exemplo, um programa de TV, um documento ou uma campanha atual em um jogo de vídeo. Quando um usuário se compromete com a atividade, o compromisso é capturado como um item do histórico que indica a hora de início e término para a atividade. À medida que o usuário se compromete novamente com essa atividade ao longo do tempo, vários itens do histórico são registrados para cada atividade do usuário.

Quando um aplicativo cria uma sessão, um objeto **historyItem** deve ser adicionado ao objeto **activity** para refletir o período de compromisso do usuário. Cada vez que um usuário se compromete novamente com uma atividade, um novo **historyItem** é adicionado à atividade para acumular compromisso do usuário.

## <a name="methods"></a>Métodos

|Método | Tipo de retorno | Descrição|
|:------|:------------|:-----------|
|[Criar ou substituir historyItem](../api/projectrome_put_historyitem.md) | [historyItem](projectrome_historyitem.md) | Cria ou substitui um **historyItem** existente para a atividade (upsert). A ID deve ser um GUID.|
|[Excluir um historyItem](../api/projectrome_delete_historyitem.md) | Nenhum conteúdo | Exclui o **historyItem** especificado para a atividade.|

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|status | status | Definido pelo servidor. Um código de status usado para identificar objetos válidos. Valores: ativo, atualizado, excluído, ignorado.|
|userTimezone | Sequência de caracteres | Opcional. O fuso horário no qual o dispositivo do usuário usado para gerar a atividade foi localizado no momento da criação de atividade. Valores fornecidos como Olson IDs para suportar a representação de plataforma cruzada.|
|createdDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto foi criado no servidor.|
|lastModifiedDateTime | DateTimeOffset | Definido pelo servidor. DateTime em UTC quando o objeto foi modificado no servidor.|
|id | Cadeia de caracteres | Obrigatório. GUID do conjunto de cliente para o objeto **historyItem**.|
|startedDateTime | DateTimeOffset | Obrigatório. DateTime UTC quando o **historyItem** (sessão de atividade) foi iniciado. Obrigatório para o histórico de linha do tempo.|
|lastActiveDateTime | DateTimeOffset | Opcional. DateTime UTC quando o **historyItem** (sessão de atividade) foi compreendido como status ativo ou concluído - se for nulo, o status do **historyItem** deve ser contínuo.|
|expirationDateTime | DateTimeOffset | Opcional. DateTime UTC quando o **historyItem** passará por exclusão irreversível. Pode ser definido pelo cliente.|
|activeDurationSeconds | int | Opcional. A duração de participação de usuário ativo. se não fornecido, isso é calculado do **startedDateTime** e **lastActiveDateTime**.|

## <a name="relationships"></a>Relações

|Relação | Tipo | Descrição|
|:------------|:-----|:-----------|
|atividade| [userActivity](../resources/projectrome_activity.md) | Opcional. NavigationProperty/Containment; propriedade de navegação à atividade associada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
