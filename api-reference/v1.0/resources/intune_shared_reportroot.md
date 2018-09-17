# <a name="reportroot-resource-type"></a>Tipo de recurso reportRoot

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso que representa uma instância dos Relatórios de históricos.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter reportRoot](../api/intune_shared_reportroot_get.md)|[reportRoot](../resources/intune_shared_reportroot.md)|Ler propriedades e relações de objetos de [reportRoot](../resources/intune_shared_reportroot.md).|
|[Atualizar reportRoot](../api/intune_shared_reportroot_update.md)|[reportRoot](../resources/intune_shared_reportroot.md)|Atualizar as propriedades de um objeto [reportRoot](../resources/intune_shared_reportroot.md).|
|**Configuração do dispositivo**|
|[Função deviceConfigurationDeviceActivity](../api/intune_shared_reportroot_deviceconfigurationdeviceactivity.md)|[relatório](../resources/intune_shared_report.md)|Metadados para o relatório de atividade do dispositivo de configuração do dispositivo|
|[Função deviceConfigurationUserActivity](../api/intune_shared_reportroot_deviceconfigurationuseractivity.md)|[relatório](../resources/intune_shared_report.md)|Metadados para o Relatório de atividades do usuário de configuração do dispositivo|
|**Solução de problemas**|
|[Solução de problemas](../api/intune_shared_reportroot_manageddeviceenrollmentfailuredetails.md)|[relatório](../resources/intune_shared_report.md)|Ainda não documentado.|
|[Função managedDeviceEnrollmentTopFailures](../api/intune_shared_reportroot_manageddeviceenrollmenttopfailures.md)|[relatório](../resources/intune_shared_report.md)|Ainda não documentado.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo dessa entidade.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Aqui está uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a>Exemplo

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```