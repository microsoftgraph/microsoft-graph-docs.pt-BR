# <a name="mobileappcontent-resource-type"></a>Tipo de recurso mobileAppContent

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppContents](../api/intune_apps_mobileappcontent_list.md)|Conjunto [mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Listar propriedades e relações de objetos de [mobileAppContent](../resources/intune_apps_mobileappcontent.md).|
|[Obter mobileAppContent](../api/intune_apps_mobileappcontent_get.md)|[mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Ler propriedades e relações de objetos de [mobileAppContent](../resources/intune_apps_mobileappcontent.md).|
|[Criar mobileAppContent](../api/intune_apps_mobileappcontent_create.md)|[mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Criar um novo objeto de [mobileAppContent](../resources/intune_apps_mobileappcontent.md).|
|[Excluir mobileAppContent](../api/intune_apps_mobileappcontent_delete.md)|Nenhum|Excluir [mobileAppContent](../resources/intune_apps_mobileappcontent.md).|
|[Atualizar mobileAppContent](../api/intune_apps_mobileappcontent_update.md)|[mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Atualizar as propriedades de um objeto de [mobileAppContent](../resources/intune_apps_mobileappcontent.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A versão do conteúdo do aplicativo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|arquivos|Conjunto [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)|A lista dos arquivos desta versão de conteúdo do aplicativo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```



