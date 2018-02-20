# <a name="detectedapp-resource-type"></a>Tipo de recurso detectedApp

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Um aplicativo gerenciado ou não gerenciado que está instalado em um dispositivo gerenciado. Aplicativos não gerenciados só aparecerão para dispositivos marcados como controlados pela empresa.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar detectedApps](../api/intune_devices_detectedapp_list.md)|Coleção [detectedApp](../resources/intune_devices_detectedapp.md)|Lista propriedades e relações dos objetos [detectedApp](../resources/intune_devices_detectedapp.md).|
|[Obter detectedApp](../api/intune_devices_detectedapp_get.md)|[detectedApp](../resources/intune_devices_detectedapp.md)|Propriedades de leitura e relações do objeto [detectedApp](../resources/intune_devices_detectedapp.md).|
|[Criar detectedApp](../api/intune_devices_detectedapp_create.md)|[detectedApp](../resources/intune_devices_detectedapp.md)|Cria um novo objeto [detectedApp](../resources/intune_devices_detectedapp.md).|
|[Excluir detectedApp](../api/intune_devices_detectedapp_delete.md)|Nenhum|Exclui um [detectedApp](../resources/intune_devices_detectedapp.md).|
|[Atualizar detectedApp](../api/intune_devices_detectedapp_update.md)|[detectedApp](../resources/intune_devices_detectedapp.md)|Atualiza as propriedades de um objeto [detectedApp](../resources/intune_devices_detectedapp.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do aplicativo detectado. Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado. Somente leitura.|
|displayName|Cadeia de caracteres|Nome do aplicativo descoberto. Somente leitura|
|version|Cadeia de caracteres|Versão do aplicativo descoberto. Somente leitura|
|sizeInByte|Int64|Tamanho do aplicativo descoberto, em bytes. Somente leitura|
|deviceCount|Int32|O número de dispositivos que instalaram esse aplicativo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedDevices|Coleção [managedDevice](../resources/intune_devices_manageddevice.md)|Os dispositivos que descobriram o aplicativo instalado|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```



