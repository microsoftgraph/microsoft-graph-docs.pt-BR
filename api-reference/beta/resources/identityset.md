# <a name="identityset-resource-type"></a>Tipo de recurso IdentitySet

O recurso **IdentitySet** é uma coleção de chaves dos recursos [identity](identity.md). É usado para representar uma coleção de identidades associada a vários eventos de um item, como _created by_ ou _last modified by_.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "user", "device", "application" ],
  "@odata.type": "microsoft.graph.identitySet"
}-->

```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a>Propriedades

| Propriedade	    | Tipo	                    | Descrição                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| application | [Identity](identity.md) | Opcional. O aplicativo associado a essa ação. |
| dispositivo      | [Identity](identity.md) | Opcional. O dispositivo associado a essa ação.      |
| Usuário        | [Identity](identity.md) | Opcional. O usuário associado a essa ação.        |

## <a name="remarks"></a>Comentários 

Consulte [DriveItem](driveitem.md) para saber mais sobre o uso de recursos **IdentitySet**.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
