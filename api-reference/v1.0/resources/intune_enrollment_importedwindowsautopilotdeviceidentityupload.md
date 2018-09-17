# <a name="importedwindowsautopilotdeviceidentityupload-resource-type"></a>Tipo de recurso importedWindowsAutopilotDeviceIdentityUpload

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Importe os dispositivos do windows auropilot usando o carregamento.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista importedWindowsAutopilotDeviceIdentityUploads](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_list.md)|Coleção [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|Propriedades de lista e relacionamentos de objetos [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md).|
|[Obter importedWindowsAutopilotDeviceIdentityUpload](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_get.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|Propriedades de leitura e relacionamentos do objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) .|
|[Criar importedWindowsAutopilotDeviceIdentityUpload](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_create.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|Crie um novo objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) .|
|[Excluir importedWindowsAutopilotDeviceIdentityUpload](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_delete.md)|Nenhum|Exclui um [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md).|
|[Atualizar importedWindowsAutopilotDeviceIdentityUpload](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_update.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|Atualizar as propriedades de um objeto [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.|
|[Função autopilotDeviceStream](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_autopilotdevicestream.md)|Cadeia de caracteres|Crie uma solicitação de carregamento com fluxo de dispositivo do autopilot nela.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto.|
|createdDateTimeUtc|DateTimeOffset|DateTime quando a entidade é criada.|
|status|[importedWindowsAutopilotDeviceIdentityUploadStatus](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityuploadstatus.md)|Status de carregamento. Os valores possíveis são: `noUpload`, `pending`, `complete`, `error`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceIdentities|Coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|Coleção de todos os dispositivos de piloto automático como parte desse carregamento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "String (identifier)",
  "createdDateTimeUtc": "String (timestamp)",
  "status": "String"
}
```








