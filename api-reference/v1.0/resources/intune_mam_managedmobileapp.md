# <a name="managedmobileapp-resource-type"></a>Tipo de recurso managedMobileApp

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O identificador da implantação de um aplicativo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedMobileApps](../api/intune_mam_managedmobileapp_list.md)|Conjunto [managedMobileApp](../resources/intune_mam_managedmobileapp.md)|Listar propriedades e relações de objetos de [managedMobileApp](../resources/intune_mam_managedmobileapp.md).|
|[Obter managedMobileApp](../api/intune_mam_managedmobileapp_get.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md)|Ler propriedades e relações de objetos de [managedMobileApp](../resources/intune_mam_managedmobileapp.md).|
|[Criar managedMobileApp](../api/intune_mam_managedmobileapp_create.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md)|Criar um novo objeto de[managedMobileApp](../resources/intune_mam_managedmobileapp.md).|
|[Excluir managedMobileApp](../api/intune_mam_managedmobileapp_delete.md)|Nenhum|Excluir [managedMobileApp](../resources/intune_mam_managedmobileapp.md).|
|[Atualizar managedMobileApp](../api/intune_mam_managedmobileapp_update.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md)|Atualizar as propriedades de um objeto de [managedMobileApp](../resources/intune_mam_managedmobileapp.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|O identificador de um aplicativo com seu tipo de sistema operacional.|
|id|Cadeia de caracteres|Chave da entidade.|
|versão|Cadeia de caracteres|Versão da entidade.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```



