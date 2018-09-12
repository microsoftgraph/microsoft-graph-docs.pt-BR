# <a name="edgesearchengine-resource-type"></a>Tipo de recurso edgeSearchEngine

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.

Herda de [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|edgeSearchEngineType|[edgeSearchEngineType](../resources/intune_deviceconfig_edgesearchenginetype.md)|Permite que os administradores de TI definam um mecanismo de pesquisa padrão predefinido para dispositivos controlados pelo MDM. Os valores possíveis são: `default`, `bing`.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```








