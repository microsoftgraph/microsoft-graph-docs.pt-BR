# <a name="manageddevice-resource-type"></a>Tipo de recurso managedDevice

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Dispositivos gerenciados ou pré-registrados pelo Intune
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDevices](../api/intune_deviceconfig_manageddevice_list.md)|Conjunto [managedDevice](../resources/intune_deviceconfig_manageddevice.md)|Listar propriedades e relações de objetos de [managedDevice](../resources/intune_deviceconfig_manageddevice.md).|
|[Obter managedDevice](../api/intune_deviceconfig_manageddevice_get.md)|[managedDevice](../resources/intune_deviceconfig_manageddevice.md)|Ler propriedades e relações de objetos de [managedDevice](../resources/intune_deviceconfig_manageddevice.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceConfigurationStates|Conjunto [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|Estados de configuração deste dispositivo.|
|deviceCompliancePolicyStates|Conjunto [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)|Estados de política de conformidade deste dispositivo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)"
}
```



