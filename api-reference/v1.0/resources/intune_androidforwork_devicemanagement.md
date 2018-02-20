# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade singleton que atua como um contêiner da funcionalidade de configurações do Android for Work no gerenciamento de dispositivos.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune_androidforwork_devicemanagement_get.md)|[deviceManagement](../resources/intune_androidforwork_devicemanagement.md)|Propriedades de leitura e relações do objeto [deviceManagement](../resources/intune_androidforwork_devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune_androidforwork_devicemanagement_update.md)|[deviceManagement](../resources/intune_androidforwork_devicemanagement.md)|Atualiza as propriedades de um objeto [deviceManagement](../resources/intune_androidforwork_devicemanagement.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)|A entidade singleton de configurações do Android for Work.|
|androidForWorkAppConfigurationSchemas|Coleção [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)|Entidades do esquema de configuração do aplicativo Android for Work.|
|androidForWorkEnrollmentProfiles|Coleção [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|Entidades do perfil de registro do Android for Work.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



