# <a name="microsoftstoreforbusinessapp-resource-type"></a>Tipo de recurso microsoftStoreForBusinessApp

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Aplicativos da Microsoft Store for Business. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.

Herda de [mobileApp](../resources/intune_apps_mobileapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar microsoftStoreForBusinessApps](../api/intune_apps_microsoftstoreforbusinessapp_list.md)|Coleção [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)|Lista propriedades e relações dos objetos [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).|
|[Obter microsoftStoreForBusinessApp](../api/intune_apps_microsoftstoreforbusinessapp_get.md)|[microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)|Propriedades de leitura e relações do objeto [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).|
|[Criar microsoftStoreForBusinessApp](../api/intune_apps_microsoftstoreforbusinessapp_create.md)|[microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)|Cria um novo objeto [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).|
|[Excluir microsoftStoreForBusinessApp](../api/intune_apps_microsoftstoreforbusinessapp_delete.md)|Nenhum|Exclui um [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).|
|[Atualizar microsoftStoreForBusinessApp](../api/intune_apps_microsoftstoreforbusinessapp_update.md)|[microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)|Atualiza as propriedades de um objeto [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).|

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
|usedLicenseCount|Int32|O número de aplicativos da Microsoft Store for Business em uso.|
|totalLicenseCount|Int32|O número total de aplicativos da Microsoft Store for Business.|
|productKey|Cadeia de caracteres|A chave de produto do aplicativo|
|licenseType|[microsoftStoreForBusinessLicenseType](../resources/intune_apps_microsoftstoreforbusinesslicensetype.md)|O tipo de licença do aplicativo Os valores possíveis são: `offline`, `online`.|
|packageIdentityName|Cadeia de caracteres|O identificador do pacote do aplicativo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileApp",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "productKey": "String",
  "licenseType": "String",
  "packageIdentityName": "String"
}
```








