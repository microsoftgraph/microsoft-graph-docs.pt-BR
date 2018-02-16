# <a name="managedappstatusraw-resource-type"></a>tipo de recurso managedAppStatusRaw

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.

Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAppStatusRaws](../api/intune_mam_managedappstatusraw_list.md)|Conjunto [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)|Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).|
|[Obter managedAppStatusRaw](../api/intune_mam_managedappstatusraw_get.md)|[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)|Ler propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).|
|[Criar managedAppStatusRaw](../api/intune_mam_managedappstatusraw_create.md)|[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)|Criar um novo objeto de [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).|
|[Excluir managedAppStatusRaw](../api/intune_mam_managedappstatusraw_delete.md)|Nenhum|Excluir [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).|
|[Atualizar managedAppStatusRaw](../api/intune_mam_managedappstatusraw_update.md)|[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)|Atualizar as propriedades de um objeto de [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome amigável do relatório de status. Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)|
|id|Cadeia de caracteres|Chave da entidade. Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)|
|versão|Cadeia de caracteres|Versão da entidade. Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)|
|conteúdo|[Json](../resources/intune_mam_json.md)|Conteúdo do relatório de status.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



