# <a name="devicecomplianceactionitem-resource-type"></a>Tipo de recurso deviceComplianceActionItem

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configuração de ação agendada
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceComplianceActionItems](../api/intune_deviceconfig_devicecomplianceactionitem_list.md)|Conjunto [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|Listar propriedades e relações de objetos de [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).|
|[Obter deviceComplianceActionItem](../api/intune_deviceconfig_devicecomplianceactionitem_get.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|Ler propriedades e relações de objetos de [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).|
|[Criar deviceComplianceActionItem](../api/intune_deviceconfig_devicecomplianceactionitem_create.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|Criar um novo objeto de [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).|
|[Excluir deviceComplianceActionItem](../api/intune_deviceconfig_devicecomplianceactionitem_delete.md)|Nenhum|Excluir [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).|
|[Atualizar deviceComplianceActionItem](../api/intune_deviceconfig_devicecomplianceactionitem_update.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|Atualizar as propriedades de um objeto de [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|gracePeriodHours|Int32|Número de horas a aguardar até que a ação seja aplicada. Valores válidos de 0 a 8760|
|actionType|Cadeia de caracteres|Qual ação será executada Os valores possíveis são: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`.|
|notificationTemplateId|Cadeia de caracteres|Qual modelo de notificação de mensagem será usado|
|notificationMessageCCList|Conjunto de cadeia de caracteres|Uma lista de IDs de grupo para especificar quem receberá uma cópia dessa mensagem de notificação.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```



