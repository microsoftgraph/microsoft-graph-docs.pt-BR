# <a name="macosofficesuiteapp-resource-type"></a>Tipo de recurso macOSOfficeSuiteApp

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades e propriedades herdadas do aplicativo do MacOS Office Suite.

Herda de [mobileApp](../resources/intune_apps_mobileapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSOfficeSuiteApps](../api/intune_apps_macosofficesuiteapp_list.md)|Coleção [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md)|Lista propriedades e relações dos objetos [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).|
|[Obter macOSOfficeSuiteApp](../api/intune_apps_macosofficesuiteapp_get.md)|[macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md)|Propriedades de leitura e relações do objeto [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).|
|[Criar macOSOfficeSuiteApp](../api/intune_apps_macosofficesuiteapp_create.md)|[macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md)|Cria um novo objeto [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).|
|[Excluir macOSOfficeSuiteApp](../api/intune_apps_macosofficesuiteapp_delete.md)|Nenhum|Exclui um [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).|
|[Atualizar macOSOfficeSuiteApp](../api/intune_apps_macosofficesuiteapp_update.md)|[macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md)|Atualiza as propriedades de um objeto [ macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|displayName|Cadeia de caracteres|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|descrição|Cadeia de caracteres|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|publicador|Cadeia de caracteres|O publicador do aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|isFeatured|Booleano|O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|privacyInformationUrl|Cadeia de caracteres|A URL da declaração de privacidade. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|informationUrl|Cadeia de caracteres|A URL de informações adicionais. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|proprietário|Cadeia de caracteres|O proprietário do conteúdo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|desenvolvedor|Cadeia de caracteres|O desenvolvedor do aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|Observações|Cadeia de caracteres|Anotações para o aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|O estado de publicação do aplicativo. O aplicativo não pode ser atribuído a menos que esteja publicado. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categorias|Coleção [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|atribuições|Coleção [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileApp",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSOfficeSuiteApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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








