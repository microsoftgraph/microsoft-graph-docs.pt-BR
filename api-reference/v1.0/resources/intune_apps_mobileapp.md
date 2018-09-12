# <a name="mobileapp-resource-type"></a>Tipo de recurso mobileApp

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileApps](../api/intune_apps_mobileapp_list.md)|Coleção [mobileApp](../resources/intune_apps_mobileapp.md)|Lista propriedades e relações dos objetos [mobileApp](../resources/intune_apps_mobileapp.md).|
|[Obter mobileApp](../api/intune_apps_mobileapp_get.md)|[mobileApp](../resources/intune_apps_mobileapp.md)|Propriedades de leitura e relações do objeto [mobileApp](../resources/intune_apps_mobileapp.md).|
|[ação assign](../api/intune_apps_mobileapp_assign.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|displayName|Cadeia de caracteres|O título do aplicativo importado ou definido pelo administrador.|
|description|Cadeia de caracteres|A descrição do aplicativo.|
|publisher|Cadeia de caracteres|O publicador do aplicativo.|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez.|
|isFeatured|Booliano|O valor que indica se o aplicativo está marcado como em destaque pelo administrador.|
|privacyInformationUrl|Cadeia de caracteres|A URL da declaração de privacidade.|
|informationUrl|Cadeia de caracteres|A URL de informações adicionais.|
|owner|Cadeia de caracteres|O proprietário do conteúdo.|
|developer|Cadeia de caracteres|O desenvolvedor do aplicativo.|
|notes|Cadeia de caracteres|Anotações para o aplicativo.|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|O estado de publicação do aplicativo. O aplicativo não pode ser atribuído a menos esteja publicado. Os valores possíveis são: `notPublished`, `processing`, `published`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|A lista de categorias para este aplicativo.|
|assignments|Coleção [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String"
}
```








