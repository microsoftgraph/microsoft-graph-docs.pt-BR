# <a name="managedappstatus-resource-type"></a>Tipo de recurso managedAppStatus

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa o status de proteção e configuração do aplicativo para a organização.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAppStatuses](../api/intune_mam_managedappstatus_list.md)|Conjunto [managedAppStatus](../resources/intune_mam_managedappstatus.md)|Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune_mam_managedappstatus.md).|
|[Obter managedAppStatus](../api/intune_mam_managedappstatus_get.md)|[managedAppStatus](../resources/intune_mam_managedappstatus.md)|Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune_mam_managedappstatus.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome amigável do relatório de status.|
|id|Cadeia de caracteres|Chave da entidade.|
|version|Cadeia de caracteres|Versão da entidade.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedAppStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



