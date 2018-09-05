# <a name="onpremisesextensionattributes-resource-type"></a>tipo de recurso onPremisesExtensionAttributes

A propriedade **onPremisesExtensionAttributes** da entidade [usuário](user.md) contém quinze propriedades de extensão personalizada de atributo. Para um usuário **onPremisesSyncEnabled**, esse conjunto de propriedades é administrado no Active Directory local e sincronizado com o Azure AD, e é somente para leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensionAttribute1|Sequência de caracteres| Primeiro atributo de extensão personalizável. |
|extensionAttribute2|Sequência de caracteres| Segundo atributo de extensão personalizável. |
|extensionAttribute3|Sequência de caracteres| Terceiro atributo de extensão personalizável. |
|extensionAttribute4|Sequência de caracteres| Quarto atributo de extensão personalizável. |
|extensionAttribute5|Sequência de caracteres| Quinto atributo de extensão personalizável. |
|extensionAttribute6|Sequência de caracteres| Sexto atributo de extensão personalizável. |
|extensionAttribute7|Sequência de caracteres| Sétimo atributo de extensão personalizável. |
|extensionAttribute8|Sequência de caracteres| Oitavo atributo de extensão personalizável. |
|extensionAttribute9|Sequência de caracteres| Nono atributo de extensão personalizável. |
|extensionAttribute10|Sequência de caracteres| Décimo atributo de extensão personalizável. |
|extensionAttribute11|Sequência de caracteres| Décimo primeiro atributo de extensão personalizável. |
|extensionAttribute12|Sequência de caracteres| Décimo segundo atributo de extensão personalizável. |
|extensionAttribute13|Sequência de caracteres| Décimo terceiro atributo de extensão personalizável. |
|extensionAttribute14|Sequência de caracteres| Décimo quarto atributo de extensão personalizável. |
|extensionAttribute15|Sequência de caracteres| Décimo quinto atributo de extensão personalizável. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->