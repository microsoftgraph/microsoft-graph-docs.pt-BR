# <a name="managedappoperation-resource-type"></a>Tipo de recurso managedAppOperation

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa uma operação aplicada a um registro de aplicativo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAppOperations](../api/intune_mam_managedappoperation_list.md)|Conjunto [managedAppOperation](../resources/intune_mam_managedappoperation.md)|Listar propriedades e relações de objetos de [managedAppOperation](../resources/intune_mam_managedappoperation.md).|
|[Obter managedAppOperation](../api/intune_mam_managedappoperation_get.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|Ler propriedades e relações de objetos de [managedAppOperation](../resources/intune_mam_managedappoperation.md).|
|[Criar managedAppOperation](../api/intune_mam_managedappoperation_create.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|Criar um novo objeto de[managedAppOperation](../resources/intune_mam_managedappoperation.md).|
|[Excluir managedAppOperation](../api/intune_mam_managedappoperation_delete.md)|Nenhum|Excluir [managedAppOperation](../resources/intune_mam_managedappoperation.md).|
|[Atualizar managedAppOperation](../api/intune_mam_managedappoperation_update.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|Atualizar as propriedades de um objeto de [managedAppOperation](../resources/intune_mam_managedappoperation.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome da operação.|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a operação de aplicativo foi modificada.|
|state|Cadeia de caracteres|O estado atual da operação|
|id|Cadeia de caracteres|Chave da entidade.|
|version|Cadeia de caracteres|Versão da entidade.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedAppOperation"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



