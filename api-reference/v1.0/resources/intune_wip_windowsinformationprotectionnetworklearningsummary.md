# <a name="windowsinformationprotectionnetworklearningsummary-resource-type"></a>Tipo de recurso windowsInformationProtectionNetworkLearningSummary

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade de resumo de aprendizagem da Rede de Proteção de Informações do Windows
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsInformationProtectionNetworkLearningSummaries](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_list.md)|Conjunto [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)|Listar propriedades e relações de objetos de [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md).|
|[Obter windowsInformationProtectionNetworkLearningSummary](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_get.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)|Ler propriedades e relações de objetos de [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md).|
|[Criar windowsInformationProtectionNetworkLearningSummary](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_create.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)|Criar um novo objeto de [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md).|
|[Excluir windowsInformationProtectionNetworkLearningSummary](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_delete.md)|Nenhum|Excluir [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md).|
|[Atualizar windowsInformationProtectionNetworkLearningSummary](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_update.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)|Atualizar as propriedades de um objeto de [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo de WindowsInformationProtectionNetworkLearningSummary.|
|url|Cadeia de caracteres|Url do site|
|deviceCount|Int32|Contagem de dispositivos|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.windowsInformationProtectionNetworkLearningSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "String (identifier)",
  "url": "String",
  "deviceCount": 1024
}
```



