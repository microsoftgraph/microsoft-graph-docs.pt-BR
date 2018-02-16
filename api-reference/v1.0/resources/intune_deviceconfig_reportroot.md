# <a name="reportroot-resource-type"></a>Tipo de recurso reportRoot

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso que representa uma instância dos Relatórios de históricos.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter reportRoot](../api/intune_deviceconfig_reportroot_get.md)|[reportRoot](../resources/intune_deviceconfig_reportroot.md)|Ler propriedades e relações de objetos de [reportRoot](../resources/intune_deviceconfig_reportroot.md).|
|[Atualizar reportRoot](../api/intune_deviceconfig_reportroot_update.md)|[reportRoot](../resources/intune_deviceconfig_reportroot.md)|Atualizar as propriedades de um objeto de [reportRoot](../resources/intune_deviceconfig_reportroot.md).|
|[Função deviceConfigurationUserActivity](../api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity.md)|[relatório](../resources/intune_deviceconfig_report.md)|Metadados para o Relatório de atividades do usuário de configuração do dispositivo|
|[função deviceConfigurationDeviceActivity](../api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity.md)|[relatório](../resources/intune_deviceconfig_report.md)|Metadados para o relatório de atividade do dispositivo de configuração do dispositivo|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo dessa entidade.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```



