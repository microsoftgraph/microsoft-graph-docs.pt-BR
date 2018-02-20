# <a name="iosstoreapp-resource-type"></a>Tipo de recurso iosStoreApp

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades e propriedades herdadas para aplicativos da loja iOS.

Herda de [mobileApp](../resources/intune_apps_mobileapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosStoreApps](../api/intune_apps_iosstoreapp_list.md)|Coleção [iosStoreApp](../resources/intune_apps_iosstoreapp.md)|Lista propriedades e relações dos objetos [iosStoreApp](../resources/intune_apps_iosstoreapp.md).|
|[Obter iosStoreApp](../api/intune_apps_iosstoreapp_get.md)|[iosStoreApp](../resources/intune_apps_iosstoreapp.md)|Propriedades de leitura e relações do objeto [iosStoreApp](../resources/intune_apps_iosstoreapp.md).|
|[Criar iosStoreApp](../api/intune_apps_iosstoreapp_create.md)|[iosStoreApp](../resources/intune_apps_iosstoreapp.md)|Cria um novo objeto [iosStoreApp](../resources/intune_apps_iosstoreapp.md).|
|[Excluir iosStoreApp](../api/intune_apps_iosstoreapp_delete.md)|Nenhum|Exclui um [iosStoreApp](../resources/intune_apps_iosstoreapp.md).|
|[Atualizar iosStoreApp](../api/intune_apps_iosstoreapp_update.md)|[iosStoreApp](../resources/intune_apps_iosstoreapp.md)|Atualiza as propriedades de um objeto [iosStoreApp](../resources/intune_apps_iosstoreapp.md).|

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
|bundleId|Cadeia de caracteres|O Nome da Identidade.|
|appStoreUrl|Cadeia de caracteres|A URL da Apple App Store|
|applicableDeviceType|[iosDeviceType](../resources/intune_apps_iosdevicetype.md)|A arquitetura do iOS na qual esse aplicativo pode ser executado.|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune_apps_iosminimumoperatingsystem.md)|O valor do sistema de operacional mínimo aplicável.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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
  "bundleId": "String",
  "appStoreUrl": "String",
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
  }
}
```



