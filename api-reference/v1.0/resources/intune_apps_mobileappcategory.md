# <a name="mobileappcategory-resource-type"></a>Tipo de recurso mobileAppCategory

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém as propriedades para uma única categoria de aplicativo do Intune.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppCategories](../api/intune_apps_mobileappcategory_list.md)|Conjunto [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Listar propriedades e as relações de objetos de [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).|
|[Obter mobileAppCategory](../api/intune_apps_mobileappcategory_get.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Ler propriedades e relações de objetos de [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).|
|[Criar mobileAppCategory](../api/intune_apps_mobileappcategory_create.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Criar um novo objeto de [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).|
|[Excluir mobileAppCategory](../api/intune_apps_mobileappcategory_delete.md)|Nenhum|Excluir uma [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).|
|[Atualizar mobileAppCategory](../api/intune_apps_mobileappcategory_update.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Atualizar as propriedades de um objeto de [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave da entidade.|
|displayName|Cadeia de caracteres|O nome da categoria do aplicativo.|
|lastModifiedDateTime|DateTimeOffset|A data e hora que a mobileAppCategory foi modificada pela última vez.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mobileAppCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```



