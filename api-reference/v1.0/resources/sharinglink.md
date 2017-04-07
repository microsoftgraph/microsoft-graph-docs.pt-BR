# <a name="sharinglink-resource-type"></a>Tipo de recurso SharingLink

O recurso **SharingLink** agrupa itens de dados relacionados ao link em uma única estrutura.

Se um recurso [**Permission**](permission.md) tiver uma faceta **sharingLink** não nula, a permissão representará um link sharnig (em vez de permissões concedidas a uma pessoa ou um grupo).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "type": "view | edit",
  "scope": "anonymous | organization",
  "webUrl": "url"
}
```

## <a name="properties"></a>Propriedades

| Propriedade	    | Tipo	                    | Descrição                                                                                                                                                                                             |
|:------------|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| aplicativo | [identity](identity.md) | O aplicativo ao qual o link está associado.                                                                                                                                                                    |
| type        | String                  | O tipo do link criado.                                                                                                                                                                           |
| scope       | String                  | O escopo do link representado por esta permissão. O valor `anonymous` indica que o link é utilizável por qualquer pessoa; `organization` indica que o link só é útil para usuários conectados ao mesmo locatário. |
| webUrl      | String                  | Uma URL que abre o item no navegador no site do OneDrive.                                                                                                                                       |

## <a name="type-enumeration"></a>Enumeração Type

Esta tabela define os valores possíveis para a propriedade **type**:

| Valor   | Função    | Descrição                                                                     |
|:--------|:--------|:--------------------------------------------------------------------------------|
| `view`  | `read`  | Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.                            |
| `edit`  | `write` | Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.                               |

## <a name="scope-enumeration"></a>Enumeração de escopo

| Valor          | Descrição                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | O link de compartilhamento está disponível para uso por qualquer pessoa.                                                                            |
| `organization` | O link de compartilhamento está disponível para uso por qualquer pessoa na mesma organização (locatário). Não disponível para o OneDrive Personal. |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharingLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
