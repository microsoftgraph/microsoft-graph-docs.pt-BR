# <a name="managedandroidlobapp-resource-type"></a>tipo de recurso managedAndroidLobApp

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades e propriedades herdadas para aplicativos de linha de negócios Android gerenciados.

Herda de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAndroidLobApps](../api/intune_apps_managedandroidlobapp_list.md)|Coleção [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)|Lista propriedades e relações dos objetos [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).|
|[Obter managedAndroidLobApp](../api/intune_apps_managedandroidlobapp_get.md)|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)|Propriedades de leitura e relações do objeto [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).|
|[Criar managedAndroidLobApp](../api/intune_apps_managedandroidlobapp_create.md)|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)|Cria um novo objeto [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).|
|[Excluir managedAndroidLobApp](../api/intune_apps_managedandroidlobapp_delete.md)|Nenhum|Exclui um [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).|
|[Atualizar managedAndroidLobApp](../api/intune_apps_managedandroidlobapp_update.md)|[managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)|Atualiza as propriedades de um objeto [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|displayName|Cadeia de caracteres|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|description|Cadeia de caracteres|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|publisher|Cadeia de caracteres|O publicador do aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|isFeatured|Booleano|O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|privacyInformationUrl|Cadeia de caracteres|A URL da declaração de privacidade. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|informationUrl|Cadeia de caracteres|A URL de informações adicionais. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|owner|Cadeia de caracteres|O proprietário do conteúdo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|developer|Cadeia de caracteres|O desenvolvedor do aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|Observações|Cadeia de caracteres|Anotações para o aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|O estado de publicação do aplicativo. O aplicativo não pode ser atribuído a menos que esteja publicado. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.|
|appAvailability|[managedAppAvailability](../resources/intune_apps_managedappavailability.md)|A disponibilidade do aplicativo. Herdada do [managedApp](../resources/intune_apps_managedapp.md). Os valores possíveis são: `global`, `lineOfBusiness`.|
|version|Cadeia de caracteres|A versão do Aplicativo. Herdado de [managedApp](../resources/intune_apps_managedapp.md)|
|committedContentVersion|Cadeia de caracteres|A versão do conteúdo interno confirmado. Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)|
|fileName|Cadeia de caracteres|O nome do arquivo do aplicativo Lob principal. Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)|
|size|Int64|O tamanho total, incluindo todos os arquivos carregados. Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)|
|packageId|Cadeia de caracteres|O identificador do pacote.|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune_apps_androidminimumoperatingsystem.md)|O valor do sistema de operacional mínimo aplicável.|
|versionName|Cadeia de caracteres|O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.|
|versionCode|Cadeia de caracteres|O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|contentVersions|Coleção [mobileAppContent](../resources/intune_apps_mobileappcontent.md)|A lista das versões de conteúdo deste aplicativo. Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedMobileLobApp",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAndroidLobApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "publishingState": "String",
  "appAvailability": "String",
  "version": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "packageId": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "String",
  "versionCode": "String"
}
```








