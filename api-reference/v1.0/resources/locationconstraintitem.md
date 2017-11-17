# <a name="locationconstraintitem-resource-type"></a>Tipo de recurso locationConstraintItem

As condições indicadas por um cliente para o local de uma reunião.

Derivado de [location](location.md).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  
  ],
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
| address | [physicalAddress](physicalAddress.md) |O endereço físico do local. |
| displayName  | Cadeia de caracteres | O nome associado ao local.                       |
| locationEmailAddress | Cadeia de caracteres | O endereço de email opcional do local. |
| resolveAvailability | Boolean | Se definido como true e o recurso especificado está ocupado, [findMeetingTimes](../api/user_findmeetingtimes.md) procura outro recurso livre. Se definido como false e o recurso especificado está ocupado, **findMeetingTimes** retorna o recurso melhor classificado no cache do usuário sem verificar se ele está livre. O padrão é true. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->