# <a name="shared-resource-type"></a>Tipo de recurso compartilhado

O recurso **Shared** indica que um DriveItem foi compartilhado com outras pessoas. O recurso inclui informações sobre como o item é compartilhado.

Se um [**Driveitem**](driveitem.md) tem uma faceta **shared** não nula, o item foi compartilhada.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shared",
  "optionalProperties": [ "sharedBy", "sharedDateTime" ]
}-->

```json
{
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "scope": "public | organization | users",
  "sharedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "sharedDateTime": "datetime"
}
```

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                          | Descrição                                                                                        |
| :------------- | :---------------------------- | :------------------------------------------------------------------------------------------------- |
| owner          | [IdentitySet](identityset.md) | A identidade do proprietário do item compartilhado. Somente leitura.                                           |
| escopo          | String                        | Indica o escopo de como o item é compartilhado: `anonymous`, `organization` ou `users`. Somente leitura. |
| sharedBy       | [identitySet](identityset.md) | A identidade do usuário que compartilhou o item. Somente leitura.                                           |
| sharedDateTime | DateTimeOffset                | A data e a hora UTC que o item foi compartilhado. Somente leitura.                                         |

## <a name="scope-values"></a>Valores de escopo

| Valor        | Descrição                                                                           |
|:-------------|:--------------------------------------------------------------------------------------|
| public       | O item é compartilhado usando-se um link que funciona para qualquer pessoa que tem o link.               |
| organização | O item é compartilhado usando-se um link que funciona para qualquer pessoa na organização do proprietário. |
| usuários        | O item é compartilhado apenas com usuários específicos.                                          |

## <a name="remarks"></a>Comentários

Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shared resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
