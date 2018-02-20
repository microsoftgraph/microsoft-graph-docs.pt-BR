# <a name="androidlobapp-resource-type"></a>androidLobApp resource type

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades e propriedades herdadas para aplicativos de linha de negócios Android.

Herda de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidLobApps](../api/intune_apps_androidlobapp_list.md)|Coleção [androidLobApp](../resources/intune_apps_androidlobapp.md)|Lista propriedades e relações dos objetos [androidLobApp](../resources/intune_apps_androidlobapp.md).|
|[Obter androidLobApp](../api/intune_apps_androidlobapp_get.md)|[androidLobApp](../resources/intune_apps_androidlobapp.md)|Propriedades de leitura e relações do objeto [androidLobApp](../resources/intune_apps_androidlobapp.md).|
|[Criar androidLobApp](../api/intune_apps_androidlobapp_create.md)|[androidLobApp](../resources/intune_apps_androidlobapp.md)|Cria um novo objeto [androidLobApp](../resources/intune_apps_androidlobapp.md).|
|[Excluir androidLobApp](../api/intune_apps_androidlobapp_delete.md)|Nenhum|Exclui um [androidLobApp](../resources/intune_apps_androidlobapp.md).|
|[Atualizar androidLobApp](../api/intune_apps_androidlobapp_update.md)|[androidLobApp](../resources/intune_apps_androidlobapp.md)|Atualiza as propriedades de um objeto [androidLobApp](../resources/intune_apps_androidlobapp.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|displayName|Cadeia de caracteres|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|description|Cadeia de caracteres|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|publisher|Cadeia de caracteres|O publicador do aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune_apps_mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|isFeatured|Booliano|O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|privacyInformationUrl|Cadeia de caracteres|A URL da declaração de privacidade. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|informationUrl|Cadeia de caracteres|A URL de informações adicionais. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|owner|Cadeia de caracteres|O proprietário do conteúdo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|developer|Cadeia de caracteres|O desenvolvedor do aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|notes|Cadeia de caracteres|Anotações para o aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|publishingState|Cadeia de caracteres|O estado de publicação para o aplicativo. O aplicativo não pode ser assinado, a menos que ele seja publicado. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.|
|committedContentVersion|Cadeia de caracteres|A versão do conteúdo interno confirmado. Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)|
|fileName|Cadeia de caracteres|O nome do arquivo do aplicativo Lob principal. Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)|
|size|Int64|O tamanho total, incluindo todos os arquivos carregados. Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)|
|packageId|Cadeia de caracteres|O identificador do pacote.|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune_apps_androidminimumoperatingsystem.md)|O valor do sistema de operacional mínimo aplicável.|
|versionName|Cadeia de caracteres|O nome da versão do aplicativo de Linha de Negócios (LoB) Android.|
|versionCode|Cadeia de caracteres|O código da versão do aplicativo de Linha de Negócios (LoB) Android.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|contentVersions|Coleção [mobileAppContent](../resources/intune_apps_mobileappcontent.md)|A lista das versões de conteúdo deste aplicativo. Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidLobApp",
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



