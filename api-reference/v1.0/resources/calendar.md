# <a name="calendar-resource-type"></a>tipo de recurso calendar

Um calendário que é um contêiner para eventos.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar calendários](../api/user_list_calendars.md)|Coleção [calendar](calendar.md)|Obtenha todos os calendários do usuário ou os calendários no grupo de calendários padrão ou em outro grupo de calendários específico.|
|[Criar calendário](../api/user_post_calendars.md) |[calendar](calendar.md)| Crie um novo calendário no grupo de calendários padrão ou no calendário especificado.|
|[Obter calendário](../api/calendar_get.md) | [calendar](calendar.md) |Leia as propriedades e as ações do objeto calendar.|
|[Update](../api/calendar_update.md) | [calendar](calendar.md)  |Atualize o objeto calendar. |
|[Delete](../api/calendar_delete.md) | Nenhuma |Exclua um objeto calendar. |
|[Listar calendarView](../api/calendar_list_calendarview.md) |Coleção [event](event.md)| Obtenha as ocorrências, as exceções e as instâncias de eventos únicas em uma visão de calendário definida por um intervalo de tempo, do calendário principal do usuário `(../me/calendarview)` ou de um calendário especificado.|
|[Listar eventos](../api/calendar_list_events.md) |Coleção [event](event.md)| Recupere uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres em série.|
|[Criar Evento](../api/calendar_post_events.md) |[event](event.md)| Criar um novo Evento no calendário especificado ou padrão.|
|[Criar propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[calendar](calendar.md)  |Criar uma ou mais propriedades estendidas de valor único em um calendário novo ou existente.   |
|[Obter calendário com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_get.md)  | [calendar](calendar.md) | Obter calendários que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [calendar](calendar.md) | Criar uma ou mais propriedades estendidas de vários valores em um calendário novo ou existente.  |
|[Obter calendário com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_get.md)  | [calendar](calendar.md) | Obter um calendário que contenha uma propriedade estendida de vários valores usando `$expand`. |


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|canEdit |Boolean |Verdadeira se o usuário pode gravar o calendário, falsa caso contrário. Essa propriedade é verdadeira para o usuário que criou o calendário. Esta propriedade também é verdadeira para um usuário com o qual tenha sido compartilhado um calendário e tenha sido concedido acesso de gravação. |
|canShare |Boolean |Verdadeira se o usuário tem permissão para compartilhar o calendário, falsa caso contrário. Somente o usuário que criou o calendário pode compartilhá-lo. |
|canViewPrivateItems |Boolean |Verdadeira se o usuário pode ler itens do calendário que foram marcados como particulares, falsa caso contrário. |
|changeKey|String|Identifica a versão do objeto calendar. Toda vez que o calendário é alterado, a changeKey também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto. Somente leitura.|
|color|String|Especifica o tema de cores para distinguir o calendário de outros calendários em uma interface do usuário. Os valores de propriedade são: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1|
|id|String|O identificador exclusivo do grupo. Somente leitura.|
|name|String|O nome do calendário.|
|owner |[emailAddress](emailaddress.md) | Se definida, representa o usuário que criou ou adicionou o calendário. Para um calendário que o usuário criou ou adicionou, a propriedade **owner** é definida para o usuário. Para um calendário compartilhado com o usuário, a propriedade **owner** é definida para a pessoa que compartilhou o calendário com o usuário. |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|calendarView|Coleção [Event](event.md)|O modo de exibição do calendário. Propriedade de navegação. Somente leitura.|
|events|Coleção [Event](event.md)|Os eventos do calendário. Propriedade de navegação. Somente leitura.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para o calendário. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a mensagem. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendar"
}-->

```json
{
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
