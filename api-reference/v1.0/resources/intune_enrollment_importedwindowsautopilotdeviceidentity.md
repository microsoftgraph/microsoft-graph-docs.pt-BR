# <a name="importedwindowsautopilotdeviceidentity-resource-type"></a>Tipo de recurso importedWindowsAutopilotDeviceIdentity

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Dispositivos importados do Windows AutoPilot.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar importedWindowsAutopilotDeviceIdentities](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_list.md)|Coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|Lista as propriedades e relações de objetos [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).|
|[Obter importedWindowsAutopilotDeviceIdentity](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_get.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|Lê as propriedades e relações do objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).|
|[Criar importedWindowsAutopilotDeviceIdentity](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_create.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|Crie um novo objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).|
|[Excluir importedWindowsAutopilotDeviceIdentity](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_delete.md)|Nenhum|Exclui uma [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).|
|[Atualizar importedWindowsAutopilotDeviceIdentity](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_update.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|Atualizar as propriedades de um objeto [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto.|
|orderIdentifier|Cadeia de caracteres|ID do pedido do dispositivo do Windows AutoPilot.|
|serialNumber|Cadeia de caracteres|Número de série do dispositivo do Windows AutoPilot.|
|productKey|Cadeia de caracteres|Chave do produto (Product Key) do dispositivo do Windows AutoPilot.|
|hardwareIdentifier|Binária|Blob de hardware do dispositivo do Windows AutoPilot.|
|state|[importedWindowsAutopilotDeviceIdentityState](../resources/intune_enrollment_importedwindowsautopilotdeviceidentitystate.md)|Estado atual do dispositivo importado.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "orderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "hardwareIdentifier": "binary",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "String",
    "deviceRegistrationId": "String",
    "deviceErrorCode": 1024,
    "deviceErrorName": "String"
  }
}
```



