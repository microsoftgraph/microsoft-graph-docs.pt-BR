# <a name="managedioslobapp-resource-type"></a>managedIOSLobApp resource type

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades e propriedades herdadas para aplicativos de linha de negócios iOS gerenciados.

Herda de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedIOSLobApps](../api/intune_apps_managedioslobapp_list.md)|Coleção [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)|Lista propriedades e relações dos objetos [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).|
|[Obter managedIOSLobApp](../api/intune_apps_managedioslobapp_get.md)|[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)|Propriedades de leitura e relações do objeto [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).|
|[Criar managedIOSLobApp](../api/intune_apps_managedioslobapp_create.md)|[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)|Cria um novo objeto [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).|
|[Excluir managedIOSLobApp](../api/intune_apps_managedioslobapp_delete.md)|Nenhum|Exclui um [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).|
|[Atualizar managedIOSLobApp](../api/intune_apps_managedioslobapp_update.md)|[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)|Atualiza as propriedades de um objeto [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).|

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
|appAvailability|Cadeia de caracteres|A disponibilidade do Aplicativo. Herdado de [managedApp](../resources/intune_apps_managedapp.md). Os possíveis valores são: `global`, `lineOfBusiness`.|
|version|Cadeia de caracteres|A versão do Aplicativo. Herdado de [managedApp](../resources/intune_apps_managedapp.md)|
|committedContentVersion|Cadeia de caracteres|A versão do conteúdo interno confirmado. Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)|
|fileName|Cadeia de caracteres|O nome do arquivo do aplicativo Lob principal. Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)|
|size|Int64|O tamanho total, incluindo todos os arquivos carregados. Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)|
|bundleId|Cadeia de caracteres|O Nome da Identidade.|
|applicableDeviceType|[iosDeviceType](../resources/intune_apps_iosdevicetype.md)|A arquitetura do iOS na qual esse aplicativo pode ser executado.|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune_apps_iosminimumoperatingsystem.md)|O valor do sistema de operacional mínimo aplicável.|
|expirationDateTime|DateTimeOffset|O tempo de expiração.|
|versionNumber|Cadeia de caracteres|O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.|
|buildNumber|Cadeia de caracteres|O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|contentVersions|Coleção [mobileAppContent](../resources/intune_apps_mobileappcontent.md)|A lista das versões de conteúdo deste aplicativo. Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedIOSLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "bundleId": "String",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "expirationDateTime": "String (timestamp)",
  "versionNumber": "String",
  "buildNumber": "String"
}
```



