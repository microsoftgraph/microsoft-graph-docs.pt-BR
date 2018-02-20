# <a name="deviceappmanagement-resource-type"></a>Tipo de recurso deviceAppManagement

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceAppManagement](../api/intune_apps_deviceappmanagement_get.md)|[deviceAppManagement](../resources/intune_apps_deviceappmanagement.md)|Propriedades de leitura e relações do objeto [deviceAppManagement](../resources/intune_apps_deviceappmanagement.md).|
|[Atualizar deviceAppManagement](../api/intune_apps_deviceappmanagement_update.md)|[deviceAppManagement](../resources/intune_apps_deviceappmanagement.md)|Atualiza as propriedades de um objeto [deviceAppManagement](../resources/intune_apps_deviceappmanagement.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|mobileApps|Coleção [mobileApp](../resources/intune_apps_mobileapp.md)|Os aplicativos móveis.|
|mobileAppCategories|Coleção [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|As categorias dos aplicativos móveis.|
|mobileAppConfigurations|Coleção [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)|As configurações de aplicativos móveis de gerenciamento de dispositivos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



