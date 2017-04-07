# <a name="timeconstraint-resource-type"></a>Tipo de recurso timeConstraint

Os períodos de tempo para uma atividade da natureza especificada.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|activityDomain|String|A natureza da atividade, opcional. Os valores possíveis são: `unknown`, `work`, `personal`. Atualmente, [findMeetingTimes](../api/user_findmeetingtimes.md) sempre pressupõe que o valor é `work` e retorna as sugestões de reunião somente durante o expediente do organizador ou do participante.|
|intervalos de tempo|Coleção [timeSlot](timeslot.md)|Uma matriz de períodos de tempo.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->